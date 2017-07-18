---
title: "Azure Resource Manager"
date: 2017-07-18T14:19:32-07:00
menu: "Main"
---

Azure resource manager is the platform through which azure provisions resources. Resources can be provisioned using `Azure CLI, Azure Portal, Powershell or Azure resource manager templates`. Behind the scene, all these tools interact with azure resource manager platform to provision the resources. 

```cs
public interface IAzure 
{
    void AzureResourceManager();
    void AzureNetworking();
}
```

Azure resource manager does not directly provision resources. It goes through azure resource providers to help it get the job done. Azure resource providers all the details related to the specific resource that needs to be provisioned. All resources within azure belong to a resource provider. For example storage is provided by Microsoft.AzureStorage, network related resources are provided by Microsoft.AzureNetworking etc.

![Image of something](http://via.placeholder.com/725x150/bf616a.jpg)

