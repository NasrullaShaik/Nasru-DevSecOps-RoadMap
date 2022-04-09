# Yaml Overviews

| kind       | version |
| ---------- | ------- |
| POD        | v1      |
| Service    | v1      |
| Replication Controller | v1 |
| ReplicaSet | apps/v1 |
| Deployment | apps/v1 |

## Pod Yaml

**Image Pull Policy Options under `spec`**

When creating the POD, one can specify the imagePullPolicyspecification, which guides the Kubelet service on how to pull the specified image during an update. In the above example, it has been set to Always, which means Kubernetes should always pull the image from the registry when updating the container.

There are three image policy pull options for Kubernetes.

If imagePullPolicy is set to Always, Kubernetes will always pull the image from the Repository.
With IfNotPresent, Kubernetes will only pull the image when it does not already exist on the node.
While with imagePullPolicy set to Never, Kubernetes will never pull the image.

**Restart Policies Options under `spec`:**

There are three possible values for a pod’s restart policy in Kubernetes:

- Always
- OnFailure &
- Never

Note: Only a .spec.template.spec.restartPolicy equal to Always is allowed, which is the default if not specified.

Is the same case for DaemonSets, ReplicaSets, ReplicationController.

**DNS Policy for Pods, Services Under `spec`:**
[DNS Policy](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/)

## Multi Pod Containers YAML

The multiple containers inside the pod are life partners :-)

- They are created and killed together when a pod is created or deleted.
- They share the same network space and can communicate with each other as localhost.
- They have access to the same storage volumes.

## Init Containers YAML

In a multi-container pod, each container is expected to run a process that stays alive as long as the POD's life cycle. For example in the multi-container pod that we talked about earlier that has a web application and logging agent, both the containers are expected to stay alive at all times. The process running in the log agent container is expected to stay alive as long as the web application is running. If any of them fails, the POD restarts.

But at times you may want to run a process that runs to completion in a container. For example a process that pulls a code or binary from a repository that will be used by the main web application. That is a task that will be run only  one time when the pod is first created. Or a process that waits  for an external service or database to be up before the actual application starts. That's where initContainers comes in.

An initContainer is configured in a pod like all other containers, except that it is specified inside a initContainers section.

## Command vs Argument in Kubernetes Objects Under `spec.containers`

-> Argument

```sh $ kubectl run busybox --image=busybox --restart=Never -o yaml --dry-run -- /bin/sh -c 'echo hello;sleep 3600'```

-> Command

```sh $kubectl run busybox --image=busybox --restart=Never -o yaml --dry-run --command /bin/sh -c 'echo hello;sleep 3600'```

When working with containers in Kubernetes, you should be careful not to mix up **Kubenetes command** and **Docker Cmd**.

the **command** field in Kubernetes corresponds to the **EntryPoint** field in Docker
the **args** field in Kubernetes corresponds to the **Cmd** field in Docker
From [Kubernets documentation](https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#notes):

When you override the default Entrypoint and Cmd, these rules apply:

- If you do not supply command or args for a Container, the defaults defined in the Docker image are used.
- If you supply a command but no args for a Container, only the supplied command is used. The default EntryPoint and the default Cmd defined in the Docker image are ignored.
- If you supply only args for a Container, the default Entrypoint defined in the Docker image is run with the args that you supplied.
- If you supply a command and args, the default Entrypoint and the default Cmd defined in the Docker image are ignored. Your command is run with your args.

```yaml
spec:
  containers:
  - name: command-demo-container
    image: debian
    command: ["printenv"]
    args: ["HOSTNAME", "KUBERNETES_PORT"]
  restartPolicy: OnFailure

#or

env:
- name: MESSAGE
  value: "hello world"
command: ["/bin/echo"]
args: ["$(MESSAGE)"]

#only Args

args:
  - /bin/sh
  - -c
  - touch /tmp/healthy; sleep 30; rm -rf /tmp/healthy; sleep 600
```

Once the Pod Object created use below command to create `pod`

```sh kubectl create -f pod-Defination.yml``` or ```sh kubectl run <name of pod> --image=<name of the image from registry>```

```sh kubectl create -f init-Pod.yml```

```sh kubectl create -f Multi-Pod.yaml```

## Controllers

- Kubernetes had many controllers. Controllers in the Kubernetes do much work. They act as the brain for Kubernetes. In this article, we are going to see Replication controller(old technology) and ReplicaSets(new technology). Both Replication Controller and ReplicaSets will do the same task. However, they are not the same. They had minor differences. We will see the difference later.

- In simple terms, Replication Controller/ReplicaSets is used to run multiple instances of a single Pod to achieve load balancing and high availability. This can be done by simply mentioning the replicas count in the YAML file. If any Pod dies, then the controller will re-create a new one by watching the Pod status.

1. Creating multiple instances of the same application using the replicas option.
2. Re-create a new Pod when the Pod dies.

## Deployments

-> Rollout and Versioning

- Before we look at how we upgrade our application, let’s try to understand Rollouts and Versioning in a deployment. Whenever you create a new deployment or upgrade the images in an existing deployment trigger a Rollout.
- A rollout is the process of gradually deploying or upgrading your application containers. When you first create a deployment, it triggers a rollout.
- A new rollout creates a new Deployment revision. Let’s call it revision 1.
- In the future when the application is upgraded – meaning
- when the container version is updated to a new one – a new rollout is triggered and a a new deployment revision is created named Revision 2.
- This helps us keep track of the changes made to our deployment and enables us to rollback to a previous version of deployment if necessary.
- You can see the status of your rollout by running the command

```sh kubectl rollout history deployment nginx-deploy```

-> Deployment Strategy

- There are two types of deployment strategies.
  - Say for example you have 5 replicas of your web application instance deployed.
  - One way to upgrade these to a newer version is to destroy all of these and then create newer versions of application instances.
  - Meaning first, destroy the 5 running instances and then deploy 5 new instances of the new application version.
  - The problem with this, as you can imagine, is that during the period after the older versions are down and before any newer version is up, the application is down and inaccessible to users.
  - This strategy is known as the Recreate strategy, and thankfully this is NOT the default deployment strategy.

- The second strategy is where we do not destroy all of them at once. Instead we take down the older version and bring up a newer version one by one. This way the application never goes down and the upgrade is seamless. Remember, if you do not specify a strategy while creating the deployment, it will assume it to be a Rolling Update. In other words, RollingUpdate is the default Deployment Strategy.

```sh
#Configure -- First Strategy
kubectl apply -f Deployment.yml

#update -- Second Strategy
kubectl set image deployment/nginx-deploy nginx=nginx:1.9.1
```

-> Difference b/w recreate and rolling updates

- The difference between the recreate and rolling update strategies can also be seen when you view the deployments in detail.
- Run the kubectl describe deployment command to see detailed information regarding the deployments.
- You will notice when the **Recreate strategy** was used the events indicate that the old replica set was scaled down to 0 first and the new replica set scaled up to 5.
- However when the **RollingUpdate strategy** was used the old replica set was scaled down one at a time simultaneously scaling up the new replica set one at a time.

-> Rollback

- Say for instance once you upgrade your application, you realise something isn’t very right. Something’s wrong with the new version of the build you used to upgrade. So you would like to rollback your update. Kubernetes deployments allow you to rollback to a previous revision. To undo a change run the command kubectl rollout undo followed by the name of the deployment.
- The deployment will then destroy the PODs in the new replica set and bring the older ones up in the old replica set. And your application is back to its older format. When you compare the output of the kubectl get replicasets command, before and after the rollback, you will be able to notice this difference. Before the rollback the first replicaset had 0 PODs and the new replica set had 5 PODs and this is reversed after the rollback is finished.

```sh
kubectl rollout undo deployment/nginx-deploy
```

## Services

```sh
# To create the respective type of service
kubectl create -f <service-definition file>

#Check service created and status
kubectl get services

#Test Connections
curl http://192.168.1.2:30008

#Using Minikube
minikube service <servicename> --url
```
