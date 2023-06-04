
You've deployed your application by using infrastructure and services that are as cost-effective as possible. But what do you do when your business, customer demand, or application changes? How do you ensure that your costs aren't growing out of control relative to the resources that are required to run them? How do you detect areas to improve efficiency in your environment? Architectures aren't static, resource demands will shift over time, and cloud services will evolve to introduce new features and cost savings.

## Track your cloud spend

To make intelligent decisions, you need data. By analyzing where your money is going, you can compare your costs to your utilization to discover where you might have waste within your environment.

You can export billing data at any time. By using your billing data, you can track where your costs are going and how they're allocated across your resources. One challenge for you is that the billing data shows your costs, but not your utilization. You'll have data that indicates you're paying for a large VM, but how much are you actually using it?

Microsoft Cost Management gives you insights into where your spend is going, as well as underutilized resources. Microsoft Cost Management tracks your total spend, cost by service, and cost over time. You can drill down into resource types and instances. You can also break down your costs by organization or cost center by tagging resources with those categories.

![Screenshot of Microsoft Cost Management.](https://learn.microsoft.com/en-us/training/modules/azure-well-architected-cost-optimization/media/4-grouped-daily-accum-view.png)

Azure Advisor also has a cost component that:

- Recommends VM resizing when necessary.
- Identifies unused Azure ExpressRoute circuits and idle virtual network gateways.
- Advises when to consider buying reserved instances because that might be more cost-effective than using pay-as-you-go instances.

Azure Advisor makes additional recommendations in the areas of performance, high availability, and security.

The important part of optimization is to take time to review your spend and evaluate where your money is going. Effective analysis will help you identify areas of inefficiency and ensure you're operating as cost-effectively as possible.

## Conduct cost reviews

After your Azure services are running, you should regularly check your costs to track your Azure spending. You can use cost analysis to understand where the costs originated for your Azure usage.

![Screenshot of cost analysis in the Azure portal.](https://learn.microsoft.com/en-us/training/modules/azure-well-architected-cost-optimization/media/4-cost-analysis.png)

Take time as an organization to regularly meet and review billing and expenditures that are related to cloud services. Review the respective expenditures with the technical and business stakeholders for each application. This brings increased visibility to the costs that are associated with an application and the decisions made from a cost perspective.

## Respond to cost alerts

One of the key features of Microsoft Cost Management is the ability to configure alerts that are based on spending. These alerts can provide immediate visibility into spending that might be exceeding your budget. You can then take steps to address these costs. There are three types of cost alerts:

- _Budget alerts_ notify you when spending, based on usage or cost, reaches or exceeds the amount defined in the alert condition of the budget. Budgets in Microsoft Cost Management help you plan for and drive organizational accountability.
    
    With budgets, you can account for the Azure services that you consume or subscribe to during a specific period. They help you to proactively inform others about their spending and to monitor how spending progresses over time. When you exceed the budget thresholds that you've created, alerts can be sent to the appropriate teams. You can set budgets at varying levels, from resource groups to subscriptions to enterprise agreements.
    
- _Credit alerts_ notify you when your Azure credit monetary commitments are consumed. Monetary commitments are for organizations with enterprise agreements.
    
- _Department spending quota alerts_ notify you when department spending reaches a fixed threshold of the quota. You can configure spending quotas in the Azure Enterprise Agreement portal. When you meet a threshold, an email is sent to department owners and a notification appears in cost alerts.
    

## Report anomalies

When an anomaly in spending is identified through your data collection, cost reviews, or cost alerts, you should report it to the necessary stakeholders. Active engagement on cost can ensure that you identify a potential for cost overrun before it becomes problematic. Transparency with stakeholders is important so they can fully understand any technical or business decisions that caused abnormal cloud costs.