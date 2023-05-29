Azure compute is an on-demand computing service for running cloud-based applications. It provides computing resources such as disks, processors, memory, networking, and operating systems. The resources are available on-demand and can typically be made available in minutes or even seconds. You pay only for the resources you use, and only for as long as you're using them.

Azure supports a wide range of computing solutions for development and testing, running applications, and extending your datacenter. The service supports Linux, Windows Server, SQL Server, Oracle, IBM, and SAP. Azure also has many services that can run virtual machines (VMs). Each service provides different options depending on your requirements. Some of the most prominent services are:

- Azure Virtual Machines
- Azure Container Instances
- Azure App Service
- Azure Functions (or _serverless computing_)

![Screenshot of the Azure portal compute services page that includes VMs and containers.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-compute-fundamentals/media/compute-services-13e531e1.png)

**Virtual machines**

Virtual machines are software emulations of physical computers. They include a virtual processor, memory, storage, and networking resources. VMs host an operating system, and you can install and run software just like a physical computer. When using a remote desktop client, you can use and control the VM as if you were sitting in front of it.

With [Azure Virtual Machines](https://azure.microsoft.com/services/virtual-machines/), you can create and use VMs in the cloud. Virtual Machines provides infrastructure as a service (IaaS) and can be used in different ways. When you need total control over an operating system and environment, VMs are an ideal choice. Just like a physical computer, you can customize all the software running on the VM. This ability is helpful when you're running custom software or custom hosting configurations.

![Icon representing virtual machines.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-compute-fundamentals/media/icon-virtual-machine-863c3e59.png)

![Icon representing virtual machine scale sets.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-compute-fundamentals/media/icon-scale-sets-8682cc12.png)

**Virtual machine scale sets**

[Virtual machine scale sets](https://azure.microsoft.com/services/virtual-machine-scale-sets) are an Azure compute resource that you can use to deploy and manage a set of identical VMs. With all VMs configured the same, virtual machine scale sets are designed to support true autoscale. No pre-provisioning of VMs is required. For this reason, it's easier to build large-scale services targeting big compute, big data, and containerized workloads. As demand goes up, more VM instances can be added. As demand goes down, VM instances can be removed. The process can be manual, automated, or a combination of both.

**Containers and Kubernetes**

[Container Instances](https://azure.microsoft.com/services/container-instances) and [Azure Kubernetes Service](https://azure.microsoft.com/services/kubernetes-service) are Azure compute resources that you can use to deploy and manage containers. Containers are lightweight, virtualized application environments. They're designed to be quickly created, scaled out, and stopped dynamically. You can run multiple instances of a containerized application on a single host machine.

![Icon representing containers and Kubernetes.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-compute-fundamentals/media/icon-container-instance-7b714f67.png)

![Icon representing Azure App Service.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-compute-fundamentals/media/icon-app-service-9aa4dd22.png)

**App Service**

With [Azure App Service](https://azure.microsoft.com/services/app-service), you can quickly build, deploy, and scale enterprise-grade web, mobile, and API apps running on any platform. You can meet rigorous performance, scalability, security, and compliance requirements while using a fully managed platform to perform infrastructure maintenance. App Service is a platform as a service (PaaS) offering.

**Functions**

[Functions](https://azure.microsoft.com/services/functions) are ideal when you're concerned only about the code running your service and not the underlying platform or infrastructure. They're commonly used when you need to perform work in response to an event (often via a REST request), timer, or message from another Azure service, and when that work can be completed quickly, within seconds or less.