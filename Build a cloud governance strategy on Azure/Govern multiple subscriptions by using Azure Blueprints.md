
Instead of having to configure features like Azure Policy for each new subscription, with [Azure Blueprints](https://azure.microsoft.com/services/blueprints) you can define a repeatable set of governance tools and standard Azure resources that your organization requires. In this way, development teams can rapidly build and deploy new environments with the knowledge that they're building within organizational compliance with a set of built-in components that speed the development and deployment phases.

Azure Blueprints orchestrates the deployment of various resource templates and other artifacts, such as:

- Role assignments
- Policy assignments
- Azure Resource Manager templates
- Resource groups

## Azure Blueprints in action

When you form a cloud center of excellence team or a cloud custodian team, that team can use Azure Blueprints to scale their governance practices throughout the organization.

Implementing a blueprint in Azure Blueprints involves these three steps:

1. Create an Azure blueprint.
2. Assign the blueprint.
3. Track the blueprint assignments.

With Azure Blueprints, the relationship between the blueprint definition (what should be deployed) and the blueprint assignment (what was deployed) is preserved. In other words, Azure creates a record that associates a resource with the blueprint that defines it. This connection helps you track and audit your deployments.

Blueprints are also versioned. Versioning enables you to track and comment on changes to your blueprint.

## How will Tailwind Traders use Azure Blueprints for ISO 27001 compliance?

[ISO 27001](https://www.iso.org/isoiec-27001-information-security.html) is a standard that applies to the security of IT systems, published by the International Organization for Standardization. As part of its quality process, Tailwind Traders wants to certify that it complies with this standard. Azure Blueprints has several built-in blueprint definitions that relate to ISO 27001.

As an IT administrator, you decide to investigate the **ISO 27001: Shared Services Blueprint** definition. Here's an outline of your plan.

1. Define a management group that's named **PROD-MG**. Recall that a management group manages access, policies, and compliance across multiple Azure subscriptions. Every new Azure subscription is added to this management group when the subscription is created.
2. Create a blueprint definition that's based on the **ISO 27001: Shared Services Blueprint** template. Then publish the blueprint.
3. Assign the blueprint to your **PROD-MG** management group.

The following image shows artifacts that are created when you run an ISO 27001 blueprint from a template.

![Screenshot showing artifacts listed when you create an ISO 27001 blueprint from template.](https://learn.microsoft.com/en-us/training/azure-fundamentals/build-cloud-governance-strategy-azure/media/10-iso-27001-shared-blueprint-dc443de7.png)

You see that the blueprint template contains policy assignments, Resource Manager templates, and resource groups. The blueprint deploys these artifacts to any existing subscriptions within the **PROD-MG** management group. The blueprint also deploys these artifacts to any new subscriptions as they're created and added to the management group.