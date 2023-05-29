
Containers are a virtualization environment. Much like running multiple virtual machines on a single physical host, you can run multiple containers on a single physical or virtual host. Unlike virtual machines, you don't manage the operating system for a container. Virtual machines appear to be an instance of an operating system that you can connect to and manage, but containers are lightweight and designed to be created, scaled out, and stopped dynamically. While it's possible to create and deploy virtual machines as application demand increases, containers are designed to allow you to respond to changes on demand. With containers, you can quickly restart in case of a crash or hardware interruption. One of the most popular container engines is Docker, which is supported by Azure.

## Manage containers

Containers are managed through a container orchestrator, which can start, stop, and scale out application instances as needed. There are two ways to manage both Docker and Microsoft-based containers in Azure: Azure Container Instances and Azure Kubernetes Service (AKS).

**Azure Container Instances**

[Azure Container Instances](https://azure.microsoft.com/services/container-instances) offers the fastest and simplest way to run a container in Azure without having to manage any virtual machines or adopt any additional services. It's a platform as a service (PaaS) offering that allows you to upload your containers, which it runs for you.

![Icon representing Azure Container Instances.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-compute-fundamentals/media/icon-container-instance-7b714f67.png)

![Icon representing Azure Kubernetes Service.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-compute-fundamentals/media/icon-kubernetes-a0946004.png)

**Azure Kubernetes Service**

The task of automating, managing, and interacting with a large number of containers is known as orchestration. [Azure Kubernetes Service](https://azure.microsoft.com/services/kubernetes-service) is a complete orchestration service for containers with distributed architectures and large volumes of containers.

## Use containers in your solutions

Containers are often used to create solutions by using a _microservice architecture_. This architecture is where you break solutions into smaller, independent pieces. For example, you might split a website into a container hosting your front end, another hosting your back end, and a third for storage. This split allows you to separate portions of your app into logical sections that can be maintained, scaled, or updated independently.

Imagine your website back-end has reached capacity but the front end and storage aren't being stressed. You could:

- Scale the back end separately to improve performance.
- Decide to use a different storage service.
- Replace the storage container without affecting the rest of the application.

