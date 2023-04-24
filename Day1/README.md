# KubeWeek Challenge Day 1

Kubernetes Architecture and Components, Kubernetes Installation and Configuration.


## Getting Started With Kubernetes and It's Architecture

Kubernetes is an open-source container orchestration platform that automates the deployment, scaling, and management of containerized applications. It was originally developed by Google and is now maintained by the Cloud Native Computing Foundation (CNCF).

![My Image](https://www.upgrad.com/blog/wp-content/uploads/2020/10/Kubernetes-architecture-1536x1046.png)

## API Server
- API server is the component that provides the Kubernetes API, which is the primary interface for interacting with a Kubernetes cluster.
- Managing the state of the Kubernetes API objects, such as Pods, Deployments, and Services.
- Validating and authorizing API requests, to ensure that they are authorized and meet the requirements of the Kubernetes API.
- Serving as the primary point of contact for Kubernetes clients, including kubectl and Kubernetes Dashboard.
- Providing authentication and authorization services for Kubernetes clients and other Kubernetes components.
- Serving as the entry point for Kubernetes extensions and plugins, such as Custom Resource Definitions (CRDs) and admission controllers.

## Scheduler
- Scheduler is the component that is responsible for scheduling workloads, such as Pods, onto the available nodes in a Kubernetes cluster.
- Selecting the nodes that the workload should be scheduled on, based on the resource requirements and constraints of the workload, as well as the availability of resources on the nodes.
- Ensuring that the workload is scheduled in a way that maximizes the overall resource utilization of the cluster, while also balancing the workload across the available nodes.
- Taking into account various factors that may affect scheduling decisions, such as the availability of network resources, the availability of specific hardware or software features, and any user-defined scheduling preferences.

## Controller-Manager
- Controller-manager is a component of the control plane that runs a set of controllers that are responsible for managing the state of various Kubernetes objects and ensuring that the desired state of the cluster is maintained.
- Replication controller: Ensures that a specified number of replicas of a pod are running at any given time.
- Replica set controller: Similar to the replication controller, but supports more advanced features such as selector-based matching and rolling updates.
- Deployment controller: Manages the deployment of new versions of an application, including rolling updates and rollback capabilities.
- Stateful set controller: Manages the deployment of stateful applications, such as databases, that require stable network identities and persistent storage.
- Daemon set controller: Ensures that a specified pod runs on all nodes in a cluster.
- Job controller: Manages the execution of short-lived, batch-oriented workloads.

## etcd
- etcd is a distributed key-value store that is used to store the state of the cluster, including information about the Kubernetes API objects such as Pods, Services, and Deployments.
- Etcd is a reliable and highly available database that provides a consistent and fault-tolerant way to store and retrieve data.
- Etcd is a standalone database that is designed to be used by distributed systems like Kubernetes.
- The Kubernetes API server communicates with etcd to store and retrieve the state of the cluster.
