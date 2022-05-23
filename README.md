# azure-resource-management
Info on Azure Resource Management

-------
Video
-------

Resources, Resource Groups & Resource Manager

https://www.youtube.com/watch?v=gIhf-S7BCdo

-------
Management Groups
-------

https://docs.microsoft.com/en-us/azure/governance/management-groups/overview

If your organization has many Azure subscriptions, you may need a way to efficiently manage access, policies, and compliance for those subscriptions. Management groups provide a governance scope above subscriptions. You organize subscriptions into management groups the governance conditions you apply cascade by inheritance to all associated subscriptions.

Management groups give you enterprise-grade management at scale no matter what type of subscriptions you might have. However, all subscriptions within a single management group must trust the same Azure Active Directory (Azure AD) tenant.

For example, you can apply policies to a management group that limits the regions available for virtual machine (VM) creation. This policy would be applied to all nested management groups, subscriptions, and resources, and allow VM creation only in authorized regions.

![image](https://user-images.githubusercontent.com/38502893/169841729-33d3aab9-adb5-4acf-a1a3-726ec329d472.png)

-------
Resource Manager
-------

https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview

Azure Resource Manager is the deployment and management service for Azure. It provides a management layer that enables you to create, update, and delete resources in your Azure account. You use management features, like access control, locks, and tags, to secure and organize your resources after deployment.

![image](https://user-images.githubusercontent.com/38502893/169842487-bc4b5307-842a-4f1f-92e5-037d0bf286a3.png)

* resource - A manageable item that is available through Azure. Virtual machines, storage accounts, web apps, databases, and virtual networks are examples of resources. Resource groups, subscriptions, management groups, and tags are also examples of resources.
* resource group - A container that holds related resources for an Azure solution. The resource group includes those resources that you want to manage as a group. You decide which resources belong in a resource group based on what makes the most sense for your organization. See Resource groups.
* resource provider - A service that supplies Azure resources. For example, a common resource provider is Microsoft.Compute, which supplies the virtual machine resource. Microsoft.Storage is another common resource provider. See Resource providers and types.
* declarative syntax - Syntax that lets you state "Here's what I intend to create" without having to write the sequence of programming commands to create it. ARM templates and Bicep files are examples of declarative syntax. In those files, you define the properties for the infrastructure to deploy to Azure.
* ARM template - A JavaScript Object Notation (JSON) file that defines one or more resources to deploy to a resource group, subscription, management group, or tenant. The template can be used to deploy the resources consistently and repeatedly. See Template deployment overview.
* Bicep file - A file for declaratively deploying Azure resources. Bicep is a language that's been designed to provide the best authoring experience for infrastructure as code solutions in Azure. See Bicep overview.
