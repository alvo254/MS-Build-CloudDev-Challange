To begin using Azure Storage, you first create an Azure Storage account to store your data objects. You can create an Azure Storage account by using the Azure portal, PowerShell, or the Azure CLI.

![Screenshot of creating a storage account.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-storage-fundamentals/media/create-storage-account-1c42138c.png)

Your storage account will contain all of your Azure Storage data objects, such as blobs, files, and disks.

 Note

Azure VMs use Azure Disk Storage to store virtual disks. However, you can't use Azure Disk Storage to store a disk outside of a virtual machine.  

![Diagram of hierarchy of a storage account.](https://learn.microsoft.com/en-us/training/azure-fundamentals/azure-storage-fundamentals/media/account-container-blob-4da0ac47.png)

A storage account provides a unique namespace for your Azure Storage data, that's accessible from anywhere in the world over HTTP or HTTPS. Data in this account is secure, highly available, durable, and massively scalable.

For more information, see [Create a storage account](https://learn.microsoft.com/en-us/azure/storage/common/storage-account-create).