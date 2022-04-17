# DevSecOps

- [DevSecOps](#devsecops)
  - [SDLC](#sdlc)
    - [What is SDLC?](#what-is-sdlc)
    - [Process Of SDLC](#process-of-sdlc)
  - [Types Of SDLC Models](#types-of-sdlc-models)
    - [Waterfall Model](#waterfall-model)
    - [Agile Model](#agile-model)
      - [Agile Implementation](#agile-implementation)
    - [DevOps Model](#devops-model)
      - [What is DevOps](#what-is-devops)
      - [Why we need DevOps](#why-we-need-devops)
      - [How DevOps Works (LifeCycle Of DevOps)?](#how-devops-works-lifecycle-of-devops)
      - [DevOps Culture](#devops-culture)
      - [Adopting DevOps](#adopting-devops)
      - [Principles Of DevOps](#principles-of-devops)
      - [Framwork In DevOps](#framwork-in-devops)
      - [DevOps and Cloud-Native Development](#devops-and-cloud-native-development)
      - [DevSecOps Detailed](#devsecops-detailed)
      - [SRE](#sre)
      - [Diffrence B/W Waterfall vs Agile vs DevOps](#diffrence-bw-waterfall-vs-agile-vs-devops)
      - [Advantages and DisAdvantages](#advantages-and-disadvantages)
      - [Roles and Responsibilies](#roles-and-responsibilies)
      - [DevOps Tools](#devops-tools)
  - [**kubernetes-Beginners**](#kubernetes-beginners)
    - [Kubernetes Basics](#kubernetes-basics)
    - [Kubernetes Overview](#kubernetes-overview)
      - [Container Orchestration](#container-orchestration)
      - [Kubernetes Advantages](#kubernetes-advantages)
    - [Kubernetes Architechture](#kubernetes-architechture)
    - [SetUp Kubernetes](#setup-kubernetes)
    - [Kubernetes Concepts - Pods, ReplicaSets, Deployments](#kubernetes-concepts---pods-replicasets-deployments)
    - [Networking in Kubernets](#networking-in-kubernets)
      - [Internal Networking](#internal-networking)
      - [Cluster Networking](#cluster-networking)
    - [Services](#services)
      - [Service Types](#service-types)
    - [MicroServices Architechture](#microservices-architechture)
      - [Deploying an application on Docker](#deploying-an-application-on-docker)
      - [Deploying an application on kubernetes cluster](#deploying-an-application-on-kubernetes-cluster)
    - [Kubernetes On Cloud](#kubernetes-on-cloud)
    - [Kubernets vs Docker Swarm](#kubernets-vs-docker-swarm)
      - [What is Kubernetes?](#what-is-kubernetes)
        - [Pros of Kubernetes](#pros-of-kubernetes)
        - [Cons of Kubernetes](#cons-of-kubernetes)
      - [What is Docker Swarm?](#what-is-docker-swarm)
        - [Pros of Docker Swarm](#pros-of-docker-swarm)
        - [Cons of Docker Swarm](#cons-of-docker-swarm)
      - [K8s vs K3s](#k8s-vs-k3s)
  - [**Kubernetes Development**](#kubernetes-development)
    - [What is Kubernets?](#what-is-kubernets)
    - [Demo App in Kubernets](#demo-app-in-kubernets)
    - [Docker Container for App](#docker-container-for-app)
    - [Kubernetes On Minikube](#kubernetes-on-minikube)
    - [Moving to Azure AKS](#moving-to-azure-aks)
    - [DevOps for Kubernetes using Azure DevOps](#devops-for-kubernetes-using-azure-devops)
    - [CI/CD Pipelines for Kubernetes using YAML pipelines](#cicd-pipelines-for-kubernetes-using-yaml-pipelines)
    - [Deploying using Helm](#deploying-using-helm)
    - [Ingress Controller](#ingress-controller)
    - [GitOps with Kubernetes](#gitops-with-kubernetes)
    - [Kubernetes NodePools](#kubernetes-nodepools)
    - [Upgrade the Cluster](#upgrade-the-cluster)
    - [Cluster backup](#cluster-backup)
  - [**Kubernetes Administration**](#kubernetes-administration)
    - [Introduction](#introduction)
    - [Core Concepts](#core-concepts)
      - [Cluster Architechture](#cluster-architechture)
        - [ETCD](#etcd)
        - [kube-apiserver](#kube-apiserver)
        - [kube-controller-manager](#kube-controller-manager)
        - [kube-scheduler](#kube-scheduler)
        - [Kubelet](#kubelet)
        - [Container runtime](#container-runtime)
        - [Kube-Proxy](#kube-proxy)
    - [Scheduling](#scheduling)
      - [Manual Scheduling](#manual-scheduling)
      - [Labels and Selectors](#labels-and-selectors)
      - [Taint and Toleration](#taint-and-toleration)
      - [Node Selectors](#node-selectors)
      - [Node Affinity](#node-affinity)
      - [Taint and Toleration vs Node Affinity](#taint-and-toleration-vs-node-affinity)
      - [Resource Requirements and Limits](#resource-requirements-and-limits)
      - [Editing Pods and Deployments](#editing-pods-and-deployments)
      - [Daemon Sets](#daemon-sets)
      - [Static pods](#static-pods)
      - [Multiple Scheduler](#multiple-scheduler)
      - [Configure K8s Scheduler](#configure-k8s-scheduler)
    - [Logging and Monotoring](#logging-and-monotoring)
      - [Monitor Cluster Components](#monitor-cluster-components)
      - [Manage Application Logs](#manage-application-logs)
    - [Application Lifecycle Management](#application-lifecycle-management)
      - [Rolling Updates and Rollbacks](#rolling-updates-and-rollbacks)
      - [Commands and Arguments](#commands-and-arguments)
      - [Env Variables](#env-variables)
      - [Secrets](#secrets)
      - [ConfigMap](#configmap)
      - [Scale Application](#scale-application)
      - [Multi Container](#multi-container)
      - [Init Container](#init-container)
      - [Probes](#probes)
      - [Jobs](#jobs)
      - [Self-Healing](#self-healing)
    - [Cluster Maintainance](#cluster-maintainance)
      - [OS Upgrades](#os-upgrades)
      - [Kubernetes Software Version](#kubernetes-software-version)
      - [Cluster Upgrade Process](#cluster-upgrade-process)
      - [BackUp and Restore Method](#backup-and-restore-method)
      - [Working with ETCDCTL](#working-with-etcdctl)
    - [Security](#security)
      - [Kubernetes Security Primitives](#kubernetes-security-primitives)
      - [Authentication](#authentication)
      - [TLS Introduction](#tls-introduction)
      - [TLS in Basics](#tls-in-basics)
      - [TLS in Kubernetes](#tls-in-kubernetes)
      - [TLS in Kubernetes - certificatin details](#tls-in-kubernetes---certificatin-details)
      - [Certificate API](#certificate-api)
      - [Kubeconfig](#kubeconfig)
      - [Persistance key/value pair](#persistance-keyvalue-pair)
      - [API Groups](#api-groups)
      - [Authorization](#authorization)
      - [Role Based Access Controll](#role-based-access-controll)
      - [Cluster Role and Role Binding](#cluster-role-and-role-binding)
      - [Service Account](#service-account)
      - [Image Security](#image-security)
      - [Security Context](#security-context)
      - [Network Polocies](#network-polocies)
      - [Developing Network Policies](#developing-network-policies)
    - [Storage](#storage)
      - [Intoduction to Docker Storage](#intoduction-to-docker-storage)
      - [Storage in Docker](#storage-in-docker)
      - [Volume Driver Plugin in Docker](#volume-driver-plugin-in-docker)
      - [Container Storage Interface](#container-storage-interface)
      - [Volumes](#volumes)
      - [Persistent Volumes](#persistent-volumes)
      - [Persistent Volume Claims](#persistent-volume-claims)
      - [Using PVC's in Pods](#using-pvcs-in-pods)
      - [Application Configuration](#application-configuration)
      - [Additional Topics](#additional-topics)
      - [Storage Class](#storage-class)
    - [Network](#network)
      - [DNS](#dns)
      - [CoreDNS](#coredns)
      - [Network Namespace](#network-namespace)
      - [FAQ](#faq)
      - [Docker Network](#docker-network)
      - [CNI](#cni)
      - [Cluster Network](#cluster-network)
      - [Pod Network](#pod-network)
      - [CNI in Kubernetes](#cni-in-kubernetes)
      - [CNI Weave](#cni-weave)
      - [IP Address Management - Weave](#ip-address-management---weave)
      - [Service Network](#service-network)
      - [DNS in Kubernetes](#dns-in-kubernetes)
      - [Core DNS in Kubernetes](#core-dns-in-kubernetes)
      - [Ingress](#ingress)
    - [Design and Install Kubernetes Cluster](#design-and-install-kubernetes-cluster)
      - [Design Kubernetes Cluster](#design-kubernetes-cluster)
      - [Choose Kubernetes Infrastructure](#choose-kubernetes-infrastructure)
      - [Configure High Availability](#configure-high-availability)
      - [ETCD in HA](#etcd-in-ha)
    - [Install Kubernets hardway](#install-kubernets-hardway)
      - [Resources](#resources)
      - [Deploy with Kubeadm](#deploy-with-kubeadm)
    - [End to End Test on a kubernets Cluster](#end-to-end-test-on-a-kubernets-cluster)
    - [Troubleshooting](#troubleshooting)
      - [Application Failure](#application-failure)
      - [Control Plane Failure](#control-plane-failure)
      - [Worker Node Failuer](#worker-node-failuer)
      - [Network Troubleshooting](#network-troubleshooting)
      - [Other Topics](#other-topics)
        - [JSON Path](#json-path)
        - [Advance Kubectl Commands](#advance-kubectl-commands)
    - [**Kubernetes Master Course**](#kubernetes-master-course)
      - [Kubernetes Introduction](#kubernetes-introduction)
      - [Understanding the Kubernetes Architechture](#understanding-the-kubernetes-architechture)
      - [Installing and Maintaining The Kubeadm Cluster](#installing-and-maintaining-the-kubeadm-cluster)
      - [Kubernetes Core Concepts](#kubernetes-core-concepts)
      - [Workloads in Kubernetes](#workloads-in-kubernetes)
      - [Scheduling In Kubernetes](#scheduling-in-kubernetes)
      - [Configuring Application](#configuring-application)
      - [Networking In Kubernetes](#networking-in-kubernetes)
      - [Storage In Kubernetes](#storage-in-kubernetes)
      - [Security In Kubernetes](#security-in-kubernetes)
      - [Monitoring and Autoscaling kubernetes Cluster](#monitoring-and-autoscaling-kubernetes-cluster)

--------------------------------------

## SDLC

### What is SDLC?

An SDLC goal is to develop a high quality system that meets or exceeds customer expectations, is cost effective to maintain and enhance, and works effectively in the existing and planned IT infrastructure.

In Simple Words SDLC aims for:

1. High Quality System that meets or exceeds customer expectations.
2. Cost effective to maintain and enhance.
3. Existing IT infrastructure products should work effectively.

### Process Of SDLC

1. Requirement Phase
Business analysts collect the requirement from the customer/client as per the client business needs and documents the requirement in the **Business Requirement Specification (BRS)** and provides the same to the Development team.
2. Analysis Phase
Once the requirement gathering is done the next step is to define and document the product requirement and get approved from the customer/client. This is done through the **Software Requirement Specification document (SRS)**.

Key people involved in this phase are Project manager, Business Analyst, and Senior member in the team.

The outcome of the phase is **Software Requirement Specification (SRS)**.
3. Design Phase

  1. **High Level Document (HLD)**: It gives the architecture of the software project to be developed and is done by architects and senior developers.
  2. **Low Level Document (LLD)**: It is done by Senior developers. It describes how each and every feature in the product should work and how every component should work.
  
   The Outcome of this phase is **High Level Document** and **Low Level Document**.
4. Development Phase
This phase where we start building the software and start writing the code for the product.The outcome from this phase is Source Code Document and the developed product.
5. Testing Phase
When the software is ready, it is sent to the Test team. Once the QA makes sure that the software is error-free, iit goes to the next stage, which is implementation.
The outcome of this phase is the Quality Product and the Testing Artifacts.
6. Deployment & maintenance phase
Deployment is done by the Deployment/Implementation Engineers. Once when the customers start using the developed system then the actual problem will come up and needs to be solved from time to time. Maintenance should be done as per Service Level Agreement.

## Types Of SDLC Models

### Waterfall Model

It is a linear or sequential (non-iterative) design process, used for software development. Its approach is downwards(top to down) like a waterfall. One should move to the next phase only when the preceding phase is reviewed and verified.
Eg: Mechanical Production Company
![image info](./Image/waterfall-model-1.png)

>Monolithic Architechture Followed By WaterFall Model

Most of the time, a software is a combination of different feature sets. In the monolithic architecture, all features of a software reside in a single code base, and deployed as a single file. If any code updates are required, then those updates can’t be accommodated independently. Developer has to use the same code base, make the required code changes and then re-deploy the updated code. So even if a single change is required, the whole code base is touched and re-deployed.

[What is Monolithic Architechture-1](https://www.geeksforgeeks.org/monolithic-architecture/)
[What is Monolithic Architechture-1](https://www.integrate.io/glossary/what-is-monolithic-architecture/)

[What is Microservices Archtechture-1](https://www.atlassian.com/microservices/microservices-architecture)

[What is Microservices Archtechture-2](https://www.edureka.co/blog/microservice-architecture/)

>Advantages

1. It is very simple.
2. Provides a structured way of doing this.
3. Works well for small projects where requirements are well understood beforehand.
4. Time spent early in the software development cycle can reduce cost at latter stages.

>DisAdvantages

1. Can’t change in the middle of the development.
2. Poor resource allocation (tester/deployment eng. Should sit idle until development takes place)
3. Communication Gap can result in disaster.
4. Needs a crystal clear requirement from the client (sometimes the client also wants to change his requirement).
5. No working of software will be available until all phases are finished.
6. It might be very difficult to foresee all the risks which will come in the latter stage of development.

### Agile Model

1. What is Agile?
Software development using Agile Methodology respects our rapidly changing world through adaptive planning, self-organization, and short delivery times. The methodology is flexible, fast, and aims for continuous quality improvements.

Or

However, Agile methodology differs significantly from other methodologies. In English, Agile means ‘ability to move quickly and easily’ and responding swiftly to change – this is a key aspect of Agile software development as well.

Eg: Adobe is working on a project to come up with a competing product for Microsoft Word, that provides all the features provided by Microsoft Word and any other features requested by the marketing team.

![image info](./Image/Agile-Model-1.png)
2. What are the Principles of Agile

![image info](./Image/Agile-Principles-2.png)

  1. Satisfy the Customer
**"our highest priority is to satisfy the customer through early and continuous delivery of valuable software".**
By applying this concept, you will increase your process's agility and respond to changes in a timely fashion. On the other hand, your customers will be happier because they will get the value they are paying for more frequently. Also, they will be able to provide you with feedback early on, so you will be able to decrease the likelihood of making significant changes later in the process.

  2. Welcome Changing Requirement
**"welcome changing requirements, even late in development. Agile processes harness change for the customer's competitive advantage".**
In traditional project management, any late-stage changes are taken with a grain of salt as this usually means scope creep and thus higher costs. In Agile, however, teams aim to embrace uncertainty and acknowledge that even a late change can still bear a lot of value to the end customer. Due to the nature of Agile's iterative process, teams shouldn't have a problem responding to those changes in a timely fashion.

  3. Delivery Working Software Frequently
**"deliver working software frequently, from a couple of weeks to a couple of months, with a preference to the shorter timescale".**
This principle became necessary due to the extensive amounts of documentation that were part of the planning process in software development at the end of the 20th century. Logically, by taking it to heart, you will reduce the time frame for which you are planning and spend more time working on your projects. In other words, your team will be able to plan in a more agile way.

  4. Frequent Interaction With StakeHolders
**"business people and developers must work together daily throughout the project".**
In a knowledge work context that is not explicitly related to software development, you can easily change the word "developers" to "engineers" or "designers" or whatever best suits your situation. The goal is to create a synchronisation between the people who create value and those who plan or sell it. This way, you can make internal collaboration seamless and improve your process performance.

  5. Motivated Individuals
**"build projects around motivated individuals. Give them the environment and support they need, and trust them to get the job done".**
The second sentence of this principle is especially important. If you don't trust your team and keep even the tiniest decisions in your company centralized, you will only hinder your team's engagement. As a result, individuals will never feel a sense of belonging to the purpose that a given project is trying to fulfill, and you won't get the most of their potential.

  6. Face To Face Communications
**"The most efficient and effective method of conveying information to and within a development team is face-to-face conversation."**
Thankfully, with the development of technology, you can interpret this Agile principle from face-to-face to "synchronous" or otherwise direct communication. So as long as you have a way to quickly reach your team and discuss work matters without bouncing back and forward emails for days, you are good to go.

  7. Measure By Working Software
The 7th of the Agile core principles is pretty straight forward. It doesn't matter how many working hours you've invested in your project, how many bugs you managed to fix, or how many lines of code your team has written.
If the result of your work is not the way your customer expects it to be, you are in trouble.

  8. Maintain Constant Phase
**"Agile processes promote sustainable development. The sponsors, developers, and users should be able to maintain a constant pace indefinitely."**
Logically, when putting Agile to practice, your goal is to avoid overburdening and optimize the way you work so you can frequently deliver to the market and respond to change without requiring personal heroics from your team.

  9. Sustain technical Excellence and Good Design
**"continuous attention to technical excellence and good design enhances agility".**
Still, the 9th of the Agile management principles is applicable in every industry. When you maintain operational excellence, you will have less trouble reacting to changes and maintaining agility.

  10. Keep It Simple
**"Simplicity–the art of maximizing the amount of work not done–is essential".**
If you can do something in a simple way, why waste time complicating it? Your customers are not paying for the amount of effort you invest. They are buying a solution to a specific problem that they have. Keep that in mind, when implementing Agile and avoid doing something just for the sake of doing it.
  
  11. Empower Self-Organizing Teams
**"the best architectures, requirements, and designs emerge from self-organizing teams".**
If you have to push your team and "drive them forward", maybe you are not ready for Agile, or you need to make some changes to your leading style.

  12. Reflect and Adjust Continuously
**"At regular intervals, the team reflects on how to become more effective, then tunes and adjusts its behavior accordingly".**
By doing this, you will be able to experiment and improve your performance continuously. If things don't go as you've planned, you can discuss what went wrong and adjust to get back on track.

#### Agile Implementation

![image info](./Image/Agile-Implementation-3.png)

[Deails About Agile](https://www.youtube.com/watch?v=WjwEh15M5Rw&t=9s)

[Scrum Vs Kanban](https://www.youtube.com/watch?v=pxxmSLJj8FQ)

1. Scrum
2. Kanban

Difference B/w Agile Model and WaterFall Model
| S.no.                                                                                                                                                                    |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Purpose                                                                                                                                                                  |
| Agile model                                                                                                                                                              |
| Waterfall model                                                                                                                                                          |
| 1.                                                                                                                                                                       |
| Definition                                                                                                                                                               |
| Agile model follows the incremental approach, where each incremental part is developed through iteration after every timebox.                                            |
| Waterfall model follows a sequential design process.                                                                                                                     |
| 2.                                                                                                                                                                       |
| Progress                                                                                                                                                                 |
| In the agile model, the measurement of progress is in terms of developed and delivered functionalities.                                                                  |
| In the waterfall model, generally the measurement of success is in terms of completed and reviewed artifacts.                                                            |
| 3.                                                                                                                                                                       |
| Nature                                                                                                                                                                   |
| Agile model is flexible as there is a possibility of changing the requirements even after starting the development process.                                              |
| On the other hand, the waterfall model is rigid as it does not allow to modify the requirements once the development process starts.                                     |
| 4.                                                                                                                                                                       |
| Customer interaction                                                                                                                                                     |
| In Agile model, there is a high customer interaction. It is because, after every iteration, an incremental version is deployed to the customer.                          |
| Customer interaction in waterfall model is very less. It is because, in a waterfall model, the product is delivered to the customer after overall development.           |
| 5.                                                                                                                                                                       |
| Team size                                                                                                                                                                |
| It has a small team size. As smaller is the team, the fewer people work on it so that they can move faster.                                                              |
| In the waterfall model, the team may consist more members.                                                                                                               |
| 6.                                                                                                                                                                       |
| Suitability                                                                                                                                                              |
| Agile model is not a suitable model for small projects. The expenses of developing the small projects using agile is more than compared to other models.                 |
| Waterfall model works well in smaller size projects where requirements are easily understandable. But waterfall model is not suitable for developing the large projects. |
| 7.                                                                                                                                                                       |
| Test plan                                                                                                                                                                |
| The test plan is reviewed after each sprint.                                                                                                                             |
| Test plan is reviewed after complete development.                                                                                                                        |
| 8.                                                                                                                                                                       |
| Testing                                                                                                                                                                  |
| Testing team can take part in the requirements change phase without problems.                                                                                            |
| It is difficult for the testing team to initiate any change in needs.                                                                                                    |

Advantages Of Agile Model:

- It is a focused client process. So, it makes sure that the client is continuously involved during every stage.
- Agile teams are extremely motivated and self-organized so it likely to provide a better result from the development projects.
- Agile software development method assures that quality of the development is maintained
- The process is completely based on incremental progress. Therefore, the client and team know exactly what is complete and what is not. This reduces risk in the development process.

Disadvantages Of Agile Method:

- It is not a useful method for small development projects.
- It requires an expert to take important decisions in the meeting.
- Cost of implementing an agile method is little more compared to other development methodologies.
- The project can easily go off track if the project manager is not clear what outcome he/she wants.

### DevOps Model

DevOps speeds delivery of higher quality software by combining and automating the work of software development and IT operations teams.

#### What is DevOps

A compound of development (Dev) and operations (Ops), DevOps is the union of people, process and technology to continually provide value to customers.

DevOps enables formerly siloed roles—development, IT operations, quality engineering and security—to coordinate and collaborate to produce better, more reliable products. By adopting a DevOps culture along with DevOps practices and tools, teams gain the ability to better respond to customer needs, increase confidence in the applications they build and achieve business goals faster.

#### Why we need DevOps

Teams that adopt DevOps culture, practices and tools become high-performing, building better products faster for greater customer satisfaction. This improved collaboration and productivity is also integral to achieving business goals like these:

1. Accelerating time to market
2. Adapting to the market and competition
3. Maintaining system stability and reliability
4. Improving the mean time to recovery

#### How DevOps Works (LifeCycle Of DevOps)?

![image info](./Image/DevOps-Model-1.png)

The DevOps lifecycle (sometimes called the continuous delivery pipeline, when portrayed in a linear fashion) is a series of iterative, automated development processes, or workflows, executed within a larger, automated and iterative development lifecycle designed to optimize the rapid delivery of high-quality software. The name and number of workflows can differ depending on whom you ask, but they typically boil down to these six:

- Planning (or ideation). In this workflow, teams scope out new features and functionality in the next release, drawing from prioritized end-user feedback and case studies, as well as inputs from all internal stakeholders. The goal in the planning stage is to maximize the business value of the product by producing a backlog of features that when delivered produce a desired outcome that has value.

- Development. This is the programming step, where developers test, code, and build new and enhanced features, based on user stories and work items in the backlog. A combination of practices such as test-driven development (TDD), pair programming, and peer code reviews, among others are common. Developers often use their local workstations to perform the “inner loop” of writing and testing code before sending it down the continuous delivery pipeline.

- Integration (or build, or continuous Integration and continuous delivery (CI/CD). As noted above, in this workflow the new code is integrated into the existing code base, then tested and packaged into an executable for deployment. Common automation activities include merging code changes into a “master” copy, checking out that code from a source code repository, and automating the compile, unit test and packaging into an executable. Best practice is to store the output of the CI phase in a binary repository, for the next phase.

- Deployment (usually called continuous deployment). Here the runtime build output (from integration) is deployed to a runtime environment - usually a development environment where runtime tests are executed for quality, compliance and security. If errors or defects are found, developers have a chance to intercept and remediate any problems before any end users see them. There are typically environments for development, test, and production, with each environment requiring progressively “stricter” quality gates. A good practice for deployment to a production environment is typically to deploy first to a subset of end users, and then eventually to all users once stability is established.

- Operations. If getting features delivered to a production environment is characterized as “Day 1”, then once features are running in production “Day 2” operations occur. Monitoring feature performance, behavior, and availability ensures that the features are able to provide value add to end users. Operations ensures that features are running smoothly and that there are no interruptions in service - by making sure the network, storage, platform, compute and security posture are all healthy! If something goes wrong, operations ensures incidents are identified, the proper personnel are alerted, problems are determined, and fixes are applied.

- Learning (sometimes called continuous feedback). This is the gathering of feedback from end users and customers on features, functionality, performance and business value to take back to planning for enhancements and features the next release. This would also include any learning and backlog items from the operations activities, that could empower developers to proactively avoid any past incidents that could happen again in the future. This is the point where the “wraparound” to the Planning phase happens and we “continuously improve!”

Three other important continuous workflows occur between these workflows:

- Continuous testing:  Classical DevOps lifecycles include a discrete “test” phase that occurs between integration and deployment. However, DevOps has advanced such that certain elements of testing can occur in planning (behavior-driven development), development (unit testing, contract testing), integration (static code scans, CVE scans, linting), deployment (smoke testing, penetration testing, configuration testing), operations (chaos testing, compliance testing), and learning (A/B testing). Testing is a powerful form of risk and vulnerability identification and provides an opportunity for IT to accept, mitigate, or remediate risks.

- Security: While waterfall methodologies and agile implementations 'tack on' security workflows after delivery or deployment, DevOps strives to incorporate security from the start (Planning) - when security issues are easiest and least expensive to address - and continuously throughout the rest of the development cycle. This approach to security is referred to as shifting left (which is easier to understand if you look Figure 1). Some organizations have had less success shifting left than others, which led to the rise of DevSecOps (see below).

- Compliance. Regulatory compliance (governance and risk) are also best addressed early and throughout the development lifecycle. Regulated industries are often mandated to provide a certain level of observability, traceability and access of how features are delivered and managed in their runtime operational environment. This requires planning, development, testing, and enforcement of policies in the continuous delivery pipeline and in the runtime environment. Auditability of compliance measures is extremely important for proving compliance to 3rd party auditors.

![image info](./Image/DevOps-2.png)

1. Manage: DevOps closes the loop and incorporates feedback and learnings from the entire lifecycle into your ongoing iteration.

2. Plan: DevOps describes the work that needs to be done, prioritize it, and track its completion.

3. Create: DevOps writes code, proposes changes, and discusses these proposals with coworkers.

4. Verify: DevOps automatically tests code to make sure it works correctly.

5. Package: DevOps stores the software in a state where it can be reused later.

6. Secure: DevOps checks whether the software contains vulnerabilities through static and dynamic tests, fuzz testing, and dependency scanning.

7. Release: DevOps deploys the software to end users.

8. Configure: DevOps manages infrastructure and software platforms.

9. Monitor: DevOps sees the impact of the software is on infrastructure and users. It also provides data to help effectively respond to incidents.

10. Protect: DevOps secures the infrastructure the software is running on by ensuring containers are up to date and locked down.

#### DevOps Culture

It's generally accepted that DevOps methods can't work without a commitment to DevOps culture, which can be summarized as a different organizational and technical approach to software development.

At the organizational level, DevOps requires continuous communication, collaboration and shared responsibility among all software delivery stakeholders - software development and IT operations teams for certain, but also security, compliance, governance, risk and line-of-business teams - to innovate quickly and continually, and to build quality into software from the start.

In most cases the best way to accomplish this is to break down these silos and reorganize them into cross-functional, autonomous DevOps teams that can work on code projects from start to finish - planning to feedback - without making handoffs to, or waiting for approvals from, other teams. When put in the context of agile development, the shared accountability and collaboration are the bedrock of having a shared product focus that has a valuable outcome.

At the technical level, DevOps requires a commitment to automation that keeps projects moving within and between workflows, and to feedback and measurement that enable teams to continually accelerate cycles and improve software quality and performance.

  1. Collaboration, visibility and alignment
  2. Shifts in scope and accountability
  3. Shorter release cycles
  4. Continuous learning

**Benifits:**

The business value of DevOps and the benefits of a DevOps culture lies in the ability to improve the production environment in order to deliver software faster with continuous improvement. You need the ability to anticipate and respond to industry disruptors without delay. This becomes possible within an Agile software development process where teams are empowered to be autonomous and deliver faster, reducing work in progress. Once this occurs, teams are able to respond to demands at the speed of the market.

There are some fundamental concepts that need to be put into action in order for DevOps to function as designed, including the need to:

- Remove institutionalized silos and handoffs that lead to roadblocks and constraints, particularly in instances where the measurements of success for one team is in direct odds with another team’s key performance indicators (KPIs).

- Implement a unified tool chain using a single application that allows multiple teams to share and collaborate. This will enable teams to accelerate delivery and provide fast feedback to one another.

#### Adopting DevOps

Habits are hard to break. Teams entrenched in siloed ways of working can struggle with, or even be resistant to, overhauling team structures to embrace DevOps practices. Some teams may mistakenly believe new tools are sufficient to adopt DevOps. Yet, DevOps is a combination of people, tools, and culture. Everyone on a DevOps team must understand the entire value stream — from ideation, to development, to the end user experience. It requires breaking down silos in order to collaborate throughout the product lifecycle.

Moving from a legacy infrastructure to using Infrastructure as Code (IaC) and microservices can offer faster development and innovation, but the increased operational workload can be challenging. It’s best to build out a strong foundation of automation, configuration management, and continuous delivery practices to help ease the load.

An over-reliance on tools can detract teams from the necessary foundations of DevOps: the team and organization structure. Once a structure is established, the processes and team should come next and the tools should follow.

Adopting DevOps first requires a commitment to evaluating and possibly changing or removing any teams, tools, or processes your organization currently uses. It means building the necessary infrastructure to give teams the autonomy to build, deploy, and manage their products without having to rely too heavily on external teams.

- A DevOps culture is where teams embrace new ways of working that involve greater collaboration and communication. It’s an alignment of people, processes, and tools toward a more unified customer focus. Multidisciplinary teams take accountability for the entire lifecycle of a product.

- Organizations that do DevOps well are places where experimentation and some amount of risk-taking are encouraged. Where thinking outside the box is the norm, and failure is understood to be a natural part of learning and improving.

- Agile methodologies are immensely popular in the software industry since they empower teams to be inherently flexible, well-organized, and capable of responding to change. DevOps is a cultural shift that fosters collaboration between those who build and maintain software. When used together, agile and DevOps result in high efficiency and reliability.

#### Principles Of DevOps

The DevOps methodology comprises four key principles that guide the effectiveness and efficiency of application development and deployment. These principles, listed below, center on the best aspects of modern software development.

   1. Automation of the software development lifecycle
   2. Collaboration and communication
   3. Continuous improvement and minimization of waste
   4. Hyperfocus on user needs with short feedback loops
By adopting these principles, organizations can improve code quality, achieve a faster time to market, and engage in better application planning.

As DevOps has evolved, so has its complexity. This complexity is driven by two factors:

- Organizations are moving from monolithic architectures to microservices architectures. As DevOps matures, organizations need more and more DevOps tools per project.

- The result of more projects and more tools per project has been an exponential increase in the number of project-tool integrations. This necessitated a change in the way organizations adopted DevOps tools.

This evolution took place in following four phases:

Phase 1: Bring Your Own DevOps
In the Bring Your Own DevOps phase, each team selected its own tools. This approach caused problems when teams attempted to work together because they were not familiar with the tools of other teams.

Phase 2: Best-in-class DevOps
To address the challenges of using disparate tools, organizations moved to the second phase, Best-in-class DevOps. In this phase, organizations standardized on the same set of tools, with one preferred tool for each stage of the DevOps lifecycle. It helped teams collaborate with one another, but the problem then became moving software changes through the tools for each stage.

Phase 3: Do-it-yourself DevOps
To remedy this problem, organizations adopted Do-it-yourself (DIY) DevOps, building on top of and between their tools. They performed a lot of custom work to integrate their DevOps point solutions together. However, since these tools were developed independently without integration in mind, they never fit quite right. For many organizations, maintaining DIY DevOps was a significant effort and resulted in higher costs, with engineers maintaining tooling integration rather than working on their core software product.

Phase 4: DevOps Platform
A single-application platform approach improves the team experience and business efficiency. GitLab, The DevOps Platform, replaces DIY DevOps, allowing visibility throughout and control over all stages of the DevOps lifecycle.

By empowering all teams – Software, Operations, IT, Security, and Business – to collaboratively plan, build, secure, and deploy software across an end-to-end unified system, GitLab represents a fundamental step-change in realizing the full potential of DevOps. The DevOps Platform is a single application powered by a cohesive user interface, agnostic of self-managed or SaaS deployment. It is built on a single codebase with a unified data store, that allows organizations to resolve the inefficiencies and vulnerabilities of an unreliable DIY toolchain.

As we look ahead to software-led organizations becoming even more distributed and agile, every company will need a DevOps platform to modernize software development and delivery. By making it easier and trusted to adopt the next generation of cloud-native technologies – from microservices to serverless and eventually edge architecture – all companies will be empowered to ship software faster, at maximum efficiency, with security embedded across their end-to-end software supply chain.

#### Framwork In DevOps

[Four Frameworks in DevOps](https://www.atlassian.com/devops/frameworks)

**DevOps is associated with Agile software development because Agile practitioners promoted DevOps as a way to extend the methodology into production. The approach has even been labeled a counterculture to the IT service management practices championed in ITIL. DevOps does not have an official framework.
To hone their strategies, organizations should understand the related contexts of DevOps, Agile and Waterfall development, site reliability engineering (SRE) and SysOps, and even the variations within DevOps.**

#### DevOps and Cloud-Native Development

Cloud-native is an approach to building applications that leverage foundational cloud computing technologies. The goal of cloud-native is to enable a consistent and optimal application development, deployment, management and performance across public, private and multicloud environments.

Today, cloud-native applications are typically

- Built using microservices - loosely-coupled, independently deployable components that have their own self-contained stack, and communicate with each other via REST APIs, event streaming or message brokers.

- Deployed in containers - executable units of code that contain all the code, runtimes and operating system dependencies required to run the application. (For most organizations, 'containers' is synonymous with Docker containers, but other container types exist.)

- Operated (at scale) using Kubernetes, an open-source container orchestration platform for scheduling and automating the deployment, management and scaling of containerized applications.

By packaging and permanently fixing all OS dependencies, containers enable rapid CI/CD and deployment cycles, because all integration, testing and deployment occurs in the same environment. And Kubernetes orchestration performs the same continuous configuration tasks for containerized applications as Ansible, Puppet and Chef perform for non-containerized applications.

Most leading cloud computing providers - including AWS, Google, Microsoft Azure, and IBM Cloud - offer some sort of managed DevOps pipeline solution.

**Example:**

For example, developing and updating microservices - that is, the iterative delivery of small units of code to a small code base - is a perfect fit for DevOps rapid release and management cycles. And it would be difficult to deal with the complexity of a microservices architecture without DevOps deployment and operation. A recent IBM survey of developers and IT executives found that 78% of current microservices users expect to increase the time, money and effort they’ve invested in the architecture, and 56% of non-users are likely to adopt microservices within the next two years. To explore some of the specific microservices benefits and challenges they cited, use the interactive tool below:

#### DevSecOps Detailed

[DevSecOps-1](https://www.ibm.com/cloud/learn/devsecops)

[DevSecOps-2](https://www.redhat.com/en/topics/devops/what-is-devsecops)

#### SRE

Site reliability engineering (SRE) uses software engineering techniques to automate IT operations tasks - e.g. production system management, change management, incident response, even emergency response - that might otherwise be performed manually by systems administrators. SRE seeks to transform the classical system administrator into an engineer.

The ultimate goal of SRE is similar to the goal of DevOps, but more specific: SRE aims to balance an organization's desire for rapid application development with its need to meet performance and availability levels specified in service level agreements (SLAs) with customers and end-users.

Site reliability engineers achieve this balance by determining an acceptable level of operational risk caused by applications - called an 'error budget' - and by automating operations to meet that level.

On a cross-functional DevOps team, SRE can serve as a bridge between development and operations, providing the metrics and automation the team needs to push code changes and new features through the DevOps pipeline as quickly as possible, without 'breaking' the terms of the organizations SLAs.

[SRE-1](https://www.ibm.com/cloud/learn/site-reliability-engineering)
[SRE-2](https://www.redhat.com/en/topics/devops/what-is-sre)
[SRE-3](https://www.dynatrace.com/news/blog/what-is-site-reliability-engineering/#:~:text=Site%20reliability%20engineering%20%28SRE%29%20is%20the%20practice%20of,organizations%20create%20highly%20reliable%20and%20scalable%20software%20systems.)

#### Diffrence B/W Waterfall vs Agile vs DevOps

![Image Info](Image/DevOps-3.png)

| **The Basis Of Comparison** |                          **Agile**                           |                          **DevOps**                          |
| :-------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|        **Intention**        | A development and management approach for managing complex projects. | This is an end-to-end management process related to engineering. |
|          **Task**           |        The agile process focuses on constant changes.        |       DevOps focuses on constant testing and delivery.       |
|        **Practices**        | Some of the best practices adopted in Agile are listed below –   1. Building a backlog 2. Sprint development 3. Daily Scrums | DevOps also have some best practices that ease the process –   1. Respond to changes quickly 2. Collaborate directly with users and incorporate their feedback 3. Focus on technical excellence. |
|   **Speed of Production**   | Agile pertains largely to the way development is carried of; any department of the company can be agile in its practices. This can be achieved through training. | DevOps focuses more on software deployment choosing the most reliable and safest route. |
|      **Team Skillset**      | All the team members working in an agile practice have a wide variety of similar skill sets. This is one of the advantages of having such a team because, in the time of need, any of the team members can lend assistance rather than waiting for the team leads or any specialist interference. | DevOps has a different approach and is quite effective; most of the time, it follows “Divide and Conquer”. Work divided among the development and operation teams. |
|        **Team Size**        | Agile believes in “smaller and concise”. The smaller the team better it would be to deliver with fewer complexities. | DevOps, on the other hand, believes that “bigger is better”. |
|       **Scheduling**        | Since Agile teams are short, a predetermined amount of time is there, which are sprints. Hardy, it happens that a sprint has lasted longer than a month but often a week long. | DevOps, on the other hand, prioritizes reliabilities. It is because of this behavior that they can focus on a long-term schedule that minimizes business disturbances. |
|      **Shortcomings**       | In Agile, the gap between these teams is bridged in daily scrum calls where all the rollbacks are discussed and resolved with agile-scrum methodologies. | DevOps helps to bridge the line between several cross-functional teams (Development, QA, Monitoring, Deployment, Management etc.) by simplifying the process. |
|       **Advantages**        | *Customer satisfaction is there as there is the short and continuous delivery of small chunks of working applications.* People and interactions are preferred over processes and tools. *Working software is delivered at frequent timings.* Daily interaction among business people and developers. *Late changes are welcomed.*Agile prefers face to face communication over any other medium. | *Faster solutions* Improved performances *Increased efficiency* Continuous improvement *Improved customer experience.* Faster ROI * Reduced failures and rollbacks. |
|      **Disadvantages**      | *If there are some big projects, there can be issues in handling the efforts required at the initial stages of development.* The project can get out of the track if the client or the representatives are not clear with their needs. * No place for a newbie as the Agile works is based on the level of expertise. So there are lesser chances for newcomers. | * Infrastructure changes *No control over the evolution of the products that the services depend on.* A Complexity level, in some instances, has a steep curve. These can be in terms of cost, performance, deployment, and Operations. |

[Head to head Comparision b/w agile and devops](https://www.educba.com/agile-vs-devops/)

![Image Info](Image/DevOps-4.png)

How does DevOps relate to both waterfall and agile methodologies?

- DevOps leverages and enhances the beneficial aspects of agile
- It brings your development and operations teams together
- DevOps facilitates automation to speed up procedures and eliminate human errors
- It can handle complex projects at lower risks
- Through constant feedback and removal of siloed work practices, DevOps solves problems at faster intervals
- It makes continuous delivery possible by providing customers with quick but effective small updates

How does DevOps relate to the software development lifecycle?

DevOps is not limited to software developers who write code, operations teams who handle service quality, or IT departments who deal with the IT operations.

It also impacts other areas of your organization, such as project management teams.

In fact, an effective and seamless project management practice is necessary to keep software projects on schedule and to make improvements whenever needed.

So, how does DevOps affect the software development lifecycle?

1. It applies agile principles to project management.
2. It lends itself to using microservices.
3. It results in an evolution in project planning.
4. It encourages the usage of the same tools across teams.
5. It accelerates the development of a Minimum Viable Product (MVP).

#### Advantages and DisAdvantages

[In-Short-Real-Time-DevOps-Issues](https://www.orientsoftware.com/blog/advantages-and-disadvantages-of-devops/)

Advantages:

1. events, documented management processes and detailed reports are easy to track;
2. developers have more control over the environment, giving the infrastructure a more applied understanding of the product and its operation processes;
3. a significant reduction in time to market through a seamless development and deployment cycle;
4. improved customer satisfaction;
5. improved product quality and reliability;
6. increased productivity and efficiency;
7. rapid response and high speed of experiments;
8. expanding developer competencies and responsibilities – programmers are involved in server setup and bug finding, writing automated tests, smoothing out possible infrastructure vulnerabilities in the code. This reduces the number of errors during application deployment by about 5 times.

DisAdvantages:

1. Cycle incompleteness – important stages of software life, such as requirements development and analysis, as well as architecture design, remain overboard the Devops processes. It is also possible to miss manual testing, which may be critical in some cases. For example, if developers have not analyzed the requirements properly enough and tested the product from the point of view of “ideal” code rather than from the point of view of users, the result may be inconvenient to use.
2. Insufficient professionalism of the participants, who understand everything (development, testing, deployment, support), but superficially.
3. High management load – if developers and operators have no common goals, it is the fault of managers who did not organize effective interaction between teams of different specialists. To solve this problem, a new manager evaluation system based on feedback from subordinates is needed.

DevOps-As-Service Advantages and Disadvantages:

Advantages of DevOps-as-a-Service

For this reason, ordering DevOps-as-a-Service is a good choice:

1. You get immediate access to experienced DevOps engineers who can bring their expertise to your project from day one.

2. Your DevOps partner works on a variety of projects for several companies in different industries. This gives the teams invaluable R&D experience, so they can immediately tell which approaches and solutions work and which don't. This helps to save time and money while avoiding costly errors in your project.

3. A dedicated DevOps team provides developer documentation and supports your internal IT department in mastering your new DevOps tools and systems. Once again, you need to learn from the mistakes of others rather than make your own.

Disadvantages of DevOps-as-a-Service

However, this approach is not a panacea for several reasons:

1. Managing your IT infrastructure is one of the most resource-intensive areas of your business. Therefore, you need to hire a reliable partner to ensure the uninterrupted availability of your products/services.

2. In order not to reduce the security due to outsourcing, a careful assessment is imperative to ensure the security of operations.

3. Your internal IT department should have a certain level of skills and understanding of the integration between different software modules, cloud systems and custom DevOps solutions delivered by your DevOps partner. Otherwise the IT department will not be able to support the system in production.

4. Therefore, some additional training will be required. The only remedy is a long-term partnership with a DevOps service provider so that they take over all aspects of your IT operations for you.

DevOps-Methoolgy Advantages and Disadvantages:

1. It has high productivity.
2. Product release and time to market are both accelerated.
3. Process effectiveness.
4. Production cycles have been shortened.
5. Improved operational support.
6. Employees who are engaged and motivated.
7. Within the team, there is a clear product vision.
8. Deployment success rates have increased.
9. Flexibility and support have been increased.
10. Product failure is less likely.
11. Cross-skilling and self-improvement are important.
12. Improved management of the customer experience.
13. Increased the success rate of deployments.
14. Product quality has improved.
15. Increased team efficiency.

Disadvantages of DevOps-Methodologies:

1. Requires a proper mindset throughout the organization.
2. Outsourcing DevOps operations reduced business security.
3. Dealing with the legacy system is difficult.
4. Problems with the number of tools and switching between them.
5. Transitional difficulties
6. Security training for CI/CD is a separate matter.
7. Finding the right pool of DevOps expertise is difficult.

#### Roles and Responsibilies

The primary roles and responsibilities of a DevOps Engineer are:

[R-A-R-1](https://optymize.io/blog/devops-engineer-roles-responsibilities-and-benefits/)

[R-A-R-2](https://staragile.com/blog/roles-and-responsibilities-of-devops-engineer)

[R-A-R-3](https://mindmajix.com/role-of-a-devops-engineer)

[R-A-R-4](https://www.dotnettricks.com/learn/devops/roles-and-responsibilities-of-a-devops-engineer)

#### DevOps Tools

- Project planning
  - Jira
  - GitLab
  - GitHub
  - BitBucket
  - Confluence/WIKI

- Continuous Integration and Deployment Tools
  - **[Jenkins](https://jenkins.io/)** [Open Source]
  - **[Github Actions](https://github.com/marketplace?category=continuous-integration&type=actions)** [Free & Enterprise]
  - **[Gitlab CI](https://about.gitlab.com/stages-devops-lifecycle/continuous-integration/)** [Free & Enterprise]
  - **[UrbanCode Deployment](https://www.ibm.com/cloud/urbancode/deploy)**
  - Agro CD
  - Tekton

- Infrastructure & Configuration Management Tools
  
  Infrastructure Management Tool:
  - Terraform ❎
  
  VM/Container Image Management & Configuration:
  - Docker
  - Helm
  - Crio
  - Podman
  
  Configuration Management:
  - Ansible

  Secret Management:
  - Hashicorp Vault
  
  Config/Service Discovery Tools
  - Consul
  - ETCD

- Container Clustering/Orchestration Tools
  
  Contianer Orchestration:
  - Kubernetes
  - Docker Swarm
  - OpenShift

  Container Security:
  K8s Compliance Tools:
  Service Mesh Tools:
  - Istio

- App/Infrastructure Logging/Monitoring/Visualization Tools
  
  Logging:
  - ELK / EFK
  - Spulnk
  
  Monitoring:
  - Prometheus
  - Nagois
  - Zabbix
  - Dynatrace
  - Data Dog

  Visualization:
  - Grafana
  - Kibana

- Collaboration
  - Slack
  - Google
  - WebEx
  - Teams
  - Gmail/Outlook

- Source Code Management
  - **[Github](https://github.com/)** [Free & Paid]
  - **[Bitbucket](https://bitbucket.org/product)** [Free & Paid]
  - **[Gitlab](https://about.gitlab.com/)** [Free & Paid]
  - [**AWS CodeCommit**](https://aws.amazon.com/codecommit/) [Free & Paid]
  - [**Azure Repos**](https://azure.microsoft.com/en-us/services/devops/repos/) [Free & Paid]
  - [**Google Cloud Source Repositories**](https://cloud.google.com/source-repositories) [Free & Paid]

- Developer Productivity Tools
  
  Environment Setup:
  - Vagrant [Open Source]
  - Docker [Open Source]
  
  API Tools:
  - Postman
  - SoapUI
  
  IDE’s:
  - VS Code
  - Eclips
  - Notepad ++
  
- DevOps Build Tools
  - IBM ACE
  - IBM MQ
  - JAVA
  - Python
  - NodeJS
  - Go Lang.
  - DP and APIC
  - Gradle

- Artifact Management Tools for DevOps
  - Nexus
  - JFrog
  - NPM

- Test Automation/Performance Testing Tools
  - Selenium
  - JUnit

> Other SDLC Models: ~~Spiral~~, ~~V model~~, ~~Prototype~~

Environments:

DEV: A development environment in software and web development is a workspace for developers to make changes without breaking anything in a live environment. The development environment is often seen as a developer's “everything-goes” workspace.

QA:

1. UAT/SIT: UAT and SIT testing are the two different levels of testing in the application testing phase of QA. UAT stands for User Acceptance Testing and SIT stands for System Integration Testing. Here we compare UAT vs. SIT against one another. UAT: User Acceptance Testing Best Practices
2. Stress: Stress Testing is a type of software testing that verifies stability & reliability of software application. The goal of Stress testing is measuring software on its robustness and error handling capabilities under extremely heavy load conditions and ensuring that software doesn’t crash under crunch situations. It even tests beyond normal operating points and evaluates how software works under extreme conditions.

SandBox: a sandbox environment is an isolated virtual machine in which potentially unsafe software code can execute without affecting network resources or local applications. Cybersecurity researchers use sandboxes to run suspicious code from unknown attachments and URLs and observe its behavior.

PROD: Production is the final environment in your software development process. It is the work that it ready to be publicly available, and only the most thoroughly tested code should end up here. While most people associate the production environment with the product being live, this is not necessarily the case.

--------------------------------------

## **kubernetes-Beginners**

"CKA Certification Should be my first Certification"

### Kubernetes Basics

Before knowing k8s, we need to know the containers and before knowing containers we need to have knowledge on difference b/w the legacy system and container based systems

And Here we are talking about containers. So, we are taking the most popular tool called **Docker**.

### Kubernetes Overview

#### Container Orchestration

![Image Info](Image/Kuberetes-1.png)

So we learned about containers and we now have our application packaged into a docker container. But what next? How do you run it in production? What if your application relies on other containers such as database or messaging services or other backend services? What if the number of users increase and you need to scale your application? You would also like to scale down when the load decreases.

To enable these functionalities you need an underlying platform with a set of resources. The platform needs to orchestrate the connectivity between the containers and automatically scale up or down based on the load. This whole process of automatically deploying and managing containers is known as Container Orchestration.

Kubernetes is thus a container orchestration technology. There are multiple such technologies available today
– Docker has its own tool called Docker Swarm.

- Kubernetes from Google and Mesos from Apache. While Docker Swarm is really easy to set up and get started, it lacks some of the advanced auto scaling features required for complex applications.

- Mesos on the other hand is quite difficult to set up and get started, but supports many advanced features.

- Kubernetes - arguably the most popular of it all – is a bit difficult to setup and get started but provides a lot of options to customise deployments and supports deployment of complex architectures. Kubernetes is now supported on all public cloud service providers like GCP, Azure and AWS and the kubernetes project is one of the top ranked projects in Github.

#### Kubernetes Advantages

![Image Info](Image/Kuberetes-2.png)

There are various advantages of container orchestration. Your application is now highly available as hardware failures do not bring your application down because you have multiple instances of your application running on different nodes. The user traffic is load balanced across the various containers. When demand increases, deploy more instances of the application seamlessly and within a matter of seconds and we have the ability to do that at a service level. When we run out of hardware resources, scale the number of nodes up/down without having to take down the application. And do all of these easily with a set of declarative object configuration files.

And THAT IS Kubernetes. It is a container Orchestration technology used to orchestrate the deployment and management of 100s and 1000s of containers in a clustered environment. Don’t worry if you didn’t get all of what was just said, in the upcoming lectures we will take a deeper look at the architecture and various concepts surrounding kubernetes.

### Kubernetes Architechture

Before we head into setting up a kubernetes cluster, it is important to understand some of the basic concepts. This is to make sense of the terms that we will come across while setting up a kubernetes cluster.

![Image Info](Image/Kuberetes-3.png)

Let us start with Nodes. A node is a machine – physical or virtual – on which kubernetes is installed. A node is a worker machine and this is where containers will be launched by kubernetes.

It was also known as Minions in the past. So you might hear these terms used interchangeably.

But what if the node on which our application is running fails? Well, obviously our application goes down. So you need to have more than one node.

-> Cluster

![Image Info](Image/Kuberetes-4.png)

A cluster is a set of nodes grouped together. This way even if one node fails you have your application still accessible from the other nodes. Moreover having multiple nodes helps in sharing load as well.

-> Master

![Image Info](Image/Kuberetes-5.png)

Now we have a cluster, but who is responsible for managing the cluster? Where is the information about the members of the cluster stored? How are the nodes monitored? When a node fails how do you move the workload of the failed node to another worker node? That’s where the Master comes in. The master is another node with Kubernetes installed in it, and is configured as a Master. The master watches over the nodes in the cluster and is responsible for the actual orchestration of containers on the worker nodes.

-> Components

When you install Kubernetes on a System, you are actually installing the following components.

- An API Server,
The API server acts as the front-end for kubernetes. The users, management devices, Command line interfaces all talk to the API server to interact with the kubernetes cluster.

- An ETCD service,
Next is the ETCD key store. ETCD is a distributed, reliable key-value store used by kubernetes to store all data used to manage the cluster. Think of it this way, when you have multiple nodes and multiple masters in your cluster, etcd stores all that information on all the nodes in the cluster in a distributed manner. ETCD is responsible for implementing locks within the cluster to ensure there are no conflicts between the Masters.

- A kubelet service,
finally kubelet is the agent that runs on each node in the cluster. The agent is responsible for making sure that the containers are running on the nodes as expected.

- A Container Runtime,
The container runtime is the underlying software that is used to run containers. In our case it happens to be Docker.

- Schedulers,
The scheduler is responsible for distributing work or containers across multiple nodes. It looks for newly created containers and assigns them to Nodes.

- Controllers
The controllers are the brain behind orchestration. They are responsible for noticing and responding when nodes, containers or endpoints goes down. The controllers makes decisions to bring up new containers in such cases.

-> Master Vs Worker

![Image Info](Image/Kuberetes-6.png)

So far we saw two types of servers – Master and Worker and a set of components that make up Kubernetes. But how are these components distributed across different types of servers. In other words, how does one server become a master and the other slave?

The worker node (or minion) as it is also known, is where the containers are hosted. For example Docker containers, and to run docker containers on a system, we need a container runtime installed. And that’s where the container runtime falls. In this case it happens to be Docker. This doesn’t HAVE to be docker, there are other container runtime alternatives available such as Rocket or CRIO. But throughout this course we are going to use Docker as our container runtime.

The master server has the kube-apiserver and that is what makes it a master.

Similarly the worker nodes have the kubelet agent that is responsible for interacting with the master to provide health information of the worker node and carry out actions requested by the master on the worker nodes.

All the information gathered are stored in a key-value store on the Master. The key value store is based on the popular etcd framework as we just discussed.

The master also has the controller manager and the scheduler.

There are other components as well, but we will stop there for now. The reason we went through this is to understand what components constitute the master and worker nodes. This will help us install and configure the right components on different systems when we setup our infrastructure.

And finally, we also need to learn a little bit about ONE of the command line utilities known as the **kube command line tool** or **kubectl** or **kube control** as it is also called. The kube control tool is used to deploy and manage applications on a kubernetes cluster, to get cluster information, get the status of nodes in the cluster and many other things.

- The kubectl run command is used to deploy an application on the cluster.
```sh kubectl run hello-minikube```

- The kubectl cluster-info command is used to view information about the cluster.
```sh kubectl cluster-info```

- The kubectl get pod command is used to list all the nodes part of the cluster.
```sh kubectl get nodes```

That’s all we need to know for now and we will keep learning more commands throughout this course. We will explore more commands with kubectl when we learn the associated concepts. For now just remember the run, cluster-info and get nodes commands and that will help us get through the first few labs.

### SetUp Kubernetes

![Image Info](Image/Kuberetes-7.png)

There are lots of ways to set up Kubernetes. We can set it up ourselves locally on our laptops or virtual machines using solutions like Minikube and Kubeadmin. Minikube is a tool used to set up a single instance of Kubernetes in an All-in-one setup and kubeadm is a tool used to configure kubernetes in a multi-node setup. We will look more into that in a bit.

There are also hosted solutions available for setting up kubernetes in a cloud environment such as GCP and AWS. We will also have some demos around those.

And finally if you don’t have the resources or if you don’t want to go through the hassle of setting it all up yourself, and you simply want to get your hands on a kubernetes cluster instantly to play with, checkout play-with-k8s.com . I also have a demo on this.

So feel free to choose the one that is right for you. You need not go through all the demos, pick the ones that best suit your needs based on your time and resources.

-> Minikube Intallation

![Image Info](Image/Kuberetes-8.png)

We will start with Minikube which is the easiest way to get started with Kubernetes on a local system. If Minikube is not of interest to you, now would be a good time to skip this lecture. Before we head into the demo it’s good to understand how it works. Earlier we talked about the different components of Kubernetes that make up a Master and worker nodes such as the api server, etcd key value store, controllers and scheduler on the master and kubelets and container runtime on the worker nodes. It would take a lot of time and effort to setup and install all of these various components on different systems individually by ourlselves.

Minikube bundles all of these different components into a single image providing us a pre-configured single node kubernetes cluster so we can get started in a matter of minutes.

The whole bundle is packaged into an ISO image and is available online for download.

Now you don’t HAVE to download it yourself. Minikube provides an executable command line utility that will AUTOMATICALLY download the ISO and deploy it in a virtualization platform such as Oracle Virtualbox or Vmware fusion. So you must have a Hypervisor installed on your system. For windows you could use Virtualbox or Hyper-V and for Linux use Virtualbox or KVM.

And finally to interact with the kubernetes cluster, you must have the kubectl kubernetes command line tool also installed on your machine. So you need 3 things to get this working, you must have a **hypervisor** installed, **kubectl** installed and **minikube** executable installed on your system.

`Install MiniKube: https://kubernetes.io/docs/tasks/tools/install-minikube/`

`VirtualBox: https://www.virtualbox.org/wiki/Downloads`

`MiniKube Download page for  Windows: https://github.com/kubernetes/minikube/releases`

While using Minikube with  Virtualization technologies, specify the --vm-driver option like this:
```sh $ minikube start --vm-driver=<driver_name>```

`More about it here: https://kubernetes.io/docs/setup/learning-environment/minikube/#specifying-the-vm-driver`

-> Kubeadm Installation

![Image Info](Image/Kuberetes-9.png)

With the minikube utility you could only setup a single node kubernetes cluster. The kubeadmin tool helps us setup a multi node cluster with master and workers on separate machines. Installing all of these various components individually on different nodes and modifying the configuration files to make it work is a tedious task. Kubeadmin tool helps us in doing all of that very easily.

Let’s go through the steps:

![Image Info](Image/Kuberetes-10.png)

1. First, you must have multiple systems or virtual machines created for configuring a cluster. We will see how to setup up your laptop to do just that if you are not familiar with it. Once the systems are created, designate one as master and others as worker nodes.

2. The next step is to install a container runtime on the hosts. We will be using Docker, so we must install Docker on all the nodes.

3. The next step is to install kubeadmin tool on all the nodes. The kubeadmin tool helps us bootstrap the kubernetes solution by installing and configuring all the required components in the right nodes.

4. The next step is to initialize the Master server. During this process all the required components are installed and configured on the master server.That way we can start the cluster level configurations from the master server.

5. Once the master is initialized and before joining the worker nodes to the master, we must ensure that the network pre-requisites are met. A normal network connectivity between the systems is not SUFFICIENT for this. Kubernetes requires a special network between the master and worker nodes which is called as a POD network. We will learn more about this network in the networking section later in this course. For now we will simply follow the instructions available to get this installed and setup in our environment.

6. The last step is to join the worker nodes to the master node. We are then all set to launch our application in the kubernetes environment.

### Kubernetes Concepts - Pods, ReplicaSets, Deployments

-> PODS

![Image Info](Image/Kuberetes-11.png)

Before we head into understanding PODs, we would like to assume that the following have been setup already. At this point, we assume that the application is already developed and built into Docker Images and it is available on a Docker repository like Docker hub, so kubernetes can pull it down. We also assume that the Kubernetes cluster has already been set up and is working. This could be a single-node setup or a multi-node setup, doesn’t matter. All the services need to be in a running state.

As we discussed before, with kubernetes our ultimate aim is to deploy our application in the form of containers on a set of machines that are configured as worker nodes in a cluster. However, kubernetes does not deploy containers directly on the worker nodes. The containers are encapsulated into a Kubernetes object known as PODs. A POD is a single instance of an application. A POD is the smallest object, that you can create in kubernetes.

![Image Info](Image/Kuberetes-12.png)

Here we see the simplest of simplest cases where you have a single node kubernetes cluster with a single instance of your application running in a single docker container encapsulated in a POD. What if the number of users accessing your application increases and you need to scale your application? You need to add additional instances of your web application to share the load. Now, where would you spin up additional instances? Do we bring up a new container instance within the same POD? No! We create a new POD altogether with a new instance of the same application. As you can see we now have two instances of our web application running on two separate PODs on the same kubernetes system or node.

What if the user base FURTHER increases and your current node has no sufficient capacity? Well THEN you can always deploy additional PODs on a new node in the cluster. You will have a new node added to the cluster to expand the cluster’s physical capacity. SO, what I am trying to illustrate in this slide is that PODs usually have a one-to-one relationship with containers running your application. To scale UP you create new PODs and to scale down you delete PODs. You do not add additional containers to an existing POD to scale your application. Also, if you are wondering how we implement all of this and how we achieve load balancing between containers etc, we will get into all of that in a later lecture. For now we are ONLY trying to understand the basic concepts.

-> Multi Container Pod

![Image Info](Image/Kuberetes-13.png)

Now we just said that PODs usually have a one-to-one relationship with the containers, but, are we restricted to having a single container in a single POD? No! A single POD CAN have multiple containers, except for the fact that they are usually not multiple containers of the same kind. As we discussed in the previous slide, if our intention was to scale our application, then we would need to create additional PODs. But sometimes you might have a scenario where you have a helper container, that might be doing some kind of supporting task for our web application such as processing a user entered data, processing a file uploaded by the user etc. and you want these helper containers to live alongside your application container. In that case, you CAN have both of these containers part of the same POD, so that when a new application container is created, the helper is also created and when it dies the helper also dies since they are part of the same POD. The two containers can also communicate with each other directly by referring to each other as ‘localhost’ since they share the same network namespace. Plus they can easily share the same storage space as well.

--> More About Pod

![Image Info](Image/Kuberetes-14.png)

If you still have doubts in this topic (I would understand if you did because I did the first time I learned these concepts), we could take another shot at understanding PODs from a different angle. Let’s, for a moment, keep kubernetes out of our discussion and talk about simple docker containers. Let’s assume we were developing a process or a script to deploy our application on a docker host. Then we would first simply deploy our application using a simple docker run python-app command and the application runs fine and our users are able to access it. When the load increases we deploy more instances of our application by running the docker run commands many more times. This works fine and we are all happy. Now, sometime in the future our application is further developed, undergoes architectural changes and grows and gets complex. We now have new helper containers that helps our web applications by processing or fetching data from elsewhere.

These helper containers maintain a one-to-one relationship with our application container and thus, needs to communicate with the application containers directly and access data from those containers. For this we need to maintain a map of what app and helper containers are connected to each other, we would need to establish network connectivity between these containers ourselves using links and custom networks, we would need to create shareable volumes and share it among the containers and maintain a map of that as well. And most importantly we would need to monitor the state of the application container and when it dies, manually kill the helper container as well as its no longer required. When a new container is deployed we would need to deploy the new helper container as well.

With PODs, kubernetes does all of this for us automatically. We just need to define what containers a POD consists of and the containers in a POD by default will have access to the same storage, the same network namespace, and the same fate as if they will be created together and destroyed together.

Even if our application didn’t happen to be so complex and we could live with a single container, kubernetes still requires you to create PODs. But this is good in the long run as your application is now equipped for architectural changes and scale in the future.

Let us now look at how to deploy PODs:

- Earlier we learned about the kubectl run command. What this command really does is it deploys a docker container by creating a POD.
- So it first creates a POD automatically and deploys an instance of the nginx docker image. But where does it get the application image from?
- For that you need to specify the image name using the –-image parameter.
- The application image, in this case the nginx image, is downloaded from the docker hub repository.
- Docker hub as we discussed is a public repository where the latest docker images of various applications are stored.
- You could configure kubernetes to pull the image from the public docker hub or a private repository within the organisation.

Now that we have a POD created, how do we see the list of PODs available? The kubectl get PODs command helps us see the list of pods in our cluster. In this case we see the pod is in a ContainerCreating state and soon changes to a Running state when it is actually running.

Also remember that we haven’t really talked about the concepts on how a user can access the nginx web server. And so in the current state we haven’t made the web server accessible to external users. You can access it internally from the Node through. For now we will just see how to deploy a POD and in a later lecture once we learn about networking and services we will get to know how to make this service accessible to end users.

The smallest unit you can create in Kubernetes object model is:

- **Pod**

-> YAML In Kubernetes

![Image Info](Image/Kuberetes-15.png)

In the previous lecture we learned about YAML files in general. Now we will learn how to develop YAML files specifically for Kubernetes. Kubernetes uses YAML files as input for the creation of objects such as **PODs, Replicas, Deployments, Services** etc. All of these follow a similar structure. A kubernetes definition file always contains 4 top level fields. The **apiVersion, kind, metadata and spec**. These are top level or root level properties. Think of them as siblings, children of the same parent. These are all REQUIRED fields, so you MUST have them in your configuration file.

- The first one is the apiVersion. This is the version of the kubernetes API we’re using to create the object. Depending on what we are trying to create we must use the RIGHT apiVersion. For now since we are working on PODs, we will set the apiVersion as v1. Few other possible values for this field are apps/v1beta1, extensions/v1beta1 etc. We will see what these are for later in this course.

- Next is the kind. The kind refers to the type of object we are trying to create, which in this case happens to be a POD. So we will set it as a Pod. Some other possible values here could be ReplicaSet or Deployment or Service, which is what you see in the kind field in the table on the right.

- The next is metadata. The metadata is data about the object like its name, labels etc. As you can see, unlike the first two where you specified a string value, this is in the form of a dictionary.
  - So everything under metadata is intended to the right a little bit and so names and labels are children of metadata. The number of spaces before the two properties name and labels doesn’t matter, but they should be the same as they are siblings.
  - In this case labels have more spaces on the left than name and so it is now a child of the name property instead of a sibling. Also the two properties must have MORE spaces than its parent, which is metadata, so that its intended to the right a little bit.
  - In this case all 3 have the same number of spaces before them and so they are all siblings, which is not correct. Under metadata, the name is a string value
  - so you can name your POD myapp-pod
  - and the label is a dictionary. So labels is a dictionary within the metadata dictionary. And it can have any key and value pairs as you wish.
  - For now I have added a label app with the value myapp. Similarly you could add other labels as you see fit which will help you identify these objects at a later point in time. Say for example there are 100s of PODs running a front-end application, and 100’s of them running a backend application or a database, it will be DIFFICULT for you to group these PODs once they are deployed.
  - If you label them now as front-end, back-end or database, you will be able to filter the PODs based on this label at a later point in time.
  - It’s IMPORTANT to note that under metadata, you can only specify name or labels or anything else that kubernetes expects to be under metadata.
  - You CANNOT add any other property as you wish under this. However, under labels you CAN have any kind of key or value pairs as you see fit.
  - So it's IMPORTANT to understand what each of these parameters expect.
  - So far we have only mentioned the type and name of the object we need to create which happens to be a POD with the name myapp-pod, but we haven’t really specified the container or image we need in the pod.
  - The last section in the configuration file is the specification which is written as spec. Depending on the object we are going to create, this is where we provide additional information to kubernetes pertaining to that object.
  - This is going to be different for different objects, so its important to understand or refer to the documentation section to get the right format for each. Since we are only creating a pod with a single container in it, it is easy.

- Spec is a dictionary so add a property under it called containers, which is a list or an array. The reason this property is a list is because the PODs can have multiple containers within them as we learned in the lecture earlier. In this case though, we will only add a single item in the list, since we plan to have only a single container in the POD. The item in the list is a dictionary, so add a name and image property. The value for the image is nginx.

Once the file is created, run the command kubectl create -f followed by the file name which is pod-definition.yml and kubernetes creates the pod.

```sh kubectl create -f pod-definition.yml```

So to summarise, remember the 4 top level properties. apiVersion, kind, metadata and spec. Then start by adding values to those depending on the object you are creating.

Once we create the pod, how do you see it? Use the kubectl get pods command to see a list of pods available. In this case it's just one. To see detailed information about the pod run the kubectl describe pod command. This will tell you information about the POD, when it was created, what labels are assigned to it, what docker containers are part of it and the events associated with that POD.

[POD YAML's and Practice Sets are Here](Kubernetes-Beginners/README.md/#pod-yaml)

Commands:

```sh $ kubectl run <name of pod> --image=<name of the image from registry>```

```sh $ kubectl run tomcat --image=tomcat:9```

```sh kubectl create -f pod-definition.yml```

-> **Controllers**

High Availability

So what is a replica and why do we need a replication controller?

- Let’s go back to our first scenario where we had a single POD running our application.
- What if for some reason, our application crashes and the POD fails?
- Users will no longer be able to access our application. To prevent users from losing access to our application, we would like to have more than one instance or POD running at the same time.
- That way if one fails we still have our application running on the other one. The replication controller helps us run multiple instances of a single POD in the kubernetes cluster thus providing High Availability.
- So does that mean you can’t use a replication controller if you plan to have a single POD?
- No! Even if you have a single POD, the replication controller can help by automatically bringing up a new POD when the existing one fails.
- Thus the replication controller ensures that the specified number of PODs are running at all times. Even if it’s just 1 or 100.

Load Balancing and scaling

- Another reason we need a replication controller is to create multiple PODs to share the load across them.
- For example, in this simple scenario we have a single POD serving a set of users. When the number of users increases we deploy additional POD to balance the load across the two pods.
- If the demand further increases and If we were to run out of resources on the first node, we could deploy additional PODs across other nodes in the cluster. As you can see, the replication controller spans across multiple nodes in the cluster.
- It helps us balance the load across multiple pods on different nodes as well as scale our application when the demand increases.

- It’s important to note that there are two similar terms. Replication Controller and Replica Set. Both have the same purpose but they are not the same.
- Replication Controller is the older technology that is being replaced by Replica Set.
- Replica set is the new recommended way to set up replication. However, whatever we discussed in the previous few slides remains applicable to both these technologies.
- There are minor differences in the way each works and we will look at that in a bit.

Labels and Selectors

- So what is the deal with Labels and Selectors? Why do we label our PODs and objects in kubernetes?
- Let us look at a simple scenario. Say we deployed 3 instances of our frontend web application as 3 PODs.
- We would like to create a replication controller or replica set to ensure that we have 3 active PODs at any time.
- And YES that is one of the use cases of replica sets. You CAN use it to monitor existing pods, if you have them already created, as it IS in this example. In case they were not created, the replica set will create them for you. The role of the replica set is to monitor the pods and if any of them were to fail, deploy new ones.
- The replica set is in FACT a process that monitors the pods. Now, how does the replicaset KNOW what pods to monitor. There could be 100s of other PODs in the cluster running different applications. This is where labelling our PODs during creation comes in handy.
- We could now provide these labels as a filter for replica sets. Under the selector section we use the matchLabels filter and provide the same label that we used while creating the pods. This way the replica set knows which pods to monitor.

[Controller YAML's and Practice Sets are Here](Kubernetes-Beginners/README.md/#controllers)

Commands:

```sh
# Once we change `replica: 6` field in ReplicaSet.yml 
kubectl replace -f ReplicaSet.yml
```

```sh kubectl scale --replicas=6 -f ReplicaSet.yml```

```sh kubectl scale --replicas=6 replicaset nginx-rc```

-> **Deployment**

- For a minute, let us forget about PODs and replica sets and other kubernetes concepts and talk about how you might want to deploy your application in a production environment. Say for example you have a web server that needs to be deployed in a production environment. You need not ONE, but many such instances of the web server running for obvious reasons.

- Secondly, when newer versions of application builds become available on the docker registry, you would like to UPGRADE your docker instances seamlessly.

- However, when you upgrade your instances, you do not want to upgrade all of them at once as we just did. This may impact users accessing our applications, so you may want to upgrade them one after the other. And that kind of upgrade is known as Rolling Updates.

- Suppose one of the upgrades you performed resulted in an unexpected error and you are asked to undo the recent update. You would like to be able to rollBACK the changes that were recently carried out.

- Finally, say for example you would like to make multiple changes to your environment such as upgrading the underlying WebServer versions, as well as scaling your environment and also modifying the resource allocations etc. You do not want to apply each change immediately after the command is run, instead you would like to apply a pause to your environment, make the changes and then resume so that all changes are rolled-out together.

[Deployment YAML's and Practice Sets are Here](Kubernetes-Beginners/README.md/#deployments)

Commands:

| Operation | Commands                                                      |
| --------- | ------------------------------------------------------------ |
| Create    | ```sh kubectl create -f Deployment.yml```                    |
| Get       | ```sh kubectl get po```                                      |
| Update    | ```sh kubectl apply -f  Deployment.yml```                    |
|           | ```sh kubectl set image deplloyment nginx-deploy nging=nginx:1.9.0``` |
| status    | ```sh kubectl rollout status deployment nginx-deploy```      |
|           | ```sh kubectl rollout history deployment nginx-deploy```     |
|           | ```sh kubectl rollout history deployment nginx-deploy --revision=<revision-number>``` |
| rolback   | ```sh kubectl rolllout undo deployment nginx-deploy```       |

### Networking in Kubernets

#### Internal Networking

- Lets start with a single node kubernetes cluster with a single pod and the node has an IP address say it is 192.168.1.2 in this case. This is the IP address we use to access the kubernetes node, ssh etc,.

- On a other side, if we are using minikube setup (IP address of the minikube VM inside hypervisor will be considered, laptop may be having different IP).

- In docker world, IP address is assigned to a conatiner whereas in kubernetes world IP address is always assigned to a POD.

- Each POD in the kubernetes, gets its own internal IP address.(10.244.0.2)

- When the kubernetes is initially confgured, we create an internal private network with the address 10.244.0.0 and all the pods are attached to it. When we deploy multiple PODS, they all get a separate IP addresses assigned from this network like 10.244.0.2, 10.244.0.3, 10.244.0.4.

- The PODs can communicate with each other through this IP(10.244.0.0), but accessing the other PODs using this internal IP address may not be a good idea as it subject to change when the PODs are recreated.

#### Cluster Networking

- For example, we have two nodes running kubernetes with IP addresses 192.168.1.2 and 192.168.1.3 assigned to them (note these are not part of a cluster yet). Each node has a single POD deployed. These PODs are attached to their internal network and have their own IP addresses assigned.

- However, if we observe the internal networks addresses, we can see that they are the same. The two networks have same address(10.244.0.0) and the PODs deployed have the same address too(10.244.0.2).

- This is not going to work well when the nodes are part of the same cluster. The PODs have the same IP addresses assigned to them and that leads to IP conflicts in the network. When a kubernetes cluster is setup, kubernetes does not automatically setup any kind of networking to handle this issues. As a matter of fact, kubernetes expects us to setup networking to meet certain fundamental requirements like:
  - All containers/PODs can communicate to one another without NAT (network address translation-method of remapping an IP address space to another).
  
  - All nodes can communicate with all containers and vice versa without NAT.

- We have multiple pre-build solutions available for this such as cisco SCI networks, vmware NSX, fannel, cilium etc,. Dependening on the platform we are deploying kuberenets cluster on, we can use one of these.

- kubernetes cluster on our system -- cilium, fannel are good options

- kubernetes cluster on vmware -- NSX

- With customer networking either with fannel or cilium setup, it now manages the networks and IPs in the nodes and assigns a different network address for each network in the node. This creates a virtual network of all PODs and nodes where they all assigned a unique IP address and by using simple routing techniques, the cluster networking enables communication between the differnt PODs or nodes to meet the networking requirements of kubernetes.

- Thus now all the PODs can communicate to each other using the assigned IP address.

### Services

- Service is a kubernetes object that enables various communication between various components within and outside of the application.

- Kubernetes services helps us to connect applications together with other applications or users.

- For example, our application has group of PODs running various sections such as a group for serving front-end load to users, other for running backend processes and third one connecting to external data source.

- It is services that enable connectivity between these groups of PODs.

- Services enable the front end application to be made available to users, it helps communication between backend and front end parts and helps in establishing connectivity to an external datasource.

- Thus services enable loose coupling between microservices in our application.

#### Service Types

1. NodePort: This service makes internal POD accessible on a port on the node.

2. ClusterIP: This service creates a vitrualIP inside the cluster, to enable communication between different services such as set of frontend servers to a set of backend servers.

3. LoadBalancer: This provisions a load balancer for our application in supported cloud providers.

-> Create a service -- Nodeport

![Image Info](Image/Kuberetes-16.png)

Among ports, port is only one which is mandatory. If we dont provide target port, by default target port is assumed to be same as port. If we dont provide nodePort, the free port between range **30000-32767** will be assigned as nodeport.

Now we can access the POD using curl
```sh curl http://192.168.1.2:30008```
Here 192.168.1.2 is the IP address of node and 30008 is the nodeport.

If we are using minikube then:
`minikube service <servicename> --url`

-> Create a service -- ClusterIP

![Image Info](Image/Kuberetes-17.png)

- A full stack application will have different types of PODs hosting different parts of an application.

- To connect different pods like frontend pods with backend pods and backend pods with database pods.

- All pods are assigned with a specific IP address, but IP addresses are not static because these PODS may go at anytime and new PODS may come into action, so we cannot rely on IP addresses for internal communication between the application.

- A kubernetes service can help group the PODs together and provide single interface to access the PODs in a group. The request will be forwarded to one of the PODs under the service randomly.

- In this case, two services will be created one for backend and one for redis for commnication.

- This enables us to easily and effectively deploy microservices based application on kubernetes cluster. Each layer can scale or move without effecting various services. Each service gets an IP and name and assigned to it inside the cluster and that it is name that to be used by other PODs to access the service. This type of service is called clusterIP.

-> Create a service -- LoadBalancer

![Image Info](Image/Kuberetes-18.png)

- To make the application accessible to the external user, we create the services of type NodePort. The services of type NodePort helps in receiving the traffic on the ports of the node and routing the traffic to the respective PODs.

- When we have 4 nodes, with what url we can access the application, we can access the application with any of the 4 urls(IP address of the nodes:port).

- All the PODs of the cluster can be accessed from any node of the cluster (irrespective of the particular node in which they reside).

- The end users want a single url(not many) to access, to achieve that we can create a new VM for load balancing purpose and install and configure a suitable loadbalancer on it (like proxy) and then configure the load balancer to route traffic to the underlying nodes. This way will be tedious.

- If we were on a supported cloud platform like Google Cloud or NWS or Azure, we could leverage the native load balancer of that cloud platform. Kubernetes has support for integrating with the native load balancers of certain cloud providers and configuring that for us.

- For this, we just need to set the type as LoadBalancer.

- This will easily work only on cloud platforms because of in-build Load Balancer setup.

[Service YAML's and Practice Sets are Here](Kubernetes-Beginners/README.md/#services)

Commands:

```sh
kubectl create service-${Type}.yml

kubectl get services
```

### MicroServices Architechture

#### Deploying an application on Docker

![Image Info](Image/Kuberetes-19.png)

#### Deploying an application on kubernetes cluster

-> In this application, we have

`voting-app --> redis <-- worker --> postgres --> result-app`

-> Our Goals are:

- Deploy Containers
- Enable connectivity
- Extrenal access for the users.

-> Steps:

- Deploy PODs
- We need to know what are the connectivity requirements. We need to be clear on what application requires access to what services.
- Redis database is accessed by both voting-app and worker app. The voting-app saves the vote to the redis database and worker app reads the vote from the redis database.
- Postgres database is accessed by the worker app to update it with the total count of the votes and also it is accessed by the result-app to read the total counts of votes to be displayed.
- voting-app is accessed by the external users i.e., voters and the result-app is also used by the external users to view the results.
- worker app is not being accessed by any one.

![Image Info](Image/Kuberetes-20.png)

- A service is only required if the application has some kind of database or process that needs to be exposed or accessed by others.

### Kubernetes On Cloud

There are various options to deploy a kubernetes cluster on the cloud like

- Google Cloud Platform
- Amazon Web Services
- Microsoft Azure

For production purposes there are many ways to get started with the kubernetes cluster both in a private or public cloud environment.

-> Self Hosted / Turnkey Solutions

- You provison VMs
- You Configure VMs
- You use Scripts to Deploy Cluster
- You maintain VMs yourself
eg: Kubernetes on AWS using kops or KubeOne

-> Hosted Solutions (Managed Solutions)

- Kubernetes-As-A-Service
- Provider provisions VMs
- Provider installs Kubernetes
- Provider maintains VMs
eg: Google Container Engine(GKE)

### Kubernets vs Docker Swarm

#### What is Kubernetes?

[Kubernetes](https://www.ibm.com/cloud/learn/kubernetes) is developed by the community with the intent of addressing container scalability and management needs. In the early days of Kubernetes, the community contributors leveraged their knowledge of creating and running internal tools, such as Borg and Omega. With the advent of the Cloud Native Computing Foundation (CNCF) in partnership with the Linux Foundation, the community adopted Open Governance for Kubernetes. IBM, as a founding member of CNCF, actively contributes to CNCF’s [cloud-native](https://www.ibm.com/cloud/learn/cloud-native) projects, along with other companies like Google, Red Hat, Microsoft, and Amazon.

Kubernetes is an open source container-management tool for those important containers and their complex production workloads. With Kubernetes, developers and DevOps teams can schedule, deploy, manage, and discover highly available apps by using the flexibility of clusters. A [Kubernetes cluster](https://www.ibm.com/cloud/blog/kubernetes-clusters-architecture-for-rapid-controlled-cloud-app-delivery) is made up of compute hosts that are called worker nodes. These worker nodes are managed by a Kubernetes master that controls and monitors all resources in the cluster. A node can be a virtual machine or  physical, bare metal machine.

##### Pros of Kubernetes

- [Open-source community](https://kubernetes.io/) that is very active in developing the code base
- Fast-growing KubeCon conferences throughout the year that are more than doubling attendance numbers
- Battle-tested by big players like Google and our own IBM workloads and runs on most operating systems
- Largest adoption in the market
- Available on the public cloud or for on-premises — managed or non-managed offerings from all the big cloud providers (IBM Cloud, AWS, Microsoft Azure, Google Cloud Platform, etc.)
- Broad Kubernetes support from an ecosystem of cloud tool vendors, such as Sysdig, LogDNA, and Portworx (among many others)
- Key functionalities include service discovery, [ingress](https://www.ibm.com/cloud/blog/kubernetes-ingress) and [load balancing](https://www.ibm.com/cloud/learn/load-balancing), self-healing, storage orchestration, horizontal scalability, automated rollouts and rollbacks, and batch execution
- Unified set of APIs and strong guarantees about the cluster state

##### Cons of Kubernetes

- Management of the Kubernetes master takes specialized knowledge
- Updates from open source community are frequent and require careful patching in order to avoid disrupting workloads
- Too heavyweight for individual developers to set up for simplistic apps and infrequent deployments
- Often need additional tools (e.g., kubectl CLI), services, continuous integration/continuous deployment (CI/CD) workflows and other DevOps practices to fully manage access, identity, governance and security

#### What is Docker Swarm?

Docker Swarm is another open-source container orchestration platform that has been around for a while. Swarm —or more accurately, *swarm mode* — is Docker’s native support for orchestrating clusters of [Docker](https://www.ibm.com/cloud/learn/docker) engines. A Swarm cluster consists of Docker Engine deployed Swarm manager nodes (which orchestrate and manage the cluster) and worker nodes (which are directed to execute tasks by the manager nodes).

##### Pros of Docker Swarm

- Built for use with the Docker Engine (Docker is a container platform used for building and deploying containerized applications)
- Has its own Swarm API
- Smoothly integrates with Docker tools like Docker Compose and Docker CLI (uses the same command line interface (CLI) as Docker Engine)
- Tools, services, and software that run with Docker containers will also work well with Swarm
- Is easy to install and set up for Docker environments
- Uses a filtering and scheduling system to provide intelligent node selection, allowing you to pick the optimal nodes in a cluster for container deployment

##### Cons of Docker Swarm

- Limited customizations and extensions
- Less functionality-rich than Kubernetes
- No easy way to separate Dev-Test-Prod workloads in DevOps pipeline

Not to confuse matters too much, but [Docker Enterprise Edition now supports Kubernetes too](https://thenewstack.io/docker-fully-embraces-kubernetes/).

| Operations             | Kubernetes                                                   | Docker Swarm                                                 |
| ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Installation and setup | No installation required for managed offerings from cloud providers. But for VM installation it is hard but widely used | Install it with Docker.                                      |
| Scalability            | Built-in with horizontal auto-scaling.                       | Auto-scaling groups.                                         |
| Load balancing         | Discovery of services through a single DNS name. Access to container applications through IP address or HTTP route. | Internal load balancers.                                     |
| High availability      | Self-healing and intelligent scheduling. High availability of services through replication. | Use Swarm Managers for availability controls.                |
| Deployment             | **Both Docker Swarm and Kubernetes provide a means to apply rolling updates and for rolling back those updates as required** | **Docker Swarm deployments are considered much more user-friendly than Kubernetes** |
| Service Discovery      | **Both Docker Swarm and Kubernetes provide DNS based service discovery**. | **Both Docker Swarm and Kubernetes provide DNS based service discovery**. |
| Performance            | Therefore, **applications deployed with Docker Swarm and Kubernetes will operate with similar speed and efficiency**. | **Docker Swarm will deploy and start containers as much as five times more quickly than Kubernetes** and **Docker Swarms ability to respond to API calls much more quickly** |

The main reason we have chosen Kubernetes over Docker Swarm is related to the following artifacts:

- **Key features:** Easy and flexible installation, Clear dashboard, Great scaling operations, Monitoring is an integral part, Great load balancing concepts, Monitors the condition and ensures compensation in the event of failure.
- **Applications:** An application can be deployed using a combination of pods, deployments, and services (or micro-services).
- **Functionality:** Kubernetes as a complex installation and setup process, but it not as limited as Docker Swarm.
- **Monitoring:** It supports multiple versions of logging and monitoring when the services are deployed within the cluster (Elasticsearch/Kibana (ELK), Heapster/Grafana, Sysdig cloud integration).
- **Scalability:** All-in-one framework for distributed systems.
- **Other Benefits:** Kubernetes is backed by the Cloud Native Computing Foundation (CNCF), huge community among container orchestration tools, it is an open source and modular tool that works with any OS.

#### K8s vs K3s

| K8s                                                          | K3s                                                          |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Kubernetes uses kubelet, an agent running on each Kubernetes node to perform a control loop of the containers running on that node. This agent runs inside the container. However, K3s does not use kubelet, but it runs kubelet on the host machine and uses the host’s scheduling mechanism to run containers. | K3s are not functionally different from K8s, but they have some differences that make them unique. K3s can deploy applications faster than kubernetes. Not only that, K3s can spin up clusters more quickly than K8s. K8s is a general-purpose container orchestrator, while K3s is a purpose-built container orchestrator for running Kubernetes on bare-metal servers. |
| Kubernetes or K8s can host [workloads](<https://www.delltechnologies.com/en-in/learn/cloud/cloud-workloads.htm#:~:text=A> cloud workload is a,are all considered cloud workloads.) running across multiple environments, while K3s can only host workloads running in a single cloud. It mainly happens because K3s don’t contain the capacity to maintain a significant workload on multiple clouds as it is small in size. | Again, we can see that K3S is lightweight because of its small size, and this helps it run [clusters](<https://www.vmware.com/topics/glossary/content/kubernetes-cluster#:~:text=A> Kubernetes cluster is a,dependences and some necessary services.&text=Kubernetes clusters allow containers to,based%2C and on-premises.) in IoT devices such as [Raspberry Pi](https://www.raspberrypi.org/), which has limited resources. In contrast, we can see that normal Kubernetes or K8s is not operable in IoT or edge computing devices. Also, K3s supports both ARM64 and ARMv7 with binaries. |
| At the same time, we can see that Kubernetes, due to its heavy size, takes advantage of hosting workloads and spin up clusters in multiple clouds. K3s is a standalone server, unlike K8s, which is a part of the Kubernetes cluster. K8s relies on CRI-O to integrate Kubernetes with CRI (Container Runtime Interface) while K3s uses CRI-O, and therefore is compatible with all of the supported container runtimes. K8s uses kubelet to schedule containers, but K3s uses the host’s scheduling mechanism to schedule containers. | K3s uses [kube-proxy](<https://kubernetes.io/docs/concepts/overview/components/#:~:text=kube-proxy> is a network,or outside of your cluster.) to proxy the network connections of the Kubernetes nodes, but K8s uses kube-proxy to proxy the network connections of an individual container. It also uses kube-proxy to set up IP masquerading, while K3s does not use kube-proxy to do that. |
| Again, K8s uses [kubelet](<https://kubernetes.io/docs/reference/command-line-tools-reference/kubelet/#:~:text=The> kubelet is the primary,object that describes a pod.) to watch the Kubernetes nodes for changes in the configuration, while K3s does not watch Kubernetes nodes for changes in the configuration. Instead, it receives a deployment manifest containing the configuration information from the Kubernetes control plane and makes changes accordingly. | k3s can have [tighter security](https://sysdig.com/blog/k3s-sysdig-falco/) deployment than k8s because of their small attack surface area. Another advantage of k3s is that it can reduce the dependencies and steps needed to install, run or update a Kubernetes cluster. |
| Kubernetes can be very beneficial when it comes to [orchestration](https://www.redhat.com/en/topics/containers/what-is-container-orchestration) (arrangement and coordination of automated tasks) of large databases as it can maintain the load of the database. At the same time, k3s can be more than useful for small databases. It happens to come in a single binary file of less than 100 MB, which will help to fire up quick clusters, faster scheduling pods and other tasks. |                                                              |

--------------------------------------

## **Kubernetes Development**

### What is Kubernets?

### Demo App in Kubernets

### Docker Container for App

### Kubernetes On Minikube

### Moving to Azure AKS

### DevOps for Kubernetes using Azure DevOps

### CI/CD Pipelines for Kubernetes using YAML pipelines

### Deploying using Helm

### Ingress Controller

### GitOps with Kubernetes

### Kubernetes NodePools

### Upgrade the Cluster

### Cluster backup

--------------------------------------

## **Kubernetes Administration**

### Introduction

What is Kubernetes?
It's is an open-source container orchestration tool designed to automate deploying, scaling, and operating containerized applications. Kubernetes was born from Google's 15-year experience running production workloads. It is designed to grow from tens, thousands, or even millions of containers.

Difference between Docker and Kubernetes
A fundamental difference between Kubernetes and Docker is that Kubernetes is meant to run across a cluster while Docker runs on a single node. Kubernetes is more extensive than Docker Swarm and is meant to coordinate clusters of nodes at scale in production in an efficient manner.

what is CKAD?
According to cncf,
A Certified Kubernetes Application Developer can define application resources and use core primitives to build, monitor, and troubleshoot scalable applications and tools in Kubernetes. The exam assumes knowledge of, but does not test for, container runtimes and a microservice architecture.

Certification Details:

Below are some references:

- Certified Kubernetes Administrator: <https://www.cncf.io/certification/cka/>
- Exam Curriculum (Topics): <https://github.com/cncf/curriculum>
- Candidate Handbook: <https://www.cncf.io/certification/candidate-handbook>
- Exam Tips: <http://training.linuxfoundation.org/go//Important-Tips-CKA-CKAD>
Use the code - DEVOPS15 - while registering for the CKA or CKAD exams at Linux Foundation to get a 15% discount.

Practice Reference:

- **K8s Hard Way: <https://github.com/mmumshad/kubernetes-the-hard-way>**
- **CKA: <https://github.com/kodekloudhub/certified-kubernetes-administrator-course>**
- **Killer shell: <https://killercoda.com/killer-shell-cka>**
- practice: <https://github.com/vzhovtan/cka_practice_questions>, <https://gist.github.com/texasdave2/8f4ce19a467180b6e3a02d7be0c765e7>, <https://github.com/alijahnas/CKA-practice-exercises>, <https://gist.github.com/PavelSlepushkin/43717d9383eb47d1ec2c87d6275ccea6>, <https://github.com/MatthewAtkinson24/Build-Your-Career-With-Latest-Linux-Foundation-CKA-PDF-Dumps-2022->

### Core Concepts

#### Cluster Architechture

In Kubernetes we have Master and Worker Node. Master node is also known as Control Panel node and Worker node is known as Minion.

![Image Info](Image/CKA-1.png)

**Master Node or Control Panel Node**: A master is other node with kubernetes installed in it and is configured as a master.
The master watches over the nodes in the cluster and is reponsible for the actual orchestration of containers on the worker nodes.
Master node manages the cluster, this will have information about the members of the cluster, this monitor the nodes and when a node fails, this will move the load of the failed node to other worker nodes.

**Worker Node or Minion or Compute Machine**: Worker Node or Minion is where the containers are hosted. To run containers on the system, we need container runtime installed. Therefore, worker nodes will have container runtime.

**Node**: Node is a physical machine or virtual machine on which kubernetes is installed. A node is a worker machine(minions), where containers are launched by kubernetes. We need to have more than one node, inorder to maintain the application if one node fails.

**Cluster**: A cluster is a set of nodes grouped together. If one node fails, our application will be still accessible from other nodes. Having multiple nodes help in sharing load as well.

![Image info](Image/CKA-3.png)

**Components**:

![Image Info](Image/CKA-2.png)

When we install the kubernetes in the system, we are actually installing the following components.

Master Components:

- API Server --> frontend for kubernetes. Users, management devices, CLI all talk to the apiServer to interact with kubernetes cluster.
- etcd --> key-value store (to store all data (in distributed manner) to manage cluster)
- Controller --> brain behind otchestration, responsible for noticing and managing when nodes, containers, endpoints goes down.
- scheduler --> distributes work to all containers across multiple nodes.

Worker Components:

- kubelet --> agent that runs on each node on the cluster and make sure that containers are running as expected.
- Container Runtime --> used to run containers i.e., docker

**Master vs Worker Nodes:**

- Worker Node or Minion is where the containers are hosted. To run containers on the system, we need container runtime installed. Therefore, worker nodes will have container runtime (docker).
- Master node will have Kube-API server and thats make it a master.
- Worker node will have kubelet agent that is responsible to interact with the master to provide health information of the worker node and to carry out actions requested by the master on the worker nodes.
- All the information gathered is stored in the key-value store on the master. The key-value store is based on the popular etcd framework.
- The master also has Controller and Scheduler.

##### ETCD

Configuration data and information about the state of the cluster lives in etcd, a key-value store database. Fault-tolerant and distributed, etcd is designed to be the ultimate source of truth about your cluster.
Port: **2379**

Outside K8s ETCD:

1. Download Binaries: curl -L <https://github.com/etcd-io/etcd/releases/download/v3.3.11/etcd-v3.3.11-linux-amd64.tar.gz> -o etcd-v3.3.11-linux-amd64.tar.gz

2. Extract: tar xzvf etcd-v3.3.11-linux-amd64.tar.gz

3. Run ETCD Service: ./etcd

Manual Setup of ETCD on K8s:

step-1

```sh
$ wget -q --https-only \
"https://github.com/coreos/etcd/releases/download/v3.3.9/etcd-v3.3.9-linux-amd64.tar.gz"
```

step-2

```sh
etcd.service
```

```yaml
ExecStart=/usr/local/bin/etcd \\
--name ${ETCD_NAME} \\
--cert-file=/etc/etcd/kubernetes.pem \\
--key-file=/etc/etcd/kubernetes-key.pem \\
--peer-cert-file=/etc/etcd/kubernetes.pem \\
--peer-key-file=/etc/etcd/kubernetes-key.pem \\
--trusted-ca-file=/etc/etcd/ca.pem \\
--peer-trusted-ca-file=/etc/etcd/ca.pem \\
--peer-client-cert-auth \\
--client-cert-auth \\
--initial-advertise-peer-urls https://${INTERNAL_IP}:2380 \\
--listen-peer-urls https://${INTERNAL_IP}:2380 \\
--listen-client-urls https://${INTERNAL_IP}:2379,https://127.0.0.1:2379 \\
--advertise-client-urls https://${INTERNAL_IP}:2379 \\
--initial-cluster-token etcd-cluster-0 \\
**--initial-cluster controller-0=https://${CONTROLLER0_IP}:2380,controller-1=https://${CONTROLLER1_IP}:2380 \\**
--initial-cluster-state new \\
--data-dir=/var/lib/etcd
```

Kubeadm Setup:

step-1

```sh
$ kubectl get pods -n kube-system
NAMESPACE NAME READY STATUS RESTARTS AGE
kube-system coredns-78fcdf6894-prwvl 1/1 Running 0 1h
kube-system coredns-78fcdf6894-vqd9w 1/1 Running 0 1h
kube-system etcd-master 1/1 Running 0 1h
kube-system kube-apiserver-master 1/1 Running 0 1h
kube-system kube-controller-manager-master 1/1 Running 0 1h
kube-system kube-proxy-f6k26 1/1 Running 0 1h
kube-system kube-proxy-hnzsw 1/1 Running 0 1h
kube-system kube-scheduler-master 1/1 Running 0 1h
kube-system weave-net-924k8 2/2 Running 1 1h
kube-system weave-net-hzfcz 2/2 Running 1 1h
NAMESPACE NAME READY STATUS RESTARTS AGE
kube-system coredns-78fcdf6894-prwvl 1/1 Running 0 1h
kube-system coredns-78fcdf6894-vqd9w 1/1 Running 0 1h
kube-system etcd-master 1/1 Running 0 1h
kube-system kube-apiserver-master 1/1 Running 0 1h
kube-system kube-controller-manager-master 1/1 Running 0 1h
kube-system kube-proxy-f6k26 1/1 Running 0 1h
kube-system kube-proxy-hnzsw 1/1 Running 0 1h
kube-system kube-scheduler-master 1/1 Running 0 1h
kube-system weave-net-924k8 2/2 Running 1 1h
kube-system weave-net-hzfcz 2/2 Running 1 1h
```

```sh
# Run below on the ETCD Master Node
$ kubectl exec etcd-master –n kube-system etcdctl get / --prefix –keys-only
/registry/apiregistration.k8s.io/apiservices/v1.
/registry/apiregistration.k8s.io/apiservices/v1.apps
/registry/apiregistration.k8s.io/apiservices/v1.authentication.k8s.io
/registry/apiregistration.k8s.io/apiservices/v1.authorization.k8s.io
/registry/apiregistration.k8s.io/apiservices/v1.autoscaling
/registry/apiregistration.k8s.io/apiservices/v1.batch
/registry/apiregistration.k8s.io/apiservices/v1.networking.k8s.io
/registry/apiregistration.k8s.io/apiservices/v1.rbac.authorization.k8s.io
/registry/apiregistration.k8s.io/apiservices/v1.storage.k8s.io
/registry/apiregistration.k8s.io/apiservices/v1beta1.admissionregistration.k8s.io
```

ETCD will explore on below from etcd master node:

|                   | Pods        |
| ----------------- | ----------- |
|                   | Replicasets |
| Registry  minions | deployment  |
|                   | roles       |
|                   | serets      |

etcd on HA:

```sh
etcd.service
```

```yaml
ExecStart=/usr/local/bin/etcd \\
--name ${ETCD_NAME} \\
--cert-file=/etc/etcd/kubernetes.pem \\
--key-file=/etc/etcd/kubernetes-key.pem \\
--peer-cert-file=/etc/etcd/kubernetes.pem \\
--peer-key-file=/etc/etcd/kubernetes-key.pem \\
--trusted-ca-file=/etc/etcd/ca.pem \\
--peer-trusted-ca-file=/etc/etcd/ca.pem \\
--peer-client-cert-auth \\
--client-cert-auth \\
--initial-advertise-peer-urls https://${INTERNAL_IP}:2380 \\
--listen-peer-urls https://${INTERNAL_IP}:2380 \\
--listen-client-urls https://${INTERNAL_IP}:2379,https://127.0.0.1:2379 \\
--advertise-client-urls https://${INTERNAL_IP}:2379 \\
--initial-cluster-token etcd-cluster-0 \\
**--initial-cluster controller-0=https://${CONTROLLER0_IP}:2380,controller-1=https://${CONTROLLER1_IP}:2380 \\**
--initial-cluster-state new \\
--data-dir=/var/lib/etcd
```

##### kube-apiserver

Need to interact with your Kubernetes cluster? Talk to the API. The Kubernetes API is the front end of the Kubernetes control plane, handling internal and external requests. The API server determines if a request is valid and, if it is, processes it. You can access the API through REST calls, through the kubectl command-line interface, or through other command-line tools such as kubeadm.

![Image Info](Image/CKA-4.png)

Manual setup:

```sh
wget https://storage.googleapis.com/kubernetes-release/release/v1.13.0/bin/linux/amd64/kube-apiserver
```

```yaml
ExecStart=/usr/local/bin/kube-apiserver \\
--advertise-address=${INTERNAL_IP} \\
--allow-privileged=true \\
--apiserver-count=3 \\
--authorization-mode=Node,RBAC \\
--bind-address=0.0.0.0 \\
--enable-admission-
plugins=Initializers,NamespaceLifecycle,NodeRestriction,LimitRanger,ServiceAccount,DefaultStorageClass,ResourceQuota \\
--enable-swagger-ui=true \\
--etcd-cafile=/var/lib/kubernetes/ca.pem \\
--etcd-certfile=/var/lib/kubernetes/kubernetes.pem \\
--etcd-keyfile=/var/lib/kubernetes/kubernetes-key.pem \\
--etcd-servers=https://127.0.0.1:2379 \\
--event-ttl=1h \\
--experimental-encryption-provider-config=/var/lib/kubernetes/encryption-config.yaml \\
--kubelet-certificate-authority=/var/lib/kubernetes/ca.pem \\
--kubelet-client-certificate=/var/lib/kubernetes/kubernetes.pem \\
--kubelet-client-key=/var/lib/kubernetes/kubernetes-key.pem \\
--kubelet-https=true \\
--runtime-config=api/all \\
--service-account-key-file=/var/lib/kubernetes/service-account.pem \\
--service-cluster-ip-range=10.32.0.0/24 \\
--service-node-port-range=30000-32767 \\
--v=2
```

Kubeadm Setup:

```sh
$ kubectl get pods -n kube-system
NAMESPACE NAME READY STATUS RESTARTS AGE
kube-system coredns-78fcdf6894-hwrq9 1/1 Running 0 16m
kube-system coredns-78fcdf6894-rzhjr 1/1 Running 0 16m
kube-system etcd-master 1/1 Running 0 15m
kube-system kube-apiserver-master 1/1 Running 0 15m
kube-system kube-controller-manager-master 1/1 Running 0 15m
kube-system kube-proxy-lzt6f 1/1 Running 0 16m
kube-system kube-proxy-zm5qd 1/1 Running 0 16m
kube-system kube-scheduler-master 1/1 Running 0 15m
kube-system weave-net-29z42 2/2 Running 1 16m
kube-system weave-net-snmdl 2/2 Running 1 16m
```

```yaml
cat /etc/kubernetes/manifests/kube-apiserver.yaml
spec:
containers:
- command:
- kube-apiserver
- --authorization-mode=Node,RBAC
- --advertise-address=172.17.0.32
- --allow-privileged=true
- --client-ca-file=/etc/kubernetes/pki/ca.crt
- --disable-admission-plugins=PersistentVolumeLabel
- --enable-admission-plugins=NodeRestriction
- --enable-bootstrap-token-auth=true
- --etcd-cafile=/etc/kubernetes/pki/etcd/ca.crt
- --etcd-certfile=/etc/kubernetes/pki/apiserver-etcd-client.crt
- --etcd-keyfile=/etc/kubernetes/pki/apiserver-etcd-client.key
- --etcd-servers=https://127.0.0.1:2379
- --insecure-port=0
- --kubelet-client-certificate=/etc/kubernetes/pki/apiserver-kubelet-client.crt
- --kubelet-client-key=/etc/kubernetes/pki/apiserver-kubelet-client.key
- --kubelet-preferred-address-types=InternalIP,ExternalIP,Hostname
- --proxy-client-cert-file=/etc/kubernetes/pki/front-proxy-client.crt
- --proxy-client-key-file=/etc/kubernetes/pki/front-proxy-client.key
- --requestheader-allowed-names=front-proxy-client
- --requestheader-client-ca-file=/etc/kubernetes/pki/front-proxy-ca.crt
- --requestheader-extra-headers-prefix=X-Remote-Extra-
- --requestheader-group-headers=X-Remote-Group
- --requestheader-username-headers=X-Remote-User
```

```sh
$ cat /etc/systemd/system/kube-apiserver.service
[Service]
ExecStart=/usr/local/bin/kube-apiserver \\
--advertise-address=${INTERNAL_IP} \\
--allow-privileged=true \\
--apiserver-count=3 \\
--audit-log-maxage=30 \\
--audit-log-maxbackup=3 \\
--audit-log-maxsize=100 \\
--audit-log-path=/var/log/audit.log \\
--authorization-mode=Node,RBAC \\
--bind-address=0.0.0.0 \\
--client-ca-file=/var/lib/kubernetes/ca.pem \\
--enable-admission-
plugins=Initializers,NamespaceLifecycle,NodeRestriction,LimitRanger,ServiceAccount,DefaultStorageClass,ResourceQuota \\
--enable-swagger-ui=true \\
--etcd-cafile=/var/lib/kubernetes/ca.pem \\
--etcd-certfile=/var/lib/kubernetes/kubernetes.pem \\
--etcd-keyfile=/var/lib/kubernetes/kubernetes-key.pem \\
--etcd-
servers=https://10.240.0.10:2379,https://10.240.0.11:2379,https://10.240.0.12:2379 \\
--event-ttl=1h \\
--experimental-encryption-provider-config=/var/lib/kubernetes/encryption-config.yaml
\\
--kubelet-certificate-authority=/var/lib/kubernetes/ca.pem \\
--kubelet-client-certificate=/var/lib/kubernetes/kubernetes.pem \\
```

```sh
$ ps -aux | grep kube-apiserver
root 2348 3.3 15.4 399040 315604 ? Ssl 15:46 1:22 kube-apiserver --authorization-mode=Node,RBAC --advertise-address=172.17.0.32 --allow-privileged=true --client-ca-file=/etc/kubernetes/pki/ca.crt --disable-
admission-plugins=PersistentVolumeLabel --enable-admission-plugins=NodeRestriction --enable-bootstrap-token-auth=true --etcd-cafile=/etc/kubernetes/pki/etcd/ca.crt --etcd-certfile=/etc/kubernetes/pki/apiserver-etcd-client.crt --etcd-keyfile=/etc/kubernetes/pki/apiserver-etcd-client.key --etcd-servers=https://127.0.0.1:2379 --insecure-port=0 --kubelet-client-certificate=/etc/kubernetes/pki/apiserver-kubelet-client.crt --kubelet-client-key=/etc/kubernetes/pki/apiserver-kubelet-client.key --kubelet-preferred-address-types=InternalIP,ExternalIP,Hostname --proxy-client-cert-file=/etc/kubernetes/pki/front-proxy-client.crt --proxy-client-key-file=/etc/kubernetes/pki/front-proxy-client.key --requestheader-allowed-names=front-proxy-client --requestheader-client-ca-file=/etc/kubernetes/pki/front-proxy-ca.crt --requestheader-extra-headers-prefix=X-Remote-Extra- --requestheader-group-headers=X-Remote-Group --requestheader-username-headers=X-Remote-User --secure-port=6443 --service-account-key-file=/etc/kubernetes/pki/sa.pub --service-cluster-ip-range=10.96.0.0/12 --tls-cert-file=/etc/kubernetes/pki/apiserver.crt --tls-private-key-file=/etc/kubernetes/pki/apiserver.key
```

##### kube-controller-manager

![Replication Controller](Image/CKA-5.png)

Controllers take care of actually running the cluster, and the Kubernetes controller-manager contains several controller functions in one. One controller consults the scheduler and makes sure the correct number of pods is running. If a pod goes down, another controller notices and responds. A controller connects services to pods, so requests go to the right endpoints. And there are controllers for creating accounts and API access tokens.

![Node Controller](Image/CKA-6.png)

![All Controllers](Image/CKA-7.png)

Manual SetUp:

```sh
$ wget https://storage.googleapis.com/kubernetes-release/release/v1.13.0/bin/linux/amd64/kube-controller-manager

ExecStart=/usr/local/bin/kube-controller-manager \\
--address=0.0.0.0 \\
--cluster-cidr=10.200.0.0/16 \\
--cluster-name=kubernetes \\
--cluster-signing-cert-file=/var/lib/kubernetes/ca.pem \\
--cluster-signing-key-file=/var/lib/kubernetes/ca-key.pem \\
--kubeconfig=/var/lib/kubernetes/kube-controller-manager.kubeconfig \\
--leader-elect=true \\
--root-ca-file=/var/lib/kubernetes/ca.pem \\
--service-account-private-key-file=/var/lib/kubernetes/service-account-key.pem \\
--service-cluster-ip-range=10.32.0.0/24 \\
--use-service-account-credentials=true \\
--v=2
```

```sh
--controllers stringSlice Default: [*]
A list of controllers to enable. '*' enables all on-by-default controllers, 'foo' enables the controller
named 'foo', '-foo' disables the controller named 'foo'.
All controllers: attachdetach, bootstrapsigner, clusterrole-aggregation, cronjob, csrapproving,
csrcleaner, csrsigning, daemonset, deployment, disruption, endpoint, garbagecollector,
horizontalpodautoscaling, job, namespace, nodeipam, nodelifecycle, persistentvolume-binder,
persistentvolume-expander, podgc, pv-protection, pvc-protection, replicaset, replicationcontroller,
resourcequota, root-ca-cert-publisher, route, service, serviceaccount, serviceaccount-token, statefulset,
tokencleaner, ttl, ttl-after-finished
Disabled-by-default controllers: bootstrapsigner, tokencleaner
```

Kubeadm Setup:

```sh
$ kubectl get pods -n kube-system
NAMESPACE NAME READY STATUS RESTARTS AGE
kube-system coredns-78fcdf6894-hwrq9 1/1 Running 0 16m
kube-system coredns-78fcdf6894-rzhjr 1/1 Running 0 16m
kube-system etcd-master 1/1 Running 0 15m
kube-system kube-apiserver-master 1/1 Running 0 15m
kube-system kube-controller-manager-master 1/1 Running 0 15m
kube-system kube-proxy-lzt6f 1/1 Running 0 16m
kube-system kube-proxy-zm5qd 1/1 Running 0 16m
kube-system kube-scheduler-master 1/1 Running 0 15m
kube-system weave-net-29z42 2/2 Running 1 16m
kube-system weave-net-snmdl 2/2 Running 1 16m
```

```yaml
$ cat /etc/kubernetes/manifests/kube-controller-manager.yaml
spec:
containers:
- command:
- kube-controller-manager
- --address=127.0.0.1
- --cluster-signing-cert-file=/etc/kubernetes/pki/ca.crt
- --cluster-signing-key-file=/etc/kubernetes/pki/ca.key
- --controllers=*,bootstrapsigner,tokencleaner
- --kubeconfig=/etc/kubernetes/controller-manager.conf
- --leader-elect=true
- --root-ca-file=/etc/kubernetes/pki/ca.crt
- --service-account-private-key-file=/etc/kubernetes/pki/sa.key
- --use-service-account-credentials=true
```

```sh
cat /etc/systemd/system/kube-controller-manager.service
[Service]
ExecStart=/usr/local/bin/kube-controller-manager \\
--address=0.0.0.0 \\
--cluster-cidr=10.200.0.0/16 \\
--cluster-name=kubernetes \\
--cluster-signing-cert-file=/var/lib/kubernetes/ca.pem \\
--cluster-signing-key-file=/var/lib/kubernetes/ca-key.pem \\
--kubeconfig=/var/lib/kubernetes/kube-controller-manager.kubeconfig \\
--leader-elect=true \\
--root-ca-file=/var/lib/kubernetes/ca.pem \\
--service-account-private-key-file=/var/lib/kubernetes/service-account-key.pem \\
--service-cluster-ip-range=10.32.0.0/24 \\
--use-service-account-credentials=true \\
--v=2
Restart=on-failure
RestartSec=5
```

```sh
$ ps -aux | grep kube-controller-manager
root 1994 2.7 5.1 154360 105024 ? Ssl 06:45 1:25 kube-controller-manager --address=127.0.0.1 --cluster-signing-cert-file=/etc/kubernetes/pki/ca.crt --cluster-signing-key-file=/etc/kubernetes/pki/ca.key --controllers=*,bootstrapsigner,tokencleaner --kubeconfig=/etc/kubernetes/controller-manager.conf --leader-elect=true --root-ca-file=/etc/kubernetes/pki/ca.crt --service-account-private-key-file=/etc/kubernetes/pki/sa.key --use-service-account-credentials=true
```

##### kube-scheduler

Is your cluster healthy? If new containers are needed, where will they fit? These are the concerns of the Kubernetes scheduler.

The scheduler considers the resource needs of a pod, such as CPU or memory, along with the health of the cluster. Then it schedules the pod to an appropriate compute node.

![Kube-Scheduler](Image/CKA-8.png)

Manual SetUp:

```sh
$ wget https://storage.googleapis.com/kubernetes-release/release/v1.13.0/bin/linux/amd64/kube-scheduler
ExecStart=/usr/local/bin/kube-scheduler \\
--config=/etc/kubernetes/config/kube-scheduler.yaml \\
--v=2
```

Kubeadm SetUp:

```yaml
$ cat /etc/kubernetes/manifests/kube-scheduler.yaml
spec:
containers:
- command:
- kube-scheduler
- --address=127.0.0.1
- --kubeconfig=/etc/kubernetes/scheduler.conf
- --leader-elect=true
```

```sh
$ ps -aux | grep kube-scheduler
root 2477 0.8 1.6 48524 34044 ? Ssl 17:31 0:08 kube-scheduler --
address=127.0.0.1 --kubeconfig=/etc/kubernetes/scheduler.conf --leader-elect=true
```

##### Kubelet

Each compute node contains a kubelet, a tiny application that communicates with the control plane. The kublet makes sure containers are running in a pod. When the control plane needs something to happen in a node, the kubelet executes the action.

![Kubelet](Image/CKA-9.png)

Kubeadm does not deploy `Kubelets`

```sh
$ wget https://storage.googleapis.com/kubernetes-release/release/v1.13.0/bin/linux/amd64/kubelet

ExecStart=/usr/local/bin/kubelet \\
--config=/var/lib/kubelet/kubelet-config.yaml \\
--container-runtime=remote \\
--container-runtime-endpoint=unix:///var/run/containerd/containerd.sock \\
--image-pull-progress-deadline=2m \\
--kubeconfig=/var/lib/kubelet/kubeconfig \\
--network-plugin=cni \\
--register-node=true \\
--v=2
```

```sh
$ ps -aux | grep kubelet

root 2095 1.8 2.4 960676 98788 ? Ssl 02:32 0:36 /usr/bin/kubelet --bootstrap-
kubeconfig=/etc/kubernetes/bootstrap-kubelet.conf --kubeconfig=/etc/kubernetes/kubelet.conf --config=/var/lib/kubelet/config.yaml --cgroup-driver=cgroupfs --cni-bin-dir=/opt/cni/bin --cni-conf-dir=/etc/cni/net.d --network-plugin=cni
```

##### Container runtime

To run the containers, each compute node has a container runtime engine. Docker is one example, but Kubernetes supports other Open Container Initiative-compliant runtimes as well, such as rkt and CRI-O.

##### Kube-Proxy

Each compute node also contains kube-proxy, a network proxy for facilitating Kubernetes networking services. The kube-proxy handles network communications inside or outside of your cluster—relying either on your operating system’s packet filtering layer, or forwarding the traffic itself.

![Kube-Proxy](Image/CKA-10.png)

Manual SetUp:

```sh
$ wget https://storage.googleapis.com/kubernetes-release/release/v1.13.0/bin/linux/amd64/kube-proxy
ExecStart=/usr/local/bin/kube-proxy \\
--config=/var/lib/kube-proxy/kube-proxy-config.yaml
Restart=on-failure
RestartSec=5
```

Kubeadm SetUp:

```sh
$ kubectl get pods -n kube-system
NAMESPACE NAME READY STATUS RESTARTS AGE
kube-system coredns-78fcdf6894-hwrq9 1/1 Running 0 16m
kube-system coredns-78fcdf6894-rzhjr 1/1 Running 0 16m
kube-system etcd-master 1/1 Running 0 15m
kube-system kube-apiserver-master 1/1 Running 0 15m
kube-system kube-controller-manager-master 1/1 Running 0 15m
kube-system kube-proxy-lzt6f 1/1 Running 0 16m
kube-system kube-proxy-zm5qd 1/1 Running 0 16m
kube-system kube-scheduler-master 1/1 Running 0 15m
kube-system weave-net-29z42 2/2 Running 1 16m
kube-system weave-net-snmdl 2/2 Running 1 16m
```

```sh
$ kubectl get daemonset -n kube-system
NAME DESIRED CURRENT READY UP-TO-DATE AVAILABLE NODE SELECTOR AGE
kube-proxy 2 2 2 2 2 beta.kubernetes.io/arch=amd64 1h
```

[Refer Pod, Deployment, Services, Replicaset etc.,](#kubernetes-beginners) and [Github-Link](https://bhavyasree.github.io/CKAD/01.kubernetes-architecture)

### Scheduling

#### Manual Scheduling

![Scheduling](Image/CKA-11.png)

The Kubernetes Scheduler is a core component of Kubernetes. In this tutorial we will discuss about different ways of Kubernetes manual scheduling a POD on a node. What you do when you don’t have a scheduler in your cluster? You probably don’t want to rely on built in scheduler and instead want to schedule the PODs yourself.

The scheduler goes through the all PODs and looks for those that don’t have this property set. Those are the candidates for the scheduling. It then identifies the right node for the POD by running the scheduling the algorithm. Once identified, it schedules the POD on the node by setting the nodeName property to the name of the node by creating the binding object.

**No Scheduler**:
If there is no scheduler to monitor and schedule a node what happens? The pods continue to the in a pending stage.

So what can we do about it. We can manually assign the PODs to nodes yourself. Without a scheduler the easiest way to schedule a POD is to simply set the nodeName field to the name of the node in your POD specification file while creating the POD. The POD then gets assigned to the specified node.

![Scheduling](Image/CKA-12.png)

What if the POD is already created and you want to assign POD to a node. Kubernetes wont’ allow you to modify the nodeName property of a POD. So another way to assign existing POD to node is to create a binding object and sent a post request to the PODs binding API. This is what the actual scheduler does.

![Scheduling](Image/CKA-13.png)

In the binding object we specify the target node with a name of the node. Then send a post request to the PODs binding API by setting data property in the JSON format. Here you must convert your YAML to its equivalent JSON format.

curl --header "Content-Type:application/json" --request POST --data http://$SERVER/api/v1/namespaces/default/pods/$PODNAME/binding/

#### Labels and Selectors

Labels and Selectors are standard method to group things together. For example, we have set of different species and a user wants to be able to filter them based on different criteria. Such as based on their class or kind or by their color.

![Labels and Selector](Image/CKA-14.png)

And not just group, you want to be able to filter them based on criteria. Such as all blue animals, or with multiple criteria such as everything green that is also a bird. Whatever the classification may be you need ability to prove things together and filter them based on your needs.

The best way to do that with specific Labels. Labels are properties attached to each item. You add properties for each item. So you add properties to each item for their class, kind and color.

![Labels and Selector](Image/CKA-15.png)

Selectors are the filters of these items. For example, when you say class=Mammal We get a list of Mammals and when you say color is green then we get the green mammal.

We use labels and selectors every where. Such as keywords you tagged in YouTube videos or blogs that have users filter and find the right content. We can see labels in online store that help you add different kinds of filters to view your products.

Now coming to how are labels and selectors used in Kubernetes. We have created a lot of different types of objects in Kubernetes. PODs, Services, ReplicaSet, Deployments etc.

For Kubernetes all of these are different objects. Over time you may deploy 100’s or 1000’s of these objects in your cluster. Then you will need a way to filter and view different objects by different categories. Such as to group objects by their type.

![Labels and Selector](Image/CKA-16.png)

also you can group by their application or group by their functionality. What ever it may be you can group and select objects using labels and selectors.

So how exactly do we specify labels in Kubernetes.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: simple-webapp
  labels: 
    app: App1
    function: Front-end
spec:
  containers:
    - name: simple-webapp
      image: simple-webapp
      ports:
        - containerPort: 8080
```

Once POD is created you can select the POD using the labels by following command.

```sh
$ kubectl get pods --selector app=App1
NAME                READY   STATUS      RESTARTS   AGE
simple-webapp       1/1     Running        0       24s
```

Kubernetes objects use labels and selectors internally to connect different objects together. For example, to create a ReplicaSet consisting of three different PODs. We first create label the POD definition and use selector in a ReplicaSet to group the PODs.

Note

1. The labels defined under templates section are the labels configured on the POD.
2. Labels defined under top metadata section are the labels of ReplicaSet.

#### Taint and Toleration

In this tutorial we well discuss about Taints and Tolerations, — another feature for the advanced Pod scheduling in Kubernetes.

The taints and toleration are all about the relationship between the pod and node. Taints and Toleration will tell what pods can be placed on what nodes.

The concept of Taints and Tolerations are can be a bit confusing for Kubernetes beginners. Taints and tolerations work together to make sure that pods are not scheduled onto inappropriate nodes.

Traints and tolerations are mainly used to set restrictions on what PODs can be scheduled on a node.

Let us start with the simple cluster with 3 worker nodes. The nodes are named 1, 2 and 3. We also have a set of PODs that are to be deployed on these nodes. Let’s call them as A, B, C and D.

![taint and toleration](Image/CKA-17.png)

When the PODs are created Kubernetes scheduler tries to place these PODs on the available worker node. As of now, there are no restrictions or limitations and asserts the scheduler places the PODs across all of the nodes to balance them out equally.

![taint and toleration](Image/CKA-18.png)

Now let’s assume that we have dedicated resources at Node 1 for particular use case or application. So here we would like only those PODs that belongs to this application to be placed on Node 1.

First we prevent all PODs from being placed on the node by placing a taint on the node. Let’s call it blue. By default PODs have no toleration which means unless specified otherwise none of the PODs can tolerate any taint.

![taint and toleration](Image/CKA-19.png)

So in this case none of the PODs can be placed on Node 1 as none of them can tolerate the taint blue. This solves half of our requirement.

No unwanted PODs are going to be placed on this Node. The other half is to enable certain PODs to be placed on this node. For this we must specify which PODs are tolerant to this particular taint.

In our case we would like to allow only POD D to be placed on this node. So we add a toleration to POD. POD D is now tolerant to blue. So when the scheduler tries to place this POD on Node 1 it goes through. Node 1 can now only accept PODs that can tolerate the taint blue.

![taint and toleration](Image/CKA-20.png)

So with all the taints and toleration in place. This is how the PODs would be scheduled.

The scheduler tries to place POD A on Node 1 due to the taint it is thrown off and it goes to Node 2, the scheduler then tries to place POD B on Node 1 but again due to the taint it is thrown off and it is placed on Node 3 which happens to be the next free node. The scheduler then tries to place POD C on Node 1 but again due to the taint it is thrown off and ends up on Node 2. Finally the scheduler tries to place POD D on Node 1, since the POD is tolerant to the Node 1.

Note:

Taints are set on nodes and toleration are set on PODs. So how do we do this.

How to set a Taint on the node

Syntax:

```sh
kubectl taint nodes [NODE_NAME] [KEY]=[VALUE]:[TAINT-EFFECT] 
```

Taint effects define how nodes with a taint react to Pods that don’t tolerate it. There are 3 types of taint effects,

1. NoSchedule: Instructs Kubernetes scheduler not to schedule any new pods to the node unless the pod tolerates the taint.
2. PreferNoSchedule: The PreferNoSchedule taints prevents scheduling Pods on a node, BUT, if no suitable untainted node can be found then it WILL schedule the Pod on that node.
3. NoExecute: Which means that new pods will not be scheduled on the node and the existing PODs on the node if any will be evicted if they don’t tolerate the taint.

These PODs may have been scheduled on node before the taint was applied to the node.

```sh
kubectl taint nodes node1 app=blue:NoSchedule
```

Now create tolarations on PODs

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: myapp-pod
spec:
  containers:
  - name: nginx
    image: nginx
  tolerations:
  - key: "app"
    operator: "Equal"
    value: "blue"
    effect: "NoSchedule"
```

To remove the taint, you have to use the [KEY] and [EFFECT] ending with [-].

Syntax:

```sh
kubectl taint nodes <node-name> [KEY]:[TAINT-EFFECT]-
```

```sh
kubectl taint nodes node1 app=blue:NoSchedule-
```

#### Node Selectors

In this tutorial we will discuss about Node Selectors in Kubernetes. Node Selector is one of the forms of node selection constraint. Hope I kept it simple as possible to understand.

This is a simple POD scheduling feature that allows scheduling a POD onto a node whose labels match the Node Selector labels specified by the user. Let us start with a simple example.

We have a 3 node cluster of which two are smaller nodes with lower hardware resources and one of them is a larger node configured with higher resources. We have different kinds of workloads running in our cluster.

![Node Selector](Image/CKA-21.png)

You would like to dedicate the data processing workloads that require higher horsepower to the larger node as that is the only node that will not run out of resources in case the job demand extra resources.

However, in the current default setup, any PODs can go to any nodes.

![Node Selector](Image/CKA-22.png)

So POD C in this case may very well end up on nodes 2 or 3 which is not desired. To solve this we can set a limitation on the PODs. So that they only run on particular nodes. There are 2 ways to do this.

The first is using Node Selectors which is the simple and easier method. For this we look at the POD definition file we created in earlier tutorials. This file has a simple definition to create a POD with a data processing image.

To run on the larger nodes, we add a new property called nodeSelector to the spec section and specify the size as large.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: myapp-pod
spec:
  containers:
    - name: data-processor
      image: data-processor
  nodeSelector:
      size: Large
```

In the about configuration file, where did the size Large come from and how does Kubernetes know which is the large node?

The key value pair of size and Large are in fact labels assigned to the nodes the scheduler uses these labels to match and identify the right node to place the PODs on.

To use labels in a nodeSelector like this, we must have first labelled our nodes prior to creating this POD. So let us see how we can label the nodes.

Syntax

```sh

kubectl label nodes <node-name> <label-key>:<label-value>

kubectl label nodes node-1 size=Large

```

Now we have labeled the node. Now when the POD is created it is placed on Node 1 as desired.

Node Selectors served our purpose but it has limitations. We used a single label and selector to achieve our goal here. But what if our requirement is much more complex.

For example, we would like to say something like place the POD on a large or medium node or something like place the POD on any nodes that are not small. You cannot achieve this using Node Selectors.

For this node affinity and anti affinity features were introduced and we will look at that next tutorial.

#### Node Affinity

In this tutorial we will discuss about Node Affinity in Kubernetes. In simple words this allows you to tell Kubernetes to schedule pods only to specific subsets of nodes. Hope I kept it simple as possible to understand.

It is recommended that you should understand the Node Selectors and Taints and Tolerations concepts before proceeding further.

The primary purpose of this feature is to ensure that PODs are hosted on particular nodes. They are 3 ways to place a POD on a specific node,

1. Node Selectors
2. Taints and Tolerations
3. Node Affinity

But each method has its own advantages and disadvantages. So based on the use case we can use any one of the above methods to place POD on a node.

Node Affinity is an advanced feature in Kubernetes when compared to the other two above methods.

With the Node Selectors we cannot provide advanced expressions like OR or NOT with node selectors. This feature provide us advanced capabilities to limit POD placement on specific nodes.

Will now look like this with this feature. Although both Node Selectors and Node affinity does exactly the same thing place the POD on the large node.

Let us look at the it a bit closer. Under spec we have affinity and then nodeEffinity under that. And then we have a property that looks like a sentence called requiredDuringSchedulingIgnoredDuringExecution, then we have the node selector terms that is an array and that is where we will specify the key and value pairs.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: myapp-pod
spec:
  containers:
    - name: data-processor
      image: data-processor
   affinity:
   nodeAffinity:
     requiredDuringSchedulingIgnoredDuringExecution:
       nodeSelectorTerms:
         - matchExpressions:
           - key: size
             operator: In
             values:
               - Large
```

They key value pairs are in the form key, operator and values. Where the operator is In. The In operator ensures that the POD will be placed on a node whose label size has any value in the list of values specified here.

Here in this case it is just one called Large. If you think your POD could be placed on a large or a medium node, you could simply specify add the value to the list of values

```yaml
spec:
  containers:
    - name: data-processor
      image: data-processor
   affinity:
   nodeAffinity:
     requiredDuringSchedulingIgnoredDuringExecution:
       nodeSelectorTerms:
         - matchExpressions:
           - key: size
             operator: In
             values:
               - Large
               - Medium
```

![Node Afinity](Image/CKA-23.png)

You could use the NOT IN operator to say something like size not in small

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: myapp-pod
spec:
  containers:
    - name: data-processor
      image: data-processor
   affinity:
   nodeAffinity:
     requiredDuringSchedulingIgnoredDuringExecution:
       nodeSelectorTerms:
         - matchExpressions:
           - key: size
             operator: NotIn
             values:
               - Small
```

When the PODs are created, these rules are considered and the PODs are placed onto the right nodes. But what if node affinity could not match a node with a given expression?

In this case what if there are no nodes with a label called size. Say we had the labels and the PODs are scheduled. What if someone changes the label on the node at a future point in time. Will the POD continue to stay on the node?

All of this is answered by the long sentence like property under this feature. which happens to be the type of node affinity. The type of this feature defines the behavior of the scheduler with respect to node affinity and stages in the life cycle of the POD.

There are two types of available node affinity types available in Kubernetes.

- **requiredDuringSchedulingIgnoredDuringExecution**
- **preferredDuringSchedulingIgnoredDuringExecution**
When considering this feature there are two stages in the life cycle of pod.

1. During Scheduling
2. During Execution

During Scheduling:

During Scheduling is the state where a pod does not exist and is created for the first time. If rules are available it will be scheduled into a particular node, we are clear about this. What if matching label are not available, for example, we forgot to label nodes. That’s where the type of Node Affinity used comes into play.

Type 1 node affinity of requiredDuringScheduling, if you select required type, the scheduler will mandate that pod is placed on node with given node affinity rules, if cannot find one, it cannot schedule. This type is used where the placement of pod is crucial, if matching node does not exist, the POD will not be schedule.

Type 2 node affinity of preferredDuringScheduling, it helps when the pod placement is less importance than running a workloads, in this type we choose preferred type, here scheduler will simply ignore node affinity rules and place the pod any available nodes.

DuringExecution

When pod has been running and a change is made in the environment that effects node Affinity, such changes like labels of nodes. For example say an administrator removed the label Size=Large from the node. Now what happens to pods that are running on that node? In this case again we got type 1 and type 2 both are at ignored phase in present node affinity types.

Type1 and type 2 that means pods will continue to run on the nodes. Any changes in node affinity rules will not impact them once they are scheduled.

There are two planned types

- **requiredDuringSchedulingRequiredDuringExecution**
- **preferredDuringSchedulingRequiredDuirngExecution.**

In these types only change comes in execution part phase, required is added that means whenever there is change, pod will be evicted or terminated.

#### Taint and Toleration vs Node Affinity

For example we have 3 nodes and 3 PODs each in 3 colors green, red and blue. The ultimate goal is to place the green POD in the green node, red POD in the red node and blue POD in the blue node.

We are sharing same Kubernetes cluster with other teams. So there are other PODs in the cluster as well as other nodes.

![T&T Node Afinity](Image/CKA-24.png)

Here we don’t want any other PODs to be placed on our 3 nodes, and also don’t want any out PODs to be placed on other nodes.

Let’s first try to solve this problem using taints and tolerations. We apply a taint to the nodes marking them with their colors. Now we apply tolerations on the PODs to tolerate the respective colors.

When the PODs are now created, the nodes ensure only accept the PODs with the right toleration. So blue POD inserted on blue node, green POD inserts green node. How ever taints and tolerations doesn’t guarantee that the PODs only prefer these nodes. So the red POD inserts one of the other node that don’t have taints and tolerations. This is not desired.

![T&T Node Afinity](Image/CKA-25.png)

Now let’s try to solve same problem using Node affinity. With node affinity we first labeled the nodes with their respective colors, we then set node selectors on the PODs to tie the PODs to the nodes. So PODs will be placed on right nodes.

However that doesn’t guarantee that other PODs are not placed on our nodes. In this case there is a chance that one of the other PODs may end up on our nodes. This is not something we desire.

![T&T Node Afinity](Image/CKA-26.png)

As such a combination of taints & tolerations and node affinity rules can be used together to completely dedicate nodes for specific PODs. We first use taints and tolerations to prevent other PODs from being placed on our nodes and then we use node affinity to prevent our PODs from being placed on other nodes.

#### Resource Requirements and Limits

![R&R&L](Image/CKA-27.png)

Let us look at a 3 node Kubernetes cluster. Each node has a set of CPU, memory and Disk resources available. Every POD consumes a set of resources. In this case 2 CPU’s, one memory and some disk space.

Whenever a POD is placed on a node, it consume resources available to that node. As we have discussed before, it is the Kubernetes scheduler that decides which node a POD goes to. The scheduler takes into consideration, the amount of resources required by a POD and those available on the nodes.

In this case, the scheduler schedules a new POD on node 2. If the node has no sufficient resources, the scheduler avoids placing the POD on that node. Instead places the POD on one where the sufficient resources are available.

If there is no sufficient resources available on any of the node, Kubernetes holds back scheduling the POD, and you will see the POD in pending state.

Let us now focus on the resource requirements for each POD. What are these blocks and what are their values?

Resource Requests:

By default, Kubernetes assumes that a POD or a container within a POD requires 0.5 CPU and 256 Mebibyte of memory. This is known as the resource request for a container. The minimum amount of CPU or memory requested by the container.

![R&R&L](Image/CKA-28.png)

When the scheduler tries to place the POD on a node, it uses these numbers to identify a node which has sufficient amount of resources available.

Now if you know that your application will need more than these you can modify these values by specifying them in your POD or deployment definition files.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-webapp
  labels:
    name: my-webapp
spec:
  caontainers:
    - name: my-webapp
      image: my-webapp:2.0.0
      ports:
        - containerPort : 8080
      resources:
        requests:
          memory: "512Mi"
          cpu: 1
```

Resource Limits:

Let’s now look at a container running on a node. In the docker world a docker container has no limit to the resources it can consume on a node. Say a container starts with 1 vCPU on a node, it can go up and consume as much resource as it requires.

However you can set a limit for the resource usage on these PODs by default. Kubernetes sets a limit of 1 vCPU to containers. So if you don’t specify explicitly, a container will be limited to consume only 1 vCPU from the Node.

The same goes with memory. By default, Kubernetes sets a limit of 512 Mebibyte on containers. If you don’t like the default limits, you can change them by adding limit section under the resources section in you POD definition file.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-webapp
  labels:
    name: my-webapp
spec:
  caontainers:
    - name: my-webapp
      image: my-webapp:2.0.0
      ports:
        - containerPort : 8080
      resources:
        requests:
          memory: "512Mi"
          cpu: 1 
        limits:
          memory: "1Gi"
          cpu: 2
```

Please note that the limits and requests are set for each container within the POD.

Exceed Limits:

What happens when a POD tries to exceed resources beyond its specified limit.

In case of the CPU, Kubernetes throttles the CPU so that it doesn’t go beyond the specified limit. A container cannot use more CPU resources than its limit.

However, this is not the case with memory. A container can use more memory resources than its limit. So if a POD tries to consume more memory than its limit constantly, the POD will be terminated.

#### Editing Pods and Deployments

Edit a POD
Remember, we CANNOT edit specifications of an existing POD other than the below.

**spec.containers[*].image**
**spec.initContainers[*].image**
**spec.activeDeadlineSeconds**
**spec.tolerations**
For example we cannot edit the environment variables, service accounts, resource limits of a running pod. But if you really want to, you have 2 options:

Run the `kubectl edit pod <pod-name>` command. This will open the pod specification in an editor (vi editor). Then edit the required properties. When you try to save it, you will be denied. This is because you are attempting to edit a field on the pod that is not editable.
A copy of the file with your changes is saved as a yaml file in a temporary location.
We can then delete the existing pod by running the command: `kubectl delete pod <pod-name>`

Then create a new pod with changes using the temporary file `kubectl create -f <newly created yaml file with changes>`

like

```sh
kubectl create -f /tmp/kubectl-edit-ccvrq.yaml
```

The second option is to extract the pod definition in YAML format to a file using the command `kubectl get pod <pod-name> -o yaml > my-new-pod.yaml`
Then make the changes to the exported file using an editor (vi editor). Save the changes vi `my-new-pod.yaml`
Then delete the existing pod `kubectl delete pod <pod-name>`
Then create a new pod with the edited file `kubectl create -f my-new-pod.yaml`

Edit Deployments

With Deployments we can easily edit any field/property of the POD template. Since the pod template is a child of the deployment specification, with every change the deployment will automatically delete and create a new pod with the new changes. So if we are asked to edit a property of a POD part of a deployment you may do that simply by running the command

```sh
kubectl edit deployment my-deployment
```

#### Daemon Sets

Every node will have a copy of the pod. When nodes are added to the cluster, PODs are added to them and when nodes are removed from the cluster, the PODs are removed. If we delete a DaemonSet it will clean up the PODs it created.

So far we have deployed various PODs on different nodes in our cluster. With the help of replica sets and deployments we made sure multiple copies of our applications are made available across various different worker nodes.

![Daemon](Image/CKA-29.png)

Daemon sets are like replica sets, as in it helps you deploy multiple instances of POD. But it runs one copy of your POD on each node in your cluster.

![Daemon](Image/CKA-30.png)

Whenever a new node is added to the cluster a replica of the POD is automatically added to that node.

![Daemon](Image/CKA-31.png)

And when the node is removed from the cluster then the POD is automatically removed.

![Daemon](Image/CKA-32.png)

The daemon sets ensure that one copy of the POD always present in all nodes in the cluster.

Use cases of daemon sets:

For example you would like to deploy a monitoring agent or log collector on each nodes in the cluster. So you can monitor your cluster better. Daemon set is perfect for that as it can deploy your monitoring agent in the form of a POD in all the nodes in the cluster.

Then, you don’t have to worry about adding/removing monitoring agents from these nodes when there are changes in your cluster. As the daemon set will take care of that for you.

Kube proxy is one good use case of daemon sets. The kube proxy component can be deployed as a daemon set in the cluster.

DaemonSet definition:

Creating DaemonSet is similar to the ReplicaSet creation process. It has nested POD specification under the template section and selectors to link the daemon set to the PODs

```yaml
apiVersion: apps/v1
kind: DaemonSet
metadata:
  name: monitoring-daemon
spec: 
  template:
    metadata:
      labels: 
        app: monitoring-agent
    spec:
      containers:
        - name: monitoring-agent
          image: monitoring-agent
  selector:
    matchLabels:
      app: monitoring-agent
```

Once ready, create the daemon set using the following command.

```sh
kubectl create -f daemon-set-definition.yaml
```

Now, to view the created daemon set run the following command.

```sh
kubectl get daemonsets
```

And of course to view more details run the following command.

```sh
kubectl describe daemonsets monitoring-daemon
```

So, how does a daemon set work? How does it schedule PODs on each node? and how does it ensure that every node has a POD?

Now, If you were asked to schedule a POD on each node in the cluster, how would you do it?

Firstly, On each POD set the nodeName property in its specification before it is created, they automatically land on the respective nodes.

![Daemon](Image/CKA-33.png)

So, that’s how it is used to be until Kubernetes version v1.12. From v1.12 on wards the daemon set used the default scheduler and node affinity rules that we discussed in

#### Static pods

In this tutorial we will discuss about Static PODs in Kubernetes. Static pods are a type of pod that is not managed via Kube API Server and is directly bound to the Kubelet agent on the node.

The kubelet agent is responsible to watch each static Pod and restart it if it crashes.

The static Pods running on a node are visible on the API server but cannot be controlled by the API Server.

Real time example:

For example, As we already know the Kubelet relies on the Kube API server for instructions on what PODs to load on its node, which is based on a decision made by the Kube Scheduler which was stored in the ETCD data store.

What if there was no Kube API server, Kube Scheduler and no controllers and no ETCD cluster? What if there was no master at all, there were no other nodes and only single node alone not part of any cluster?

Well, the kubelet can manage a node independently. On this node we have kubelet installed and of course we have docker as well to run containers. There is no Kubernetes cluster. So there are no Kube API server or any thing like that.

Is there anything that Kubelet can do? Can it operate as an independent node? If so who would provide the instructions required to create PODs?

The one thing that the Kubelet knows to do is create PODs. But we don’t have an API server here to provide POD details.

By now we know that to create a POD you need the details of the POD in a POD definition file. But how do you provide a POD definition file to the Kubelet with out Kube API server?

You can configure the Kubelet to read the POD definition files from a directory on the server designated to store information about PODs. Place POD definition files in this directory.

The Kubelet periodically checks this directory for files, read this files and create PODs on the host. Not only does it create the POD it can ensure that the POD stays alive. If the application crashes, the kubelet attempts to restart it.

If you make a change to any of the file within this directory, the kubelet recreates the POD for those changes to take effect.

Kubelet will delete your POD automatically when you remove a file from this directory.

Static PODs:

The PODs that are created by the kubelet on its own without the interaction from the API server or rest of Kubernetes cluster components are known as Static PODs.

Remember you can only create PODs this way. You can’t create Replica Sets, Deployments or Services by placing a definition file in the designated directory.

The Kubelet works at a POD level and can only understand PODs. Which is why it is able to create static PODs this way.

So what is that designated folder and how do we configure it? It could be any directory on the host and location of that directory is passed in to the Kubelet.service as an option while running the service.

The option is named POD manifest path and here it is set to **/etc/Kubernetes/ manifests**.

![Static-Pods](Image/CKA-34.png)

There is also another way to configure this. Instead of specifying the option directly in the kubelet.service file, you could provide a path to another config file using the config option, and define the directory path as static POD path in that file.

![Static-Pods](Image/CKA-35.png)

`staticPodPath=/etc/kubernetes/manifests`

Once the static PODs are created, you can view them using docker ps command.

So, why not the kubectl command as we have been so far? Remember we don’t have the rest of the Kubernetes cluster. Kubectl utility works with the Kube API Server.

Since we don’t have an API server there is no kubectl utility. So we need to use docker command.

How does it work when the node is part of a cluster:

When there is an API server requesting the kubelet to create PODs. Can the kubelet create both kinds of PODs at the same time?

Well, the way the kubelet works is it can take in requests for creating PODs from different inputs.

- Through the POD definition files from the static PODs folder
- Through an HTTP API end point. (i.e., how the Kube API Server provides input to kubelet)

The Kubelet can create both kinds of PODs (Static PODs and the ones from the API Server).

If you run the `kubectl get pods` command on the master node, the Static PODs will be listed as any other POD. Well, how is that happen?

When the kubelet creates a Static POD, if it is part of a cluster, it also creates a mirror object in the Kube API Server. What we see from the Kube API Server is just a read only mirror of the POD. You can view details about the POD, but you cannot edit or delete it like the usual PODs.

You can only delete them by modifying the files from the nodes manifest folder. Note that the name of the POD is automatically appended with the node name.

Why do we use Static PODs:

Since static PODs are not dependent on the Kubernetes control plane, you can use static PODs to deploy the control plane components itself as PODs on node.

#### Multiple Scheduler

We mainly discuss on different ways of manually scheduling a POD on a node, how to view scheduler related events.

As we know, the default scheduler has an algorithm that describes PODs across nodes evenly as well as takes into consideration, the various conditions we specify through taints and tolerations and node affinity etc.

But what if none of these satisfies your needs?

Say you have a specific application that requires its components to be placed on nodes after performing some additional checks.

So you decide to have your own scheduling algorithm to place PODs on nodes. So that you can add your own custom conditions and checks in it.

Kubernetes is highly extensible. You can write your own Kubernetes scheduler program, package it and deploy it as the default scheduler or an additional scheduler in the Kubernetes cluster.

That way all of the other applications can go through the default scheduler, however one specific application can use your custom scheduler.

Your Kubernetes Cluster can have multiple schedulers at the same time. When creating a POD or a deployment you can instruct Kubernetes to have the POD scheduled by a specific scheduler.

#### Configure K8s Scheduler

We need to download the kube scheduler binary and run it as a service with a set of options.

```sh
wget https://storage.googleapis.com/kubernetes-release/release/v1.18.6/bin/linux/amd64/kube-scheduler
```

One of the option is scheduler name. If not specified it assumes in name of default scheduler.

```sh
sudo vi /etc/systemd/system/kube-scheduler.service 

[Service]
ExecStart=/usr/local/bin/kube-scheduler \\
  --config=/etc/kubernetes/config/kube-scheduler.yaml \\
  --scheduler-name=default-scheduler
```

To deploy an additional scheduler, you can use the same kube-scheduler binary or use one that you might have built for yourself, which makes more sense.

In this case we are going to use same binary to deploy the additional scheduler. This time we set the scheduler name to a custom name.

```sh
sudo vi /etc/systemd/system/my-custom-kube-scheduler.service 

[Service]
ExecStart=/usr/local/bin/kube-scheduler \\
  --config=/etc/kubernetes/config/kube-scheduler.yaml \\
  --scheduler-name=my-custom-kube-scheduler
```

This is important to differentiate the two schedulers and this is the name that we will be specifying in the POD. definition file later on.

Lets a take a look at how it works with the kubeadm tool.

The kubeadm tool deploys the scheduler as a POD. You can find the definition file. It uses under the manifest folder.

```yaml
$ cat /etc/kubernetes/manifests/kube-scheduler.yaml

apiVersion: v1
kind: Pod
metadata:
  name: kube-scheduler
  namespace: kube-system
spec:
  containers:
  - command: 
    - kube-scheduler
    - --address=127.0.0.127
    - --kubeconfig=/etc/kubernetes/scheduler.--kubeconfig
    - --leader-elect=true
    image: k8s.gcr.io/kube-scheduler-amd64:v1:18.6
    name: kube-scheduler
```

Please note that I have removed all the other details from the file. We only focus on key parts of the configuration.

We can create a custom scheduler by making a copy of the same file, and by changing the name of the scheduler.

```yaml
$ cat /etc/kubernetes/manifests/my-custom-kube-scheduler.yaml

apiVersion: v1
kind: Pod
metadata:
  name: kube-scheduler
  namespace: kube-system
spec:
  containers:
  - command: 
    - kube-scheduler
    - --address=127.0.0.127
    - --kubeconfig=/etc/kubernetes/scheduler.--kubeconfig
    - --leader-elect=true
    - --scheduler-name=my-custom-kube-scheduler
    image: k8s.gcr.io/kube-scheduler-amd64:v1:18.6
    name: kube-scheduler
```

Finally an important option to look here is leader-elect option. The leader- elect option is used when you have multiple copies of the scheduler running on different master nodes.

If multiple copies of the same scheduler are running on different nodes, only one can be active at a time. That’s where the leader-elect option helps in choosing a leader who will lead scheduling activities.

To get multiple schedulers working, you must either set the leader-elect option to false, in case where you don’t have multiple masters.

In case you do have multiple masters, you can pass in an addition parameter to set a lock object name.

```yaml
cat /etc/kubernetes/manifests/my-custom-kube-scheduler.yaml

apiVersion: v1
kind: Pod
metadata:
  name: kube-scheduler
  namespace: kube-system
spec:
  containers:
  - command: 
    - kube-scheduler
    - --address=127.0.0.127
    - --kubeconfig=/etc/kubernetes/scheduler.--kubeconfig
    - --leader-elect=true
    - --scheduler-name=my-custom-kube-scheduler
    - --lock-object-name=my-custom-kube-scheduler
    image: k8s.gcr.io/kube-scheduler-amd64:v1:18.6
    name: kube-scheduler
```

Once done, create a POD using the kubectl create command. Run the get pods command in the kube-system name space and look for the new custom scheduler.

```sh
kubectl create -f /etc/kubernetes/manifests/my-custom-kube-scheduler.yaml
kubectl get pods --namespace=kube-system
```

Make sure your custom scheduler pod is running state.

The next step is to configure a new POD or a deployment to use the new scheduler.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: nginx
spec:
  containers:
    - name: nginx-container
      image: nginx
      
  schedulerName: my-custom-kube-scheduler
```

When the POD is created, the right scheduler picks it up to schedule. If the scheduler was not configured correctly, then the POD will continue to remain in Pending state.

So how do we know which scheduler picked up? View the events using the kubectl get events command and look for the scheduled events.

### Logging and Monotoring

#### Monitor Cluster Components

So how do you monitor resource consumption on Kubernetes? or most importantly what would you like to monitor?

I would like to know, node level metrics such as the number of nodes in the cluster, how many of them are healthy as well as performance metrics such as CPU, memory, disk and network utilization.

As well as POD level metrics such as the number of PODs, and performance metrics of each POD such as CPU, memory consumption on them.

So we need a solution that will monitor these metrics store them and provide analytics around this data.

As of this tutorial, Kubernetes does not come with a full featured built-in monitoring solution.

However, there are a number of open-source solutions available today, such as the Metrics server, Prometheus, Elastic stack, and proprietary solutions like OpsRamp, Datadog and dynatrace.

Heapster vs Metrics Server
Heapster is the one of the original projects that enabled monitoring and analysis feature for Kubernetes.

You will see a lot of reference online when you look for reference architecture on monitoring Kubernetes.

However, Heapster is now deprecated and a slimmed down version was formed known as the Metric Server.

You can have one metrics server per Kubernetes cluster. The metric server retrieves metrics from each of the Kubernetes nodes and PODs, aggregates them and stores them in memory.

Note that the metric server is only an in-memory monitoring solution and doesn’t store the metrics on the disk and as a result you cannot see historical performance data.

For that you must rely on one of the advanced monitoring solutions we discussed earlier in this tutorial.

So how are the metrics generated for the PODs on these nodes?

Kubernetes runs an agent on each node known as the Kubelet, which is responsible for receiving instructions from the Kube API Server and running PODs on the nodes.

The Kubelet also contains a sub component known as cAdvisor or Container Advisor. cAdvisor is responsible for retrieving performance metrics from PODs, and exposing them through the Kubelet API to make the metrics available for the Metric Server.

![L&M](Image/CKA-36.png)

- Metrics Server

If you are using minikube for your local cluster, then run the following command.

```sh
minikube addons enable metrics-server
```

For all other environments deploy the metric server by cloning the metric server deployment files from the git hub repository and then deploy the required components.

Once Metric Server processed cluster performance can be viewed by following command.

```sh
kubectl top node
NAME          CPU(cores)   CPU%   MEMORY(bytes)   MEMORY%  
kube-master    1032m        12%    2917Mi          47%  
kube-node-01   540m         5%     1897Mi          27%
kube-node-02   102m         2%     1012Mi          11%  
```

This provides the CPU and Memory consumption of each of the nodes. Use the following command to view performance metrics of PODs in Kubernetes.

```sh
kubectl top pod
NAME                          CPU(cores)   MEMORY(bytes)   
redis                         5m           25Mi
nginx                         9m           52Mi
```

#### Manage Application Logs

In real time applications development, we may get number of problems or bugs or exceptions while executing or testing the applications.

To identify the problems and their locations then we have to trace the applications flow of execution.

Logs will help us to understand data flow through applications, as well as spot when and where errors are occurring.

Let us start with logging in docker. I run a docker container called my-webapp-events and all that it does is generate random events simulating my web server.

```sh
docker run hub.waytoeasylearn.com/my-webapp-events:1.0.0
[2020-10-29 11:25:15,561] INFO in event-simulator: USER1 logged in
[2020-10-29 11:24:32,066] INFO in event-simulator: USER3 is viewing page2
[2020-10-29 11:24:33,067] INFO in event-simulator: USER1 is viewing page2
[2020-10-29 11:24:34,068] INFO in event-simulator: USER3 is viewing page1
[2020-10-29 11:24:35,069] INFO in event-simulator: USER3 is viewing page3
[2020-10-29 11:24:36,070] INFO in event-simulator: USER2 logged out
[2020-10-29 11:24:37,072] WARNING in event-simulator: USER5 Failed to Login as the account is locked due to MANY FAILED ATTEMPTS.
[2020-10-29 11:24:37,072] INFO in event-simulator: USER3 is viewing page2
[2020-10-29 11:24:38,074] INFO in event-simulator: USER4 is viewing page2
[2020-10-29 11:24:39,075] INFO in event-simulator: USER1 logged out
[2020-10-29 11:24:40,077] WARNING in event-simulator: USER7 Order failed as the item is OUT OF STOCK.
[2020-10-29 11:24:40,078] INFO in event-simulator: USER2 logged out
[2020-10-29 11:24:41,079] INFO in event-simulator: USER3 logged in
[2020-10-29 11:24:42,081] WARNING in event-simulator: USER5 Failed to Login as the account is locked due to MANY FAILED ATTEMPTS.
[2020-10-29 11:24:42,081] INFO in event-simulator: USER2 is viewing page2
[2020-10-29 11:24:43,081] INFO in event-simulator: USER3 logged out
[2020-10-29 11:24:44,082] INFO in event-simulator: USER2 is viewing page3
[2020-10-29 11:24:45,083] INFO in event-simulator: USER4 is viewing page3
[2020-10-29 11:24:46,085] INFO in event-simulator: USER3 logged out
```

These are events streamed to the standard output by my application.

Now, if I were to run the docker container in the background, in a detached mode using the -d option, I wouldn’t see the logs.

```sh
docker run -d hub.waytoeasylearn.com/my-webapp-events:1.0.0
```

If I wanted to view the logs, I could use following command

```sh
docker logs -f 50ab19a9548f
[2020-10-29 11:30:53,150] INFO in event-simulator: USER2 logged in
[2020-10-29 11:30:54,152] INFO in event-simulator: USER1 is viewing page2
[2020-10-29 11:30:55,152] INFO in event-simulator: USER4 is viewing page1
[2020-10-29 11:30:56,154] INFO in event-simulator: USER4 is viewing page3
[2020-10-29 11:30:57,155] INFO in event-simulator: USER3 is viewing page3
[2020-10-29 11:30:58,156] WARNING in event-simulator: USER5 Failed to Login as the account is locked due to MANY FAILED ATTEMPTS.
[2020-10-29 11:30:58,157] INFO in event-simulator: USER4 logged in
[2020-10-29 11:30:59,158] INFO in event-simulator: USER2 logged in
[2020-10-29 11:31:00,159] INFO in event-simulator: USER3 is viewing page1
[2020-10-29 11:31:01,161] WARNING in event-simulator: USER7 Order failed as the item is OUT OF STOCK.
[2020-10-29 11:31:01,161] INFO in event-simulator: USER2 logged out
[2020-10-29 11:31:02,162] INFO in event-simulator: USER2 is viewing page3
```

Here -f option helps us to see live logs of the container.

Now let’s back to the Kubernetes. We create a POD with the same docker image using the POD definition file.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-webapp-events-pod
spec:
  containers:
  - name: my-webapp-events
    image: hub.waytoeasylearn.com/my-webapp-events:1.0.0
```

Once the POD is running, we can view the logs using the following command.

```sh
kubectl logs -f my-webapp-events-pod
[2020-10-29 11:30:53,150] INFO in event-simulator: USER2 logged in
[2020-10-29 11:30:54,152] INFO in event-simulator: USER1 is viewing page2
[2020-10-29 11:30:55,152] INFO in event-simulator: USER4 is viewing page1
[2020-10-29 11:30:56,154] INFO in event-simulator: USER4 is viewing page3
[2020-10-29 11:30:57,155] INFO in event-simulator: USER3 is viewing page3
[2020-10-29 11:30:58,156] WARNING in event-simulator: USER5 Failed to Login as the account is locked due to MANY FAILED ATTEMPTS.
[2020-10-29 11:30:58,157] INFO in event-simulator: USER4 logged in
[2020-10-29 11:30:59,158] INFO in event-simulator: USER2 logged in
[2020-10-29 11:31:00,159] INFO in event-simulator: USER3 is viewing page1
[2020-10-29 11:31:01,161] WARNING in event-simulator: USER7 Order failed as the item is OUT OF STOCK.
[2020-10-29 11:31:01,161] INFO in event-simulator: USER2 logged out
[2020-10-29 11:31:02,162] INFO in event-simulator: USER2 is viewing page3
```

Here you can use -f option to stream the logs live just like the docker command.
Now these logs are specific to the container running inside the POD. As we discussed before, Kubernetes PODs can have multiple docker containers in them.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-webapp-events-pod
spec:
  containers:
  - name: my-webapp-events
    image: hub.waytoeasylearn.com/my-webapp-events:1.0.0
  - name: my-webapp-queue-listener
    image: hub.waytoeasylearn.com/my-webapp-queue:1.0.0
```

Now if you run the kubectl logs command with the POD name, which container’s log would it show?

If there are multiple containers within a POD then you must specify the name of the container explicitly in the command. Otherwise it would fail asking you to specify a name.

So in this case i will specify the name of the first container my-webapp-events and that prints the relevant logs.

```yaml
kubectl logs -f my-webapp-events-pod my-webapp-events
[2020-10-29 11:30:53,150] INFO in event-simulator: USER2 logged in
[2020-10-29 11:30:54,152] INFO in event-simulator: USER1 is viewing page2
[2020-10-29 11:30:55,152] INFO in event-simulator: USER4 is viewing page1
[2020-10-29 11:30:56,154] INFO in event-simulator: USER4 is viewing page3
[2020-10-29 11:30:57,155] INFO in event-simulator: USER3 is viewing page3
[2020-10-29 11:30:58,156] WARNING in event-simulator: USER5 Failed to Login as the account is locked due to MANY FAILED ATTEMPTS.
[2020-10-29 11:30:58,157] INFO in event-simulator: USER4 logged in
[2020-10-29 11:30:59,158] INFO in event-simulator: USER2 logged in
[2020-10-29 11:31:00,159] INFO in event-simulator: USER3 is viewing page1
[2020-10-29 11:31:01,161] WARNING in event-simulator: USER7 Order failed as the item is OUT OF STOCK.
[2020-10-29 11:31:01,161] INFO in event-simulator: USER2 logged out
[2020-10-29 11:31:02,162] INFO in event-simulator: USER2 is viewing page3
```

Conclusion:

There is a lot of nuance surrounding logging in Kubernetes. Although Kubernetes offers some basic built-in logging and monitoring functionality, it’s a far cry from a full-fledged logging solution.

To get the most out of Kubernetes logging, you’ll need an external log collection, analysis, and management tool like LogDNA, which is very easy to set up on Kubernetes distributions like IKS, where it is one of the officially supported logging solutions.

### Application Lifecycle Management

#### Rolling Updates and Rollbacks

Before we discuss at how we upgrade our application, lets try to understand rollout and versioning in a deployment.

When we first create a deployment, it triggers a rollout. A new rollout creates a new deployment revision. Lets call it as revision 1.

![ALM](Image/CKA-37.png)

In the future, when the application is upgraded meaning when the container version is updated to a new one. A new rollout is triggered and new deployment revision is created named version 2.

![ALM](Image/CKA-38.png)

This helps us keep track of the changes made to our deployment and enables us to roll back to a previous version of deployment if necessary.

We can see the status of our rollout by using following command.

```sh
kubectl rollout status deployment/myapp-deployment
```

To check the revisions and history of rollout, you can use following command.

```sh
kubectl rollout history deployment/myapp-deployment
```

The above command will show you the revisions and history of the deployment.

There are 2 types of deployment strategies. Say for example you have 5 replicas of your web application instance deployed.

One way to upgrade these to a newer version is to destroy all of these and then create newer versions of application instances. This means First destroy the 5 running instances and then deploy 5 new instances of the new application version.

![ALM](Image/CKA-39.png)

Rolling Updates and Rollbacks
The problem with this, as you can imagine is that during the period after the older versions are down and before any newer version is up. The application is down and inaccessible to users. This strategy is known as the recreate strategy and thankfully this is not the default strategy.

Rolling update
The second strategy is where we did not destroy all of them at once. Instead we take down the older version and bring up a newer version one by one. This way the application never goes down and the upgrade is seamless.

![ALM](Image/CKA-40.png)

Rolling Updates and Rollbacks
If you don’t specify a strategy while creating the deployment it will assume it to be rolling update. In other words rolling update is the default deployment strategy.

So how exactly do we update our deployment. When we say update, it could be different things such as updating our application version by updating the version of docker containers used, updating their labels or updating the number of replicas etc.

Since we have already have a deployment definition file it is easy for us to modify this file. Once we make the necessary changes, we run the following command to apply the changes. Once we run the above command, a new rollout is triggered and a new revision after deployment is created.

```sh
kubectl apply -f deployment-definition.yaml
```

But there is another way to do the same thing. You could use the following command to update the image of your application.

```sh
kubectl set image deployment/myapp-deployment nginx=nginx:1.7.1
```

But remember doing it this way will result in the deployment definition file having a different configuration. So you must be careful when using the same definition file to make changes in the future.

The difference between the recreate and rolling update strategies can also be seen when you view the deployments in detail by running the following command.

```sh
kubectl describe deployment myapp-deployment
```

You will notice when the recreate strategy was used, the events indicate that the old replica set was scaled down to zero first and then the new replica sets scaled up to 5.

However when the rolling update strategy was used the old replica set was scaled down one at a time, simultaneously scaling up the new replica set one at a time.

Upgrades:

Lets look at how a deployment performs an upgrade. When a new deployment is created say to deploy 5 replicas, it first creates a ReplicaSet automatically, which in turn creates a ReplicaSet automatically, which in turn creates the number of PODs required to meet the number of replicas.

When you upgrade your application, the Kubernetes deployment object creates a new replicaset under the hood and starts deploying the containers there.

At the same time, taking down the PODs in the old replica set following a rolling update strategy.

![ALM](Image/CKA-40.png)

This can be seen when you try to list the replicasets using the following command.

Here we see the old replicaset with 0 PODs and the new replicaset with 5 PODs.

Rollbacks:

Say for instance, once you upgrade your application you realize something is inferior right. Something is wrong with the new version of the build when you used to upgrade.

So you would like to roll back your update. Kubernetes deployments allow you to roll back to a previous revision. To undo a change, run the following command.

```sh
kubectl rollout undo deployment/myapp-deployment
```

Once you run the above command, the deployment will then destroy the PODs in the new replicaset and bring the older ones in the old replicaset. And your application is back to its older format. When you compare the output of the kubectl get replicasets command, before and after the rollback, you will be able to notice this difference.

#### Commands and Arguments

Say you were to run a docker container from an Ubuntu image. When we run the “**docker run ubuntu**” command, it runs an instance of Ubuntu image and exits immediately.

If you were to list the running containers you wouldn’t see the container running. If you list all containers including those that are stopped you will see that the new container you ran is in an exited state.

Now why is that? Unlike virtual machines, containers are not meant to host an operating system. Containers are meant to run a specific task or process. Such as to host an instance of a web server or application server or a database or simply carry out some kind of computation or analysis.

Once the task is complete, the container exits. A container only lives as long as the process inside it is alive.

If the web service inside the container is stopped or crashes the container exits. So who defines what process is run within the container?

If you look at the docker file for popular docker images like Nginx you will see an instruction called CMD which stands for command that defines the program that will be run within the container when it starts.

For the Nginx image it is the nginx command, for MySQL image it is the mysqld command.

What we tried to do earlier was to run a container with a plain Ubuntu operating system. Lets look at the docker file for this image you will see that it uses bash as the default command.

Now bash is not really a process like a web server or database server. It is a shell that listens for inputs from a terminal if it cannot find a terminal it exists.

When we ran the Ubuntu container, Docker created a container from the Ubuntu image and launched the bash program.

By default docker doesn’t attach a terminal to a container when it is run. And so the bash program doesn’t find the terminal and so it exits.

Since the process that was started when the container was created finished the container exits as well.

How do you specify a different command to start a container?
One option is to append a command to the docker run command and that way it overrides the default command specified within the image.

In our case, I run the docker run ubuntu command with the sleep 10 command as the added option.

```sh
docker run ubuntu sleep 10
```

This way when the container starts it runs the sleep program waits to 10 seconds and then exits. But how do we make that change permanent?

Say we want the image to always run the sleep command when it starts. You would then create create your own image from the base Ubuntu image and specify new command.

```dockerfile
FROM ubuntu

CMD sleep 10
```

There are different ways to specifying the command either the command simply as is in a shell form or in JSON array format like as follows.

```dockerfile
CMD ["sleep","10"]
```

But remember when you specify in a JSON array format, the first element in the array should be the executable.

Note that don’t specify the command and parameters together like “sleep 10”. The command and its parameters should be separate elements in the list.

So now I build my new image using docker build command and name it as ubuntu-sleeper. I could now simple run the docker run ubuntu-sleeper command and gets the same results.

```sh
docker build -t ubuntu-sleeper:1.0.0

docker run ubuntu-sleeper:1.0.0
```

It always sleep for 10 seconds and exits. But what if I wish to change the number of seconds it sleeps. Currently it hard coded to 10 seconds. As we discussed before, one option is to run the docker run command with the new command appended to it.

In this case sleep 20 and the command that will be run at startup will be sleep 20 but it doesn’t look very good.

```sh
docker run ubuntu-sleeper:1.0.0 sleep 20
```

The name of the image ubuntu-sleeper in itself that the container will sleep. So we shouldn’t have to specify the sleep command again.

Instead we would like it to be something like below

```sh
docker run ubuntu-sleeper 20
```

We only want to pass in the number of seconds the container should sleep and sleep command should be invoked automatically and this is where the ENTRYPOINT instructions comes into play.

```dockerfile
FROM ubuntu

ENTRYPOINT ["sleep"]
```

- ENTRYPOINT

The ENTRYPOINT instruction is like the CMD instruction as in you can specify the program that will be run when the container starts.

And whatever you specify on the command line, in this case 20 will get appended to the ENTRYPOINT (like sleep 20).

So the commands that will be run when the container starts is sleep 20. So that’s the different between ENTRYPOINT and CMD.

**In case of CMD instruction the command line parameters passed will get replaced entirely where as in case of ENTRYPOINT the command line parameters will get appended.**

Now in the second case what if we run the ubuntu-sleeper image command without appending the number of seconds? then the command at startup will be just sleep and you get the error that the operand is missing.

So, how do we configure a default value of the command? If one was not specified in the command line that’s where you would use ENTRYPOINT as well as the command instruction.

```dockerfile
FROM ubuntu

ENTRYPOINT ["sleep"]

CMD ["5"]
```

In this case the CMD instruction will be appended to the ENTRYPOINT instruction.

So at startup the command would be “sleep 5”, if you didn’t specify any parameters in the command line. If you did then that will override the CMD instruction.

Please note that, for this to happen you should always specify the ENTRYPOINT and CMD instructions in a JSON format.

Finally what if you feel you really want to modify the ENTRYPOINT during runtime, say from sleep to an imaginary sleep 2.0 command?

Well in that case you can override it by using the ENTRYPOINT option in the docker run command.

```sh
docker run --entrypoint sleep2.0 ubuntu-sleeper 30
```

In the Above, we crated a simple docker image that sleeps for a given number of seconds. We named it ubuntu-sleeper and we ran it using the following docker command.

```sh
docker run --name ubuntu-sleeper ubuntu-sleeper
```

By default it sleeps for 10 seconds. But we can override it by passing a command line argument.

```sh
docker run --name ubuntu-sleeper ubuntu-sleeper 20
```

We will now create a POD using this docker image. We start with a following POD definition file

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: ubuntu-sleeper-pod
spec:
  containers:
    - name: ubuntu-sleeper
      image: ubuntu-sleeper
```

Now if you need the container to sleep for 30 seconds as in the second command. How do you specify the additional argument in the POD definition file?

Anything that is appended to the docker run command will go into the “args” property of the POD definition file in the form of an array like as follows

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: ubuntu-sleeper-pod
spec:
  containers:
    - name: ubuntu-sleeper
      image: ubuntu-sleeper
      args: ["30"]
```

Let us try to relate that to the docker file we created earlier. The Dockerfile has an Entrypoint as well as a CMD instruction specified.

The Entrypoint is the command that is run at startup, and the CMD is the default parameter passed to the command.

```dockefile
FROM Ubuntu

ENTRYPOINT ["sleep"]

CMD ["10"]
```

With the args option in the POD definition file, we override the CMD instruction in the Dockerfile.

But what if you need to override the entrypoint? Say from sleep to sleep2.0 command.

In the docker world we would run the docker run command with the entry point option set to the new command.

```sh
docker run --name ubuntu-sleeper --entrypoint sleep2.0 ubuntu-sleeper 30
```

The corresponding entry in the POD definition file would be using a command field corresponds to entry point instruction in the Dockerfile.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: ubuntu-sleeper-pod
spec:
  containers:
    - name: ubuntu-sleeper
      image: ubuntu-sleeper
      command: ["sleep2.0"]
      args: ["30"]
```

So to summarize there are 2 fields that correspond to two instructions in the Dockerfile. The command field overrides the entrypoint instruction and the args field overrides the command instruction in the Dockerfile.

Remember it is not the command field that overrides the CMD instruction in the Dockerfile.

#### Env Variables

Environment variables define the external state of deployed services. These are particularly important because production grade applications do not run in single environments.

Applications deployed in these environments do not tend to work with the exact same configurations. Environment variables provide a way to specify parameters for deployed services that vary from environment to environment.

An example environment setup could have development, staging and production environments:

- Development

The development environment would be the first line of defense against bugs. Here, developers deploy their code and test any newly implemented features.

Any bugs found are dealt with before re-deploying for further testing. The process is iterated until the code is ready for the next stage of testing.

- Staging

Once developers are satisfied with their code and consider it fairly stable, it is then deployed to the staging environment for further testing. This is where Quality Assurance (QA) is performed.

Testers access the staging servers and ensure that the application works as it should. They run test cases to detect bugs and run performance tests to find areas that could be improved.

Any bugs or enhancements are reported back to the developers and the process is repeated until the code passes the staging phase.

- Production

Once the code has been thoroughly tested, it is then pushed to production where it is made available to end-users.

Kubernetes allows users to provide environment variables when defining Pods. A Pod definition generally looks like as following

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-web-app
spec:
  containers:
  - name: my-web-app-container
    image: my-web-app
    ports:
      - containerPort: 8080
    env:
      - name: APP_COLOR
        value: pink
```

Here env is an array. So every item under the env property start with a dash, indicating an item in the array. Each item has a name and a value property.

The name is the name of the environment variable made available within the container and the value is its value.

What we just discussed was a direct way of specifying the environment variables using a plain key value pair format.

However there are other ways of setting the environment variables such as using config maps and secrets.

- Configure Environment Variables

![ENV](Image/CKA-42.png)

The main different in this case is that instead of specifying value, we say valueFrom. And then a specification of configMap or secret.

We will discuss about configMaps and secrets in the next tutorials.

#### Secrets

Let us assume we have a simple python web application that connects to a MySQL database.

```py
import os 
from flask import Flask 

app = Flask(__name__)

@app.route("/")
def main():
    mysql.connector.connect(host="mysql", database="ashok", user="ashok", password="ashok123")
    
    return render_template("hellp.html", color=fetchcolor())
    
if __name__ == __main__:
    app.run(host="0.0.0.0", port="8080")
```

If you look closely into the code you will see the host name, user name and password hard coded. This is of course not good idea.

As we discussed in the previous tutorial, one option would be to move these values into a ConfigMap.

```yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: app-config
data:
  DB_HOST: mysql
  DB_USER: ashok
  DB_DATABASE: ashok
  DB_PASSWORD: ashok123
```

The ConfigMap stores configuration data in plain text format. So while it would be okay to move the host name, database and user name into ConfigMap. But it is definitely not the right place to store password in ConfigMap. This is where secrets coming.

Secrets are used to store sensitive information like passwords or keys. They’re similar to ConfigMap except that they’re stored in an encoded or hashed format.

As with ConfigMaps, there are 2 steps involved in working with secrets. First create the secret and second injected into POD.

There are 2 ways of creating a secret. The imperative way – without using secret definition file and the declarative way by using a secret definition file.

- Imperative method

With the imperative method, you can directly specify the key value pairs in the command line itself.

To create a secret of the given values, run the following command.

```sh
kubectl create secret generic <secret-name> --from-literal=<key>=<value>
kubectl create secret generic app-secret --from-literal=DB_HOST=mysql
```

If you wish to add additional key value pairs then simply specify the –from-leteral options multiple times

```sh
kubectl create secret generic app-secret --from-literal=DB_HOST=mysql --from-literal=DB_USER=ashok --from-literal=DB_PASSWORD=ashok123
```

However this will get complicated when you have too many configuration items. Another way to input configuration data is through a file.

```sh
kubectl create secret generic <secret-name> --from-file=app-secret.properties
kubectl create secret generic app-secret --from-file=<path-to-file>
```

- Declarative Approach

In this approach we create a definition file just like how we did for the ConfigMap. The file has apiVersion, kind, metadata and data.

```yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: app-secret
data:
  DB_HOST=mysql 
  DB_USER=ashok
  DB_PASSWORD=ashok123
```

However one thing we discussed about secrets was that used to store sensitive data and are stored in an encoded format.

Here we have specified the data in plain text which is not very safe. So while creating a secret with declarative approach you must specify the secret values in a hashed format.

So you must specify the data in an encoded form like as below,

```yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: app-secret
data:
  DB_HOST=bXlzcWw= 
  DB_USER=YXNob2s=
  DB_PASSWORD=YXNob2sxMjM=
```

But how do you convert the data from plain text to an encoded format? On a Linux host run the command echo -n followed by the text you are trying to convert, which is mysql in this case and pipe that to the base64 utility.

```sh
$ echo -n mysql | base64
bXlzcWw=

$ echo -n ashok | base64
YXNob2s=

$ echo -n ashok123 | base64
YXNob2sxMjM=
```

To view secrets run the following command

```sh
$ kubectl get secrets
NAME                        TYPE                                  DATA   AGE
default-token-kdm9m         kubernetes.io/service-account-token   3      8h
app-secret                  Opaque                                3      2h
```

Above command lists the newly created secret along with another secret previously created by Kubernetes for its internal purpose.

To view more information on the newly created secret, run the following command.

```sh
kubectl describe secrets
```

The above command shows the attributes in the secret. But hides the value themselves. To view the values as well, run the following command.

```sh
kubectl get secret app-secret -o yaml
```

The above command will display YAML format. You can now see the hashed values as well. So how do you decode these hashed values?

Use the same base64 command used earlier to encode it. But this time add a decode option to it.

```sh
$ echo -n bXlzcWw= | base64 --decode
mysql

$ echo -n YXNob2s= | base64 --decode
ashok

$ echo -n YXNob2sxMjM= | base64 --decode
ashok123
```

Now that we have secret created. Let us proceed with step 2, configuring it with a POD.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-web-app
spec:
  containers:
  - name: my-web-app-container
    image: my-web-app
    ports:
      - containerPort: 8080
    envFrom:
      - secretRef:
          name: app-secret
```

#### ConfigMap

When you have a lot of POD definition files, it will become difficult to manage the environment data stored within the query files.

We can take this information out of the POD definition file and manage it centrally using configuration maps.

ConfigMaps are used to pass configuration data in the form of key value pairs in Kubernetes.

When a POD is created, inject the ConfigMap into the POD. So the key value pairs that are available as environment variables for the application hosted inside the container in the POD.

There are 2 phases involved in configuring ConfigMaps. First create the ConfigMaps and second inject them into the POD.

Just like any other Kubernetes object, there are 2 ways of creating a ConfigMap.

The imperative way – without using ConfigMap definition file and the declarative way – by using a ConfigMap definition way.

- Imperative Approach:

If you do not wish to create a ConfigMap definition, you could simply use following command

```sh
kubectl create configmap <config-name> --from-literal=<key>=<value>
```

```sh
kubectl create configmap app-config --from-literal=APP_COLOR=pink
```

If you wish to add additional key value pairs then simply specify the –from-leteral options multiple times

```sh
kubectl create configmap app-config --from-literal=APP_COLOR=pink --from-literal=APP_MODE=production
```

However this will get complicated when you have too many configuration items. Another way to input configuration data is through a file.

```sh
kubectl create configmap <config-name> --from-file=<path-to-file>
kubectl create configmap app-config --from-file=app-config.properties
```

- Declarative Approach

In this approach we create a definition file just like how we did for the POD.

The file has apiVersion, kind, metadata and instead of spec, here we have “data”.

```yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: app-config
data:
  APP_COLOR: pink
  APP_MODE: production
```

Once you are ready then you need to run the following command.

```sh
kubectl create -f config-map.yaml
```

Above command will creates the app-config ConfigMap with the values we specified. You can create as many ConfigMaps as you need.

To view ConfigMaps, you need to run the following command.

```sh
kubectl get configmaps
NAME            DATA           AGE
app-config      2              3s
```

To describe ConfigMaps, you need to run the following command.

```sh
kubectl describe configmaps
```

Above command will list the configuration data as well under the data section.

Now that we have the ConfigMap created let us proceed with another step configuring it with a POD.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-web-app
spec:
  containers:
  - name: my-web-app-container
    image: my-web-app
    ports:
      - containerPort: 8080
    envFrom:
      - configMapRef:
          name: app-config
```

#### Scale Application

The kubectl scale command lets your instantaneously change the number of replicas you want to run your application.

To use kubectl scale, you specify the new number of replicas by setting the `--replicas` flag. For example, to scale my-app to four replicas, run the following command, substituting CONTROLLER for deployment, statefulset, or another controller object type:

```sh
kubectl scale CONTROLLER my-app --replicas 4
```

If successful, this command's output should be similar to deployment "my-app" scaled.

Next, run:

```sh
kubectl get CONTROLLER my-app

# The output should look similar to the following:

NAME                  DESIRED   CURRENT   UP-TO-DATE   AVAILABLE   AGE
my-app                4         4         4            4           15m
```

=========OR=========

You can use kubectl apply to apply a new configuration file to an existing controller object. kubectl apply is useful for making multiple changes to a resource, and may be useful for users who prefer to manage their resources in configuration files.

To scale using kubectl apply, the configuration file you supply should include a new number of replicas in the replicas field of the object's specification.

The following is an updated version of the configuration file for the example my-app object. The example shows a Deployment, so if you use another type of controller, such as a StatefulSet, change the kind accordingly. This example works best on a cluster with at least three Nodes.

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: my-app
spec:
  replicas: 3
  selector:
    matchLabels:
      app: app
  template:
    metadata:
      labels:
        app: app
    spec:
      containers:
      - name: my-container
        image: us-docker.pkg.dev/google-samples/containers/gke/hello-app:2.0
```

In this file, the value of the replicas field is 3. When this configuration file is applied, the object my-app scales to three replicas.

To apply an updated configuration file, run the following command:

```sh
kubectl apply -f config.yaml
```

Next, run:

```sh
kubectl get CONTROLLER my-app

# The output should look similar to the following:

NAME                  DESIRED   CURRENT   UP-TO-DATE   AVAILABLE   AGE
my-app                3         3         3            3           15m
```

- AutoScaling Deployment

kubectl autoscale creates a HorizontalPodAutoscaler (or HPA) object that targets a specified resource (called the scale target) and scales it as needed. The HPA periodically adjusts the number of replicas of the scale target to match the average CPU utilization that you specify.

When you use kubectl autoscale, you specify a maximum and minimum number of replicas for your application, as well as a CPU utilization target. For example, to set the maximum number of replicas to six and the minimum to four, with a CPU utilization target of 50% utilization, run the following command:

```sh
kubectl autoscale deployment my-app --max 6 --min 4 --cpu-percent 50
```

In this command, the --max flag is required. The --cpu-percent flag is the target CPU utilization over all the Pods. This command does not immediately scale the Deployment to six replicas, unless there is already a systemic demand.

After running kubectl autoscale, the HorizontalPodAutoscaler object is created and targets the application. When there is a change in load, the object increases or decreases the application's replicas.

To get a list of the HorizontalPodAutoscaler objects in your cluster, run:

```sh
kubectl get hpa
```

To see a specific HorizontalPodAutoscaler object in your cluster, run:

```sh
kubectl get hpa HPA_NAME
```

Replace HPA_NAME with the name of your HorizontalPodAutoscaler object.

To see the HorizontalPodAutoscaler configuration:

```sh
kubectl get hpa HPA_NAME -o yaml
```

The output of this command is similar to the following:

```yaml
apiVersion: v1
items:
- apiVersion: autoscaling/v1
  kind: HorizontalPodAutoscaler
  metadata:
    creationTimestamp: ...
    name: HPA_NAME
    namespace: default
    resourceVersion: "664"
    selfLink: ...
    uid: ...
  spec:
    maxReplicas: 10
    minReplicas: 1
    scaleTargetRef:
      apiVersion: apps/v1
      kind: Deployment
      name: HPA_NAME
    targetCPUUtilizationPercentage: 50
  status:
    currentReplicas: 0
    desiredReplicas: 0
kind: List
metadata: {}
resourceVersion: ""
selfLink: ""

```

In this example output, the targetCPUUtilizationPercentage field holds the 50 percentage value passed in from the kubectl autoscale example.

To see a detailed description of a specific HorizontalPodAutoscaler object in the cluster:

```sh
kubectl describe hpa HPA_NAME
```

You can modify the HorizontalPodAutoscaler by applying a new configuration file with kubectl apply, using kubectl edit, or using kubectl patch.

To delete a HorizontalPodAutoscaler object:

```sh
kubectl delete hpa HPA_NAME
```

#### Multi Container

The multi container pods are the pods that contain two or more related containers that share resources like network space, shared volumes, etc and work together as a single unit.

If you need to run a single container in Kubernetes, then you have to create a pod for it which is nothing but Single Container Pod.

If you have to run two or more containers in a pod, then the pod created to place these containers is called a Multi Container Pod.

Basically, these are helper processes or containers enhance the main containers by providing additional functionality.

Multi container PODs share the same life cycle, which means they are created together and destroyed together. They share the same network space which means they can refer to each other as localhost and they have access to the same storage volumes.

This way you don’t have to establish volume sharing or services between PODs to enable communication between them.

![Multi-Pod](Image/CKA-43.png)

Since containers should not be deployed directly to save ourselves from inevitable disasters, we use pods to deploy them as discussed previous tutorials.

But what if there are tightly-coupled containers, for example, a database container and a data container, should we place them in two different pods or a single one? This is where a Multi Container Pods comes in.

To create a multi container POD, add the new container information to the POD definition file.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-webapp
spec:
  containers:
  - name: my-webapp-container
    image: my-webapp
    ports:
      - containerPort: 8080
  - name: queue-listener
    image: queue-listener
```

Design-patterns Of Multi Container Pods:

There are 3 common patterns when it comes to designing multi container PODs.

1. Sidecar pattern
2. Adaptor pattern
3. Ambassador pattern.

Sidecar pattern

Sidecars derive their name from motorcycle sidecars. While your motorcycle can work fine without the sidecar, having one enhances or extends the functionality of your bike, by giving it an extra seat.

Similarly, in Kubernetes, a sidecar pattern is used to enhance or extend the existing functionality of the container.

Your container works perfectly well without the sidecar, but with it, it can perform some extra functions. Some great examples are using a sidecar for monitoring and logging and adding an agent for these purposes.

The most common sidecar containers are logging utilities, sync services, watchers, and monitoring agents.

Adapter Pattern

The Adapter is another pattern that you can implement with multiple containers.

The adapter pattern is used to standardize the output by the primary container. Standardizing refers to format the output in a specific manner that fits the standards across your applications.

For instance, an adapter container could expose a standardized monitoring interface to the application even though the application does not implement it in a standard way. The adapter container takes care of transforming the output into what is acceptable at the cluster level.

Ambassador Pattern

The ambassador design pattern is used to connect containers with the outside world.

In this design pattern, the helper container can send network requests on behalf of the main application. It is nothing but a proxy that allows other containers to connect to a port on the localhost.

This is a pretty useful pattern especially when you are migrating your legacy application into the cloud.

For instance, some legacy applications that are very difficult to modify, and can be migrated by using ambassador patterns to handle the request on behalf of the main application.

#### Init Container

A Pod can have multiple containers running apps within it, but it can also have one or more init containers, which are run before the app containers are started.

Init containers are exactly like regular containers, except:

Init containers always run to completion.
Each init container must complete successfully before the next one starts.
If a Pod's init container fails, the kubelet repeatedly restarts that init container until it succeeds. However, if the Pod has a restartPolicy of Never, and an init container fails during startup of that Pod, Kubernetes treats the overall Pod as failed.

To specify an init container for a Pod, add the initContainers field into the Pod specification, as an array of container items (similar to the app containers field and its contents). See Container in the API reference for more details.

The status of the init containers is returned in .status.initContainerStatuses field as an array of the container statuses (similar to the .status.containerStatuses field).

Because init containers have separate images from app containers, they have some advantages for start-up related code:

- Init containers can contain utilities or custom code for setup that are not present in an app image. For example, there is no need to make an image FROM another image just to use a tool like sed, awk, python, or dig during setup.
- The application image builder and deployer roles can work independently without the need to jointly build a single app image.
- Init containers can run with a different view of the filesystem than app containers in the same Pod. Consequently, they can be given access to Secrets that app containers cannot access.
- Because init containers run to completion before any app containers start, init containers offer a mechanism to block or delay app container startup until a set of preconditions are met. Once preconditions are met, all of the app containers in a Pod can start in parallel.
- Init containers can securely run utilities or custom code that would otherwise make an app container image less secure. By keeping unnecessary tools separate you can limit the attack surface of your app container image.

Eg:

- Wait for a Service to be created, using a shell one-line command like:

```sh
for i in {1..100}; do sleep 1; if dig myservice; then exit 0; fi; done; exit 1
```

- Register this Pod with a remote server from the downward API with a command like:

```sh
curl -X POST http://$MANAGEMENT_SERVICE_HOST:$MANAGEMENT_SERVICE_PORT/register -d 'instance=$(<POD_NAME>)&ip=$(<POD_IP>)'
```

- Wait for some time before starting the app container with a command like

```sh
sleep 60
```

- Clone a Git repository into a Volume

- Place values into a configuration file and run a template tool to dynamically generate a configuration file for the main app container. For example, place the POD_IP value in a configuration and generate the main app configuration file using Jinja.

This example defines a simple Pod that has two init containers. The first waits for myservice, and the second waits for mydb. Once both init containers complete, the Pod runs the app container from its spec section.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: myapp-pod
  labels:
    app: myapp
spec:
  containers:
  - name: myapp-container
    image: busybox:1.28
    command: ['sh', '-c', 'echo The app is running! && sleep 3600']
  initContainers:
  - name: init-myservice
    image: busybox:1.28
    command: ['sh', '-c', "until nslookup myservice.$(cat /var/run/secrets/kubernetes.io/serviceaccount/namespace).svc.cluster.local; do echo waiting for myservice; sleep 2; done"]
  - name: init-mydb
    image: busybox:1.28
    command: ['sh', '-c', "until nslookup mydb.$(cat /var/run/secrets/kubernetes.io/serviceaccount/namespace).svc.cluster.local; do echo waiting for mydb; sleep 2; done"]
```

- You can start this Pod by running:

```sh
kubectl apply -f myapp.yaml
```

And check on its status with:

```sh
kubectl get -f myapp.yaml


# The output is similar to this:

NAME        READY     STATUS     RESTARTS   AGE
myapp-pod   0/1       Init:0/2   0          6m
```

or for more details:

```sh
kubectl describe -f myapp.yaml
The output is similar to this:

Name:          myapp-pod
Namespace:     default
[...]
Labels:        app=myapp
Status:        Pending
[...]
Init Containers:
  init-myservice:
[...]
    State:         Running
[...]
  init-mydb:
[...]
    State:         Waiting
      Reason:      PodInitializing
    Ready:         False
[...]
Containers:
  myapp-container:
[...]
    State:         Waiting
      Reason:      PodInitializing
    Ready:         False
[...]
Events:
  FirstSeen    LastSeen    Count    From                      SubObjectPath                           Type          Reason        Message
  ---------    --------    -----    ----                      -------------                           --------      ------        -------
  16s          16s         1        {default-scheduler }                                              Normal        Scheduled     Successfully assigned myapp-pod to 172.17.4.201
  16s          16s         1        {kubelet 172.17.4.201}    spec.initContainers{init-myservice}     Normal        Pulling       pulling image "busybox"
  13s          13s         1        {kubelet 172.17.4.201}    spec.initContainers{init-myservice}     Normal        Pulled        Successfully pulled image "busybox"
  13s          13s         1        {kubelet 172.17.4.201}    spec.initContainers{init-myservice}     Normal        Created       Created container with docker id 5ced34a04634; Security:[seccomp=unconfined]
  13s          13s         1        {kubelet 172.17.4.201}    spec.initContainers{init-myservice}     Normal        Started       Started container with docker id 5ced34a04634
```

To see logs for the init containers in this Pod, run:

```sh
kubectl logs myapp-pod -c init-myservice # Inspect the first init container
kubectl logs myapp-pod -c init-mydb      # Inspect the second init container
```

Here's a configuration you can use to make those Services appear:

```yaml
---
apiVersion: v1
kind: Service
metadata:
  name: myservice
spec:
  ports:
  - protocol: TCP
    port: 80
    targetPort: 9376
---
apiVersion: v1
kind: Service
metadata:
  name: mydb
spec:
  ports:
  - protocol: TCP
    port: 80
    targetPort: 9377
```

To create the mydb and myservice services:

```sh
kubectl apply -f services.yaml

# The output is similar to this:

service/myservice created
service/mydb created
```

You'll then see that those init containers complete, and that the myapp-pod Pod moves into the Running state:

```sh
kubectl get -f myapp.yaml

# The output is similar to this:

NAME        READY     STATUS    RESTARTS   AGE
myapp-pod   1/1       Running   0          9m
```

#### Probes

Readiness Probes:

POD LifeCycle
A POD has a POD status and conditions.

A POD status tells us where a POD is in its lifecycle.
When a POD is creating, it will be in a pending state, this is when the scheduler tries to figure out, where to place the POD.
If the scheduler cannot find a node to place the POD, it remains in the pending state.
To find out, why it's stuck in a pending state run

```sh
kubectl describe pod <pod-name>
```

Once the POD is scheduled, it goes to containerCreating status, where are the images needed for the application are pulled and the container starts.

Once all the containers in a POD starts, it goes into a running state. It continues to be in running state until the program gets completed successfully or it is terminated.

The status of the POD can be seen under kubectl get pods. The POD status only gives us the high level summary of the POD.

Conditions complement the POD status.
It is an array of True or False values, that tell us the state of a POD.
When a POD is scheduled on a node, the POD scheduled condition is set to True and when the POD is initialised, it's value is set to True.
When all the containers in the POD are ready, the containersReady is set to True and finally the POD itself is considered to be ready.
To see the status the POD conditions..

```sh
kubectl describe <pod-name> -- under conditions.
```

We also see the ready state of the POD in the output of kubectl get pods.
The containersReady or Ready condition indicates that the containers inside the pod are ready to accept the user traffic.

Normally servers takes some seconds to intialize the server and ready to serve the users. During this wait period, the pod continues to show that the container is ready to server. In this case, the status of the container is wrong. By default, kubernetes assumes as soon as the container is created, it is ready to serve the user traffic.
This makes users to hit a pod that is not yet running a live application.

We need a way to tie the ready condition to the actual state of the application inside the container.

To check the application is ready or not, we can set up of different kinds of tests

In case of webservers - HTTP test - /api/ready
In case of database - TCP test - particular TCP socket is listening or not
customer script in the container that executes successfully when container is ready.
In the above cases, only when the test gets passed, the container will be set to ready state. These tests can be configures in pod-definition file as below

![Probes](Image/CKA-44.png)

For a minimum of 10 seconds warmup we can add initialDelaySeconds option To specify how often to probe, we can use periodSeconds option By default, if the application is not ready after 3 attemps the probe will stop.
If we want to make more attempts use failureThreshold option.

![Probes](Image/CKA-45.png)

Liveness Probes
When we run an image of nginx using docker, it starts to serve the users. For some reason, the web server crashes and nginx process exists. The container exists as well.
Since, docker is not an orchestration engine, the container continues to stays to dead and denies services to users, until we manually create other nginx container.

In kubernetes orchestation, when we run the same application with kubernetes, everytime the application crashes, kubernetes makes an attempt to restart the container to restore service to users. (if we observe, number of restarts in kubectl get pods command get increases)

If the application is not working (because of coding issues) but the container continues stay alive i.e., container is up but the users hitting the container are not served. In this case, container needs to be restarted or destroyed and a new container needs to be brought up. Here comes the liveliness probe.

A liveliness probe can be configured on the container to periodically test whether the application within the container is actually healthy? If the test fails, the container is considered unhealthy and is destroyed and recreated.
As a developer, we need to define what it means to a application to be healthy.

In case of a webapplication - when an api server is up and running.
In case of a database - a particular TCP socket is listening.
Simply execute a command to perform a test.
Liveness probe is configured in the pod definitionfile as readiness probe

![Probes](Image/CKA-46.png)
![Probes](Image/CKA-47.png)

#### Jobs

There are different types of workloads that a container can serve.
Workloads such as web servers continue to run for a long period of time, until manually taken down. There are other kinds of workloads such as batch processing, analytics or reporting, that are meant to carryout specific tasks and finish.
Example: Performing a computation, processing an image, performing an analytic task, sending an email etc,. These are meant for short period of time.

Let us first see how these workloads work in docker.
In Docker,
docker run ubuntu expr 3+2 (performs a simple math operation)
In this case, docker container comes up, perform the simple operation, prints the output and then exists.
when we run docker ps -a command, we see the container in exit state.

In Kubernetes,

![Jobs](Image/CKA-48.png)

Though the container computes output and exits, kubernetes continues to restart the container and bring it up again. This continues to happen until a threshold is reached.

Kubernetes wants our applications to live forever. The default behaviour of pods is to attempt to restart the container to keep it running.
This behaviour is defined by the property restartPolicy set on the pod which is by default set to always. Therefore, the pod always recreates the container when it exits. We can overwrite this behaviour by setting this property to Never or Onfailure. Thus, the kubernetes does not restart the container once the job is finished.

```yaml
apiVersion: v1
kind: Pod
metadata: 
  name: math-pod
spec:
  containers: 
    - name: math-add
      image: ubuntu
      command: ['expr', '3', '+', '2']

  restartPolicy: Never
```

While replicaset is used to make sure a specified number of pods are running at all time, a job is used to run a set of pods to perform a given task to completion.

We create a job using a definition file.

```yaml
apiVersion: batch/v1
kind: Job
metadata:
  name: math-add-job
spec:
  template:
  # pod-definition specification
    spec:
      containers:
        - name: math-add
          image: ubuntu
          command: ['expr', '2', '+', '3']
      restartPolicy: Never
```

To create a job `kubectl create -f job-definition.yaml`

To view the jobs

```sh
kubectl get jobs
```

The standard ouput of the container can be seen in container logs

```sh
kubectl logs <podname>
```

To delete the job

```sh
kubectl delete job <jobname>
```

![Jobs](Image/CKA-49.png)

Job with multiple pods

To run multiple pods we set a value for completions under the job specification.

![Jobs](Image/CKA-50.png)

By default, the pods are created one after the other. The second pod is created only after the first is finished.

If the pod fails, the job tries to create new pods until it has three successful completions, and that completes the job.

![Jobs](Image/CKA-51.png)

Instead of getting the pods created sequentially, we can get them created in parallel. For this add the property called parallelism to the job specification. We set it to 3, to create 3 pods in parallel.

![Jobs](Image/CKA-52.png)

The job first creates 3 pods at once, two of which completes successfully. Now, we only need one more, it is intelligent enough to create one pod at a time, until we get a total 3 successful pods.

CronJobs

A CronJob is a job that can be scheduled. We can schedule and run a CronJob Periodically. Example: A job to generate a report and send an email.

```yaml
apiVersion: batch/v1beta1
kind: CronJob
metadata: 
  name: reporting-cron-job
spec:
  # schedule option takes cron like format string, where it takes the time when the job is to be run
  schedule: "*/1 * * * *"
  jobTemplate:
    # Job spec
    spec: 
      completions: 3
      parallelism: 3
      template:
        spec:
          containers: 
            - name: reporting-tool
              image: reporting-tool
          restartPolicy: Never
```

![Jobs](Image/CKA-53.png)

To create cronjob

```sh
kubectl create -f <cronjob-definition-file>
```

To view the available cronjobs kubectl get cronjob

#### Self-Healing

Kubernetes supports self-healing applications through ReplicaSets and Replication Controllers. The replication controller helps in ensuring that a POD is re-created automatically when the application within the POD crashes. It helps in ensuring enough replicas of the application are running at all times.

Kubernetes provides additional support to check the health of applications running within PODs and take necessary actions through Liveness and Readiness Probes. However these are not required for the CKA exam and as such they are not covered here. These are topics for the Certified Kubernetes Application Developers (CKAD) exam and are covered in the CKAD course.

### Cluster Maintainance

#### OS Upgrades

we will discuss about cluster maintenance purposes like upgrade operating system or applying patches like security patches etc. on your cluster.

![OS](Image/CKA-54)

So you have a cluster with few nodes and PODs serving applications. What happens when one of these nodes go down? Of course the PODs on them are not accessible.

![OS](Image/CKA-55)

Now depending upon how you deployed these PODs, your users may be impacted.

- Simple Example

For example, since you have multiple replicas of the blue POD, the users accessing the blue application are not impacted as they are being served through the other blue POD that’s online.

However users accessing the green POD, are impacted as that was the only POD running the green application. Now what does Kubernetes do in this case?

If the node come back online immediately, then the kubelet process starts and the PODs come back online. However, if the node was down for more than 5 minutes, then the PODs are terminated from that node.

Well, Kubernetes considers them as dead. If the PODs where part of a replicaset then they are recreated on other nodes. The time it waits for a POD to come back online is known as the POD eviction timeout and is set on the controller manager with a default value of 5 minutes.

So when ever node goes offline, the master node waits for up to 5 minutes before considering the node dead.

When the node comes back online after the POD eviction timeout it comes up blank without any PODs scheduled on it.

Since the blue POD was part of a replicaset, it had a new POD created on another node. However since the green POD was not part of the replicaset it is just gone.

Thus if you have maintenance tasks to be performed on a node, if you know that the workloads running on the node have other replicas and if it’s okay that they do down for a short period of time. And if you’re sure the node will come back online within 5 minutes you can make a quick upgrade and reboot.

However you don’t for sure know if a node is going to be back online in 5 minutes. Well you cannot for sure say it is going to be back at all. So there is a safer way to do it.

You can purposefully drain the node of all the workloads. So that the workloads are moved to other nodes in the cluster.

![OS](Image/CKA-56)

Well technically they are not moved. When you drain the node the PODs are gracefully terminated from the node that they’re on and recreated on another.

```sh
kubectl drain node1
```

The node is also cordoned or marked as unschedulable. Meaning no PODs can be scheduled on this node until you specifically remove the restriction.

Now that the PODs are safe on the other nodes, you can reboot the first node. When it comes back online it is still unschedulable.

You then need to uncordon it, so that PODs can be scheduled on it again.

```sh
kubectl uncordon node1
```

Now, remember the PODs that were moved to the other nodes, don’t automatically fall back. If any of those PODs were deleted or if new PODs were created in the cluster, then they would be created on this node.

Apart from drain and uncordon, there is also another command called cordon.

```sh
kubectl cordon node1
```

Cordon simply marks a node unschedulable. Unlike drain it doesn’t terminate or move the PODs on an existing node. It simply makes sure that new PODs are not scheduled on that node.

![OS](Image/CKA-57)

#### Kubernetes Software Version

we will discuss about the various Kubernetes releases and versions.

So what do we know about API versions in Kubernetes so far? We know that when we install a Kubernetes cluster, we install a specific version of Kubernetes.

We can see that when we run the `kubectl get nodes` command.

```sh
 kubectl get nodes
NAME            STATUS   ROLES    AGE    VERSION
node3           Ready    <none>   5d1h   v1.19.3-34+a56971609ff35a
node2           Ready    <none>   5d1h   v1.19.3-34+a56971609ff35a
node1           Ready    <none>   5d2h   v1.19.3-34+a56971609ff35a
```

In this case version is v1.19.3. In this tutorial we will see how Kubernetes project manages software releases.

- About version

![KSV](Image/CKA-58.png)

Let’s take a closer look at the version number. The Kubernetes release versions consists of 3 parts. The first is the major version (v1), followed by the minor version (19) and then the patch version (3).

While minor versions are released every few months with new features and functionalities, patches are released more often with critical bug fixes.

Just like many other popular applications out there, Kubernetes follows a standard software release versioning procedure.

Every few month it comes out with new features and functionalities through a minor release. The first major version was released in July of 2015. As of this tutorial the latest stable version is 1.19.3.

Apart from this you will see alpha and beta releases. All the bug fixes and improvements first go into an alpha release tagged alpha. In this release, the features are disabled by default and may be buggy.

Then from there they make their way to beta release where the code is well tested. The new features are enabled by default. And finally they make their way to the main stable release.

![KSV](Image/CKA-59.png)

You can find all the releases in the releases page of the Kubernetes GitHub repository.

Download the Kubernetes.tar.gz file and extract it to find executables for all the Kubernetes components. The downloaded package when extracted has all the control plane components in it. All of them of the same version.

Please note that there are other components within the control plane that don’t have the same version numbers (ETCD cluster and Core DNS servers).

![KSV](Image/CKA-60.png)

The ETCD cluster and Core DNS servers have their own versions as they are separate projects.

The release notes of each release provide information about the supported versions of externally dependent applications like ETCD and Core DNS etc.

- Release References

[K8s-API](https://kubernetes.io/docs/concepts/overview/kubernetes-api/)

[Release](https://github.com/kubernetes/kubernetes/releases)

Here is a link to kubernetes documentation if you want to learn more about this topic (You don't need it for the exam though):

[Kubernetes_API_Conventions](https://github.com/kubernetes/community/blob/master/contributors/devel/sig-architecture/api-conventions.md)

[Kubernetes_API_Changes](https://github.com/kubernetes/community/blob/master/contributors/devel/sig-architecture/api_changes.md)

#### Cluster Upgrade Process

we will discuss about Cluster Upgrade Process in Kubernetes.

In the previous tutorial, we will discuss how Kubernetes manages its software releases and how different components have their versions.

![CUP](Image/CKA-60.png)

We will keep dependencies on external components like ETCD and CoreDNS aside for now and focus on the core control plane components.

![CUP](Image/CKA-61.png)

It is mandatory that they all have the same version. Now the components can be in different release versions.

Since the Kube API server is the primary component in the control plane and that is the component that all other components talked to. None of the other components should never be at a higher version than the Kube API server.

The controller manager and scheduler can be at one version lower. So if the Kube API server was at X, control managers and scheduler can be at X-1 and the kubelet and kube-proxy components can be at 2 versions lower X-2.

![CUP](Image/CKA-62.png)

None of the components could be at higher version than the Kube API server like v1.11.

Now this is not the case with the Kubectl. The Kubectl utility could be v1.11 a version higher than the Kube API server, v1.9 a version lower than the Kube API server or v1.10 same version of the Kube API server.

Now this permissible SKU in versions allows us to carryout live upgrades. We can upgrade component by component if required.
 
So, when should we upgrade? Let’s say you are at version 1.10 and Kubernetes versions is 1.11 & 1.12. At any time Kubernetes supports only up to recent 3 minor versions.

So, with 1.12 is the latest release Kubernetes supports v1.12, v1.11 and v1.10. Therefore, when v1.13 is released only versions v1.13, v1.12 and v1.11 are supported.

Before the release of v1.13 would be a good time to upgrade your cluster to the next release. So, how do we upgrade? do we upgrade directly from v1.10 to v1.13? Answer is No.

The recommended approach is to upgrade a minor version at a time. v1.10 to v1.11 then v1.11 to v1.12 and then v1.12 to v1.13. The upgrade process depends on how our cluster is configured.

For example, if out cluster is a managed Kubernetes cluster deployed on cloud service provider like Google. Google Kubernetes engine lets you upgrade our cluster easily by just a few clicks.

If we deploy our Kubernetes cluster using tools like Kubeadm then the tool can help you plan and upgrade the cluster.

If we deployed our Kubernetes cluster from scratch, then we manually upgrade the different components of cluster our self. In this tutorial, we will look at options by Kubeadm.

So, we have a cluster with master nodes and worker nodes running in production hosing PODs that serving users.

The nodes and components are at version 1.10. Upgrading the cluster involves 2 major steps.

First, we upgrade our master nodes and then upgrade the worker nodes. While the master nodes being upgraded, the control plane components such as the API server, Scheduler and the controller manager go down briefly.

The master go down doesn’t mean you worker nodes and applications are impacted. All workloads hosted on worker nodes continue to serve users normally.

Since the master is down, all management functions are down. We can’t access the cluster using the Kubectl or other Kubernetes API. We can’t deploy new applications or delete or modify existing ones.

The controller manager also didn’t work. If a POD is fails, a new POD will not be created automatically. But as long as nodes and PODs are up, our applications should be up and users will not be impacted.

Once the upgrade is complete and cluster is backed up, it should function normally.

Now we have the master and the main components had version v1.11 and the worker nodes had version v1.10.

As we discussed earlier, this is a supported configuration. Now it’s time time to upgrade worker nodes. There are different strategies available to upgrade worker nodes.

One is to upgrade all of them at once. But then PODs are down and users are no longer able to access the applications. Once the upgrade is complete, the nodes are backed up, new PODs are scheduled and users can resume access. This is one strategy that requires downtime.

The second strategy is to upgrade one node at a time. So, going back to the state where we have our master upgraded and the nodes waiting to be upgraded.

We first upgrade the first node, where the workloads moved to the second and third node and users are served from there. Once the first node is upgraded and backed up with an update the second node where the workloads moved to first and third nodes and finally the third node where the workloads are shared between first two.

Until we have all the nodes are upgraded to a newer version. We then follow the same procedure to upgrade the nodes from v1.11 to v.12 and then v1.13.

The third strategy would be to add a new node to the cluster. Nodes with newer software version. This is especially convenient if you are in a cloud environment where you can easily provision new nodes and decommission old nodes.

Nodes with the newer software version that can be added to the cluster. Move the workload to the new one and remove the old node until you finally have all the new nodes with the new software versions.

Let’s now how it is done? Say we were to upgrade this cluster from v1.11 to v1.13.

Kubeadm has an upgrade command that helps upgrading clusters. With Kubeadm run the following command to know the information about current version, kubeadm tool version, latest stable version of Kubernetes.

```sh
kubeadm upgrade plan
```

This command also lists all the control plane components and their versions and what versions these can be upgraded to. It also tells us that after we upgrading the control plane components, you must manually upgrade the kubelet versions on each node.

Please note that kubeadm doesn’t install or upgrade Kubelets. Finally it provides the commands to upgrade the cluster. Also note that we must upgrade the kubeadm tool itself before you can upgrade the cluster.

The Kubeadm tool also follows the same software version as Kubernetes.

So, we are at v1.11 and we want go to v1.13. But remember that we can only go one minor version at a time. So we first go to v1.12. First upgrade the kubeadm tool using following command

```sh
sudo apt-get upgrade -y kubeadm=1.12.0-00
```

Now upgrade the Kubernetes cluster using following command

```sh
kubeadm upgrade apply v1.12.0
```

Above command pulls the necessary images and upgrade the cluster components. Once upgrade complete our control plane components are now at v1.12. If you run following command you will still see the master node at v1.11.

```sh
kubectl get nodes
NAME        STATUS       ROLES       AGE        VERSION
node01      Ready        master      2d         v1.11.3
node02      Ready        <none>      2d         v1.11.3
node03      Ready        <none>      2d         v1.11.3
```

This is because, in the output of this command, it is showing the versions of the Kubelet on each of the nodes registered with API server and not the version of the API server version itself.

So, the next step is to upgrade the Kubelets. Remember that, depending on our configuration we may or mayn’t have Kubelet running on the master node.

In this case, the cluster deployed with the kubeadm as kubelets on the master nodes which are used to run the control plane components as part of the master node.

So, the next step is to upgrade the kubelet on the master node if we have the kubelet on them. Run the following command to upgrade kubelet

```sh
sudo apt-get upgrade -y kubelet=1.12.0-00 
```

Once the package is upgraded, restart the kubelet using following command

```sh
systemctl restart kubelet
```

Now run the following command to check the version

```sh
kubectl get nodes
NAME        STATUS       ROLES       AGE        VERSION
node01      Ready        master      2d         v1.12.0
node02      Ready        <none>      2d         v1.11.3
node03      Ready        <none>      2d         v1.11.3
```

Now the master is upgraded to v1.12. The worker nodes are still at v1.11.

So, next the worker nodes. Let us start one at a time. We need to first move the workloads from the first worker node to other nodes. The following command is used to safely shutdown all PODs from the node and reschedule to the other nodes.

```sh
kubectl drain node01
```

Now upgrade the kubeadm and kubelet packages on the worker node as we did in master node.

```sh
sudo apt-get upgrade -y kubeadm=1.12.0-00

sudo apt-get upgrade -y kubelet=1.12.0-00 

kubeadm upgrade node config --kubelet-version v1.12.0

systemctl restart kubelet
```

The node should now be up with the new software version. However when we drain the node, we actually marked it unschedulable. So we need to unmark it by running the following command.

```sh
kubectl uncordon node01
```

The node is now schedulable. But remember that it is not necessary the PODs come back to this node. It is only marked it as schedulable. Only when the PODs are deleted from other nodes or when new PODs are scheduled they really come back to this node.

Similarly we can upgrade other nodes as well. We now all the nodes are upgraded.

Steps On Demo:

1. Check the Upgrade Plan
2. Upgrade the Kubeamd on control Plane
3. Verify Upgrade successful with Upgrade Plan
4. Drain the Control Plan to change the version
5. Upgrade Kubelet and Kubectl
6. Reload Daemon and Restart the kubelet
7. Uncordon the drained Control Plane
8. Same way Upgrade Kubeadm on the worker node
9. Upgrade kubelet configuration `upgrade node-name`
10. Drain the node --> Run drain command from control plane(master Node)
11. Upgrade Kubelet and Kubectl
12. Reload Daemon and Restart the kubelet
13. Uncordon the drained worker node from control plane(master Node)

#### BackUp and Restore Method

we will discuss about various backup and restore methodologies in Kubernetes cluster.

Let’s start by looking at what we should consider backing up in a Kubernetes cluster.

So far we have deployed a number of different applications on our Kubernetes cluster using deployment, POD, Service definition files.

We know that the ETCD cluster is where all cluster related information is stored. And if our applications are configured with persistent storage then that is another candidate for backups.

- Imperative

With respective to resources that we created in the cluster, at times we used the imperative way of creating an object by executing a command. Such as while creating a namespace or secret or configmap or at times for exposing applications.

- Declarative

And at times we used the declarative approach by first creating a definition file and then running the kubectl apply command on that file. This is the preferred approach if we want to save our configuration. Because now we have all the objects required for a single application in the form of object definition files in a single folder.

This can be easily be reused at a later time or shared with others. Of course we must have a copy of these files saved at all times.

A good practice is to store these on source code repositories. That it can be maintained by a team. The source code repository should be configured with the right backup solutions.

With managed/public source code repositories like GitHub, we don’t have to worry about this. With that even when we lose our entire cluster, we can redeploy our application on the cluster by simply applying this configuration files on them.

While the declarative approach is the preferred approach it is not necessary that all of our team members stick to those standards. What if someone created an object the imperative way without documenting that information anywhere?

So a better approach to backing up resource configuration is to use query the Kube API Server.

- Backup – Resource Configs

Query the Kube API Sever using the Kubectl or by accessing the API server directly and save all resource configurations for all objects created on the cluster has a copy.

For example, one of the commands that can be used in a backup script is to get all PODs, deployments and services in all namespaces using the following command

```yaml
kubectl get all --all-namespaces -o yaml > all-deploy-services.yaml
```

Using the above kubectl utility get all command and extract the output in a YAML format. Then save that file. And that’s just for a few resources groups. There are many other resource groups that must be considered.

Of course you don’t have to develop that solutions yourself. There are tools like ARK or now called Velero by heptio that can do this for you. It can help in taking backups of your Kubernetes cluster using the Kubernetes API.

- Backup – ETCD

![B&R](Image/CKA-63.png)

Let us now move on to ETCD. The ETCD cluster stores information about the state of the cluster. So information about the cluster itself, the nodes and every other resource as created within the cluster are stored here.

So instead of backing up resource as before, you may chose to backup the ETCD server itself. As we have seen the ETCD cluster is hosted on the master nodes.

While configuring ETCD we specified a location where all the data would be stored. The data directory. That is the directory that can be configured to be backup by your backup tool.

ETCD also comes with a built in snapshot solution. You can take a snapshot of the ETCD database by using the etdctl utilities snapshot save command.

```sh
etcdctl snapshot save snapshot.db

ls 
snapshot.db
```

Once you run the above command, A snapshot file is created by the name in the current directory.

If you wanted to be created in another location specified the full path. You can view the status of the backup using the snapshot status command.

- Restore – ETCD

To restore the cluster from this backup at a later point in time, first stop the kube-api server service, as the restore process will require you to restart the ETCD cluster and the kube-api server depends on it. Then run the etcdctl snapshot restore command with the path set to the path of the backup file which is the snapshot.db file.

When ETCD restores from a backup, it initializes a new cluster configuration and configures the members of ETCD as new members to a new cluster. This is to prevent a new member from accidentally joining an existing cluster.

Say for example, you use this backup snapshot to provision a new etcd-cluster for testing purposes. You don’t want the members in the new test cluster to accidentally join the production cluster.

So during a restore you must specify a new cluster token and the same initial cluster configuration options specified in the original configuration file. On running this command a new data directory is created.

We then configure the ETCD configuration file to use the new cluster-token and data directory. The reload the service daemon and restart etcd service.

Finally start the kube-apiserver service. Your cluster should now be back in the original state.

#### Working with ETCDCTL

etcdctl is a command line client for etcd.

In all our Kubernetes Hands-on labs, the ETCD key-value database is deployed as a static pod on the master. The version used is v3.

To make use of etcdctl for tasks such as back up and restore, make sure that you set the ETCDCTL_API to 3.

You can do this by exporting the variable ETCDCTL_API prior to using the etcdctl client. This can be done as follows:

export `ETCDCTL_API=3`

On the Master Node:

![ETCD](Image/CKA-64.png)

To see all the options for a specific sub-command, make use of the `-h or --help flag`.

For example, if you want to take a snapshot of etcd, use:

`etcdctl snapshot save -h` and keep a note of the mandatory global options.

Since our ETCD database is TLS-Enabled, the following options are mandatory:

| --cacert                     | verify certificates of TLS-enabled secure servers using this CA bundle |
| ---------------------------- | ------------------------------------------------------------ |
| --cert                       | identify secure client using this TLS certificate file       |
| --endpoints=[127.0.0.1:2379] | This is the default as ETCD is running on master node and exposed on localhost 2379. |
| --key                        | identify secure client using this TLS key file               |

Similarly use the help option for snapshot restore to see all available options for restoring the backup.

`etcdctl snapshot restore -h`

For a detailed explanation on how to make use of the etcdctl command line tool and work with the -h flags, check out the solution video for the Backup and Restore Lab.

- Reference

[Backing up an etcd cluster](https://kubernetes.io/docs/tasks/administer-cluster/configure-upgrade-etcd/#backing-up-an-etcd-cluster)

[Recovey](https://github.com/etcd-io/website/blob/main/content/en/docs/v3.5/op-guide/recovery.md)

[Video](https://www.youtube.com/watch?v=qRPNuT080Hk)

### Security

#### Kubernetes Security Primitives

we will discuss about security primitives in Kubernetes.

Kubernetes being the go to platform for hosting production grade applications. Security is of primary concern.

![Security](Image/CKA-66.png)

In this tutorial we discuss the various security primitives in Kubernetes at a high level before diving deeper into those in the upcoming tutorials.

Let’s begin with the host that formed the cluster itself. Of course all access to these hosts must be secured, root access disabled, password based authentication disabled, and only SSH key based authentication to be made available.

![Security](Image/CKA-67.png)

And of course any other measures you need to take to secure your physical or virtual infrastructure that hosts Kubernetes. Of course if that is compromised, everything is compromised.

Our focus in this tutorial is more on Kubernetes related security. What are the risks and what measures do you need to take to secure the cluster.

As we have seen already, the Kube API server is at the center of all operations within Kubernetes.

We interact with it through the kubectl utility or by accessing the API directly and through that you can perform almost any operation on the cluster.

So that’s the first line of defense. Controlling access to the API server itself. We need to make two types of decisions. Who can access the cluster? and What can they do?

- Who can access?

Who can access the API server is defined by the Authentication mechanisms.

![Security](Image/CKA-68.png)

![Security](Image/CKA-69.png)

There are different ways that you can authenticate to the API server. Starting with user IDs and passwords stored in a static file, to tokens, certificates or even integration with external authentication providers like LDAP.

Finally for machines we create service accounts. We will look at these in more detail in the upcoming tutorials.

Once they gain access to the cluster, What can they do is defined by authorization mechanisms.

Authorization is implemented using Role Based Access Control, where users are associated to groups with specific permissions.

In addition there are other authorization modules like Attribute based access control, Node Authorizers, webhooks etc.

All communication with the cluster, between the various components such as the ETCD cluster, kube controller manager, scheduler, api server, as well as those running on the worker nodes such as the kubelet and kubeproxy is secured using TLS Encryption.

![Security](Image/CKA-65.png)

Security Primitives
We have a section entirely for this where we discuss and practice how to setup the certificates between the various components.

What about communication between applications within the cluster?

By default all PODs can access all other PODs within the cluster. You can restrict access between them using Network Policies.

#### Authentication

we are going to discuss about authentication in a Kubernetes cluster.

As we have discussed already the Kubernetes cluster consists of multiple nodes physical/virtual and various components that work together.

![Auth](Image/CKA-70.png)

Kubernetes authentication
We have users like,

1. Administrators that access the cluster to perform administrative tasks
2. Developers that access to cluster to test or deploy applications
3. End users who access the applications deployed on the cluster
4. Third party applications accessing the cluster for integration purposes.

Throughout this tutorial we will discuss how to secure our Kubernetes cluster by securing the communication between internal components and securing management access to the cluster through authentication and authorization mechanisms.

In this tutorial our focus is on securing access to the Kubernetes cluster with authentication mechanisms.

So we discussed about the different users that may be accessing the cluster security of end users who access the applications deployed on the cluster is managed by the applications themselves internally.

So we will take them out of our discussion. Our focus is on users access to the Kubernetes cluster for administrative purposes.

- Accounts

So we are left with 2 types of users. Humans, such as the Administrators and Developers and Robots such as other processes/services or applications that requires access to the cluster.

Kubernetes does not manage user accounts natively it relies on an external source like a file with user details or certificates or a third party identity service like LDAP to manage these users.

And so you cannot create users in a Kubernetes cluster or view the list of users.

![Auth](Image/CKA-71.png)

However in case of Service Accounts Kubernetes can manage them. You can create and manage service accounts using the Kubernetes API.

We will discuss and practice more about service accounts in further tutorials. For this section we will focus on users in Kubernetes.

All user access is managed by the API server. Weather you are accessing the cluster through kubectl tool or the API directly, all of these requests go through the Kube API Server.

![Auth](Image/CKA-72.png)

The Kube API Server authenticates the requests before processing it. So how does the Kube API Server authenticate?

- Authentication mechanisms

There are different authentication mechanisms that can be configured.

You can have a list of username and passwords in a static password file, or usernames and tokens in a static token file or you can authenticate using certificates.

![Auth](Image/CKA-73.png)

And another option is to connect to third party authentication protocols like LDAP, Kerberos etc. We will discuss at some of these in upcoming tutorials.

Let’s start with static password and token files as it is the easiest to understand.

![Auth](Image/CKA-74.png)

Let’s start with the simplest form of authentication. You can create a list of users and their passwords in a csv file and use that as the source for user information.

The file has 3 columns password, user name and user id.

```sh
ashok123,ashok,u0001
ramu@123,ramu,u0002
lakshman@321,lakshman,u0003
seetha@12345,seetha,u0004
hanuma@123,hanuma,u0005
```

We then pass the file name as an option to the Kube API Server. (kube-apiserver.service file)

`--basic-auth-file=user-details.csv`

You must then restart the Kube API Server for these options to take effect.

If you setup your cluster using the kubeadm tool, then you must modify the Kube API Server POD definition file.

![Auth](Image/CKA-75.png)

Kubeadm tool will automatically restart the Kube API Server once you update the file.

To authenticate using the basic credentials while accessing the API server specify the user and password in a curl command like this.

```sh curl -v -k https://10.0.1.2:6443/api/v1/pods -u "ashok:ashok123"```

![Auth](Image/CKA-76.png)

In the csv file with the user details that we saw we can optionally have a fourth column with the group details to assign users to specific groups.

```sh
ashok123,ashok,u0001,group1
ramu@123,ramu,u0002,group1
lakshman@321,lakshman,u0003,group2
seetha@12345,seetha,u0004,group2
hanuma@123,hanuma,u0005,group2
```

Similarly instead of a static password file, You can have a static token file here instead of password you specify a token pass the token file as an option token-auth-file to the Kube API Server.

```sh
eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9,ashok,u0001,group1
eyJtZXNzYWdlIjoiSldUIFJ1bGVzISIsImlhdCI6M,ramu,u0002,group1
6MTQ1OTQ0ODExOSwiZXhwIjoxNDU5NDU0N,lakshman,u0003,group2
b73C75osbmwwshQNRC7frWUYrqaTjTpza2y4,seetha,u0004,group2
VzISIsImlhdCI6MTQ1OTQ0ODExOSwiZXhwIjoxND,hanuma,u0005,group2
```

`token-auth-file=user-details.csv`

![Auth](Image/CKA-77.png)

While authenticating specify the token as an Authorization bearer token to your requests like this.

```sh curl -v -k https://10.0.1.2:6443/api/v1/pods --header "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9"```

Note

1. This authentication mechanism that stores user names, passwords and tokens in clear text in a static file is not a recommended approach as it is insecure. But I thought this was the easiest way to understand the basics of authentication in Kubernetes.
2. If you were trying this out in a kubeadm setup you must also consider volume mounts to pass in the auth file.

- Article

Setup basic authentication on Kubernetes (Deprecated in 1.19)
Note: This is not recommended in a production environment. This is only for learning purposes. Also note that this approach is deprecated in Kubernetes version 1.19 and is no longer available in later releases

Follow the below instructions to configure basic authentication in a kubeadm setup.

- Create a file with user details locally at /tmp/users/user-details.csv

User File Contents

```sh
password123,user1,u0001
password123,user2,u0002
password123,user3,u0003
password123,user4,u0004
password123,user5,u0005
```

- Edit the kube-apiserver static pod configured by kubeadm to pass in the user details. The file is located at /etc/kubernetes/manifests/kube-apiserver.yaml

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: kube-apiserver
  namespace: kube-system
spec:
  containers:
  - command:
    - kube-apiserver
      <content-hidden>
    image: k8s.gcr.io/kube-apiserver-amd64:v1.11.3
    name: kube-apiserver
    volumeMounts:
    - mountPath: /tmp/users
      name: usr-details
      readOnly: true
  volumes:
  - hostPath:
      path: /tmp/users
      type: DirectoryOrCreate
    name: usr-details
```

- Modify the kube-apiserver startup options to include the basic-auth file

```yaml
apiVersion: v1
kind: Pod
metadata:
  creationTimestamp: null
  name: kube-apiserver
  namespace: kube-system
spec:
  containers:
  - command:
    - kube-apiserver
    - --authorization-mode=Node,RBAC
      <content-hidden>
    - --basic-auth-file=/tmp/users/user-details.csv
```

- Create the necessary roles and role bindings for these users:

```yaml
---
kind: Role
apiVersion: rbac.authorization.k8s.io/v1
metadata:
  namespace: default
  name: pod-reader
rules:
- apiGroups: [""] # "" indicates the core API group
  resources: ["pods"]
  verbs: ["get", "watch", "list"]
---
```

- This role binding allows "jane" to read pods in the "default" namespace.

```yaml
kind: RoleBinding
apiVersion: rbac.authorization.k8s.io/v1
metadata:
  name: read-pods
  namespace: default
subjects:
- kind: User
  name: user1 # Name is case sensitive
  apiGroup: rbac.authorization.k8s.io
roleRef:
  kind: Role #this must be Role or ClusterRole
  name: pod-reader # this must match the name of the Role or ClusterRole you wish to bind to
  apiGroup: rbac.authorization.k8s.io
```

Once created, you may authenticate into the kube-api server using the users credentials

```sh curl -v -k https://localhost:6443/api/v1/pods -u "user1:password123"```

#### TLS Introduction

#### TLS in Basics

#### TLS in Kubernetes

#### TLS in Kubernetes - certificatin details

#### Certificate API

#### Kubeconfig

#### Persistance key/value pair

#### API Groups

#### Authorization

#### Role Based Access Controll

#### Cluster Role and Role Binding

#### Service Account

#### Image Security

#### Security Context

#### Network Polocies

#### Developing Network Policies

### Storage

#### Intoduction to Docker Storage

#### Storage in Docker

#### Volume Driver Plugin in Docker

#### Container Storage Interface

#### Volumes

#### Persistent Volumes

#### Persistent Volume Claims

#### Using PVC's in Pods

#### Application Configuration

#### Additional Topics

#### Storage Class

### Network

#### DNS

#### CoreDNS

#### Network Namespace

#### FAQ

#### Docker Network

#### CNI

#### Cluster Network

#### Pod Network

#### CNI in Kubernetes

#### CNI Weave

#### IP Address Management - Weave

#### Service Network

#### DNS in Kubernetes

#### Core DNS in Kubernetes

#### Ingress

### Design and Install Kubernetes Cluster

#### Design Kubernetes Cluster

#### Choose Kubernetes Infrastructure

#### Configure High Availability

#### ETCD in HA

### Install Kubernets hardway

#### Resources

#### Deploy with Kubeadm

### End to End Test on a kubernets Cluster

### Troubleshooting

#### Application Failure

#### Control Plane Failure

#### Worker Node Failuer

#### Network Troubleshooting

#### Other Topics

##### JSON Path

##### Advance Kubectl Commands

--------------------------------------

AND

--------------------------------------

### **Kubernetes Master Course**

#### Kubernetes Introduction

#### Understanding the Kubernetes Architechture

#### Installing and Maintaining The Kubeadm Cluster

#### Kubernetes Core Concepts

#### Workloads in Kubernetes

#### Scheduling In Kubernetes

#### Configuring Application

#### Networking In Kubernetes

#### Storage In Kubernetes

#### Security In Kubernetes

#### Monitoring and Autoscaling kubernetes Cluster
