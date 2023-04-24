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

## Controller-Manager

## etcd
