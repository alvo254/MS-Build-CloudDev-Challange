
The discipline of operational compliance is the cornerstone for maintaining the balance between security, governance, performance, and cost. Effective operational compliance requires consistency in a few critical processes:

- **Resource consistency**: If all resources are organized the same way and tagged the same way, other management tasks become more manageable.
- **Environment consistency**: If all landing zones are organized the same way, then management and troubleshooting become much more manageable.
- **Resource configuration consistency**: As with resources and landing zones, it's crucial to monitor resource configuration. If a configuration setting is changed, it can trigger an automation job to restore the environment.
- **Resource optimization**: Regular monitoring of resource performance reveals trends in resource utilization and opportunities to optimize the cost and performance of each resource.
- **Update consistency**: All updates to the environment should be done in a scheduled, controlled, and possibly automated way. Controlled change management reduces unnecessary outages and troubleshooting.
- **Remediation automation**: Automation for quick remediation of common incidents is a great way to increase customer satisfaction and minimize outages. However, you should fix known issues by their root causes. Fixing a root cause is often a long process, and automation is a quick fix.

Operational compliance can be fulfilled per workload; for example, in one of your landing zones.

The following table lists some of the Azure tools for operational compliance. Remember that not all of these tools need to be part of the default management baseline.

|Tool|Description|Link to more information|
|---|---|---|
|Azure Automation Update Management|Management and scheduling of updates|[Update Management overview](https://learn.microsoft.com/en-us/azure/automation/update-management/overview)|
|Azure Policy|Policy enforcement to ensure environmental and guest compliance|[Azure Policy overview](https://learn.microsoft.com/en-us/azure/governance/policy/overview)|
|Azure Blueprints|Automated compliance for core services|[Azure Blueprints overview](https://learn.microsoft.com/en-us/azure/governance/blueprints/overview)|
|Azure Automation State Configuration|Automated configuration on the guest OS and some aspects of the environment|[State Configuration overview](https://learn.microsoft.com/en-us/azure/automation/automation-dsc-overview)|