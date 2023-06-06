
## Build governance maturity

This unit explains the four-step process in the Cloud Adoption Framework to build a mature cloud-governance solution:

1. **Methodology**: Understand the underlying methodology
2. **Governance benchmark**: Assess your current-state and future-state needs
3. **Governance foundation**: Establish your governance foundation by using a set of governance tools
4. **Mature governance disciplines**: Iteratively add governance controls to address risks

These steps will get you started using the Govern methodology in the cloud. They also will set you on a path to mature each governance discipline as your cloud adoption plan progresses.

## Govern methodology

The Govern methodology provides a structured approach to building the governance maturity that's required for confidence in cloud adoption.

![Image that identifies the five disciplines of cloud governance and the components of the corporate policy process.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-govern/media/methodology.png)

_Figure 1: The Govern methodology: define corporate policy and the five disciplines of cloud governance._

## Corporate policy

_Governance_ is a big topic, and it might be intimidating at first. Governance seeks to establish the proper scope of corporate actions by mitigating tangible risks through corporate policy.

Corporate policies drive cloud governance. Proper corporate policy consists of three components:

- **Business risk**: Identify and understand tangible corporate risks and the organization's tolerance for risk
- **Policy and compliance**: Convert risks into clear policy statements that support compliance requirements without defining specific technical dependencies
- **Process**: Establish processes to monitor violations and ensure adherence to policy statements

A focus on these components helps develop clear and actionable corporate policies. In the next unit, you'll see how to develop a proper corporate policy.

## Governance disciplines

Governance disciplines support corporate policies through a mixture of tools and human processes. Each of the following disciplines protects the organization from specific, defined potential pitfalls:

- **Cost Management discipline**: Optimize costs across a broad portfolio of workloads through the application of budgets, reports, and automated enforcement
- **Security Baseline discipline**: Apply well-defined security requirements to all supported environments and underlying workloads
- **Resource Consistency discipline**: Manage resource configuration at scale to ensure that all deployed assets are discoverable, recoverable, and onboarded into operation management processes
- **Identity Baseline discipline**: Ensure proper authentication and access by applying roles and assignments to each environment
- **Deployment Acceleration discipline**: Standardize and centralize deployment templates to ensure consistency across all environments and workloads

Each discipline accelerates the application of corporate policies and ensures consistent governance. Later in this module, we'll investigate actionable implementation for each discipline.

## Governance benchmark tool

The Cloud Adoption Framework provides a [governance benchmark tool](https://cafbaseline.com/) to help you identify gaps in the governance disciplines and corporate policy in your organization.

![Image of a computer monitor that displays a line chart and a pie chart in a results webpage from the Cloud Adoption Framework benchmark tool.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-govern/media/benchmark.png)

_Figure 2: A governance benchmark output that shows areas for improvement and a comparison between current state and future state governance requirements._

You can use the governance benchmark tool for a personalized report that outlines the difference between your current state and business priorities, along with tailored resources to help you start assessing your current state and future state and establish a vision for applying the framework.

## Governance foundation

Azure includes a suite of governance tools that are built on top of the Azure Resource Manager platform. The initial governance foundation demonstrates how you can apply these tools to demonstrate cloud governance. As you progress through the units of this module, you'll learn how to apply these tools to solve governance challenges. First, start with a governance foundation to familiarize yourself with the tools.

![Image of the Azure Resource Manager tools that support governance, with a focus on Azure Policy and Azure Blueprints.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-govern/media/3-tdd-in-azure.png)

_Figure 3: The Azure Resource Manager tools that support governance, with a focus on Azure Policy and Azure Blueprints._

In later units, you'll apply these tools to create a governance foundation for Tailwind Traders.

The Cloud Adoption Framework contains two ways to apply a sound foundation for governance to new or existing deployments. Each provides a different approach to support your business needs when you get started:

- [Standard governance guide](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/standard/): A guide for most organizations that's based on the recommended initial two-subscription model, and designed for deployments in multiple regions while not spanning public and sovereign/government clouds
- [Governance guide for complex enterprises](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/complex/): A guide for enterprises that are managed by multiple independent IT business units or span public and sovereign/government clouds

## Mature governance disciplines

A governance foundation introduces you to tools that are needed to implement proper governance. To achieve sustainable governance, you'll need to apply guardrails for each governance discipline. To be more precise and more effective, teams should start with a single discipline and expand over time. The following table can help mature the disciplines that are needed to meet specific business objectives:

|Risk/need|Standard enterprise|Complex enterprise|
|---|---|---|
|Sensitive data in the cloud|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/standard/security-baseline-improvement)|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/complex/security-baseline-improvement)|
|Mission-critical applications in the cloud|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/standard/resource-consistency-improvement)|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/complex/resource-consistency-improvement)|
|Cloud cost management|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/standard/cost-management-improvement)|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/complex/cost-management-improvement)|
|Multicloud|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/standard/multicloud-improvement)|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/complex/multicloud-improvement)|
|Complex/legacy identity management|N/A|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/complex/identity-baseline-improvement)|
|Multiple layers of governance|N/A|[Discipline improvement](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/govern/guides/complex/multiple-layers-of-governance)|