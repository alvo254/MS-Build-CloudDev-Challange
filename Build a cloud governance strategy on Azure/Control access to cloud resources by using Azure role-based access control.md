## How is role-based access control applied to resources?

Role-based access control is applied to a _scope_, which is a resource or set of resources that this access applies to.

Here's a diagram that shows the relationship between roles and scopes.

![A diagram showing scopes along the Y axis and roles across the X axis. Role and scope combinations each map to a specific kind of user or account, such as an observer or an administrator.](https://learn.microsoft.com/en-us/training/azure-fundamentals/build-cloud-governance-strategy-azure/media/4-role-scope-0223bfae.png)

When you grant access at a parent scope, those permissions are inherited by all child scopes. For example:

- When you assign the [Owner](https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles#owner) role to a user at the management group scope, that user can manage everything in all subscriptions within the management group.
- When you assign the [Reader](https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles#reader) role to a group at the subscription scope, the members of that group can view every resource group and resource within the subscription.
- When you assign the [Contributor](https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles#contributor) role to an application at the resource group scope, the application can manage resources of all types within that resource group, but not other resource groups within the subscription.


## How is Azure RBAC enforced?

Azure RBAC is enforced on any action that's initiated against an Azure resource that passes through Azure Resource Manager. Resource Manager is a management service that provides a way to organize and secure your cloud resources.

You typically access Resource Manager from the Azure portal, Azure Cloud Shell, Azure PowerShell, and the Azure CLI. Azure RBAC doesn't enforce access permissions at the application or data level. Application security must be handled by your application.

RBAC uses an _allow model_. When you're assigned a role, RBAC _allows_ you to perform certain actions, such as read, write, or delete. If one role assignment grants you read permissions to a resource group and a different role assignment grants you write permissions to the same resource group, you have both read and write permissions on that resource group.

## Who does Azure RBAC apply to?

You can apply Azure RBAC to an individual person or to a group. You can also apply Azure RBAC to other special identity types, such as service principals and managed identities. These identity types are used by applications and services to automate access to Azure resources.

## How do I manage Azure RBAC permissions?

You manage access permissions on the **Access control (IAM)** pane in the Azure portal. This pane shows who has access to what scope and what roles apply. You can also grant or remove access from this pane.

The following screenshot shows an example of the **Access control (IAM)** pane for a resource group. In this example, Alain Charon has been assigned the **Backup Operator** role for this resource group.

![A screenshot that shows the Access Control Role Assignment pane. In the Access Control pane, settings and permissions for a user are shown.](https://learn.microsoft.com/en-us/training/azure-fundamentals/build-cloud-governance-strategy-azure/media/4-role-based-access-control-blade-360b5130.png)