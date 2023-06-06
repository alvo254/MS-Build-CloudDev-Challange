
Individual security team members must see themselves as part of a security team that's part of the whole organization. They're also part of a larger security community that defends against the same adversaries. This holistic view enables the team to work well in general. It's especially important as teams work through any unplanned gaps and overlaps discovered during the evolution of roles and responsibilities.

## Security responsibilities (functions)

This diagram depicts the specific organizational functions within security. It represents an ideal view of a complete enterprise security team and might be an aspirational view for some security teams. Each function can be performed by one or more people. Each person can perform one or more functions based on factors like culture, budget, and available resources.

[![A diagram that illustrates the organizational functions within security.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-security/media/security-organizational-functions.png)](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-security/media/security-organizational-functions.png#lightbox)

The following articles provide information about each function and include a summary of objectives. They discuss how the function can evolve because of the threat environment or cloud technology changes. They also explore the relationships and dependencies that are critical to the function's success:

- [Policy and standards](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-policy-standards)
- [Security operations](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-operations-center)
- [Security architecture](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-architecture)
- [Security compliance management](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-compliance-management)
- [People security](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-people)
- [Application security and DevSecOps](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-application-security-devsecops)
- [Data security](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-data-security)
- [Infrastructure and endpoint security](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-infrastructure-endpoint)
- [Identity and key management](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-identity-keys)
- [Threat intelligence](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-threat-intelligence)
- [Posture management](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-posture-management)
- [Incident preparation](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security-incident-preparation)

The following diagram summarizes the roles and responsibilities in a security program to help you familiarize yourself with these roles.

[![A diagram that summarizes the roles and responsibilities of a security program.](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-security/media/security-roles-responsibilities.png)](https://learn.microsoft.com/en-us/training/modules/cloud-adoption-framework-security/media/security-roles-responsibilities.png#lightbox)

For more information, see [Cloud security functions](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/organize/cloud-security).

## Map security to business outcomes

At the organizational level, the security disciplines map to standard plan-build-run phases seen widely across industries and organizations. This cycle is accelerating into a continuous change cycle with the digital age and the advent of DevOps. It also illustrates how security maps to normal business processes.

Security is a discipline with its own unique functions. A critical element is integration into normal business operations.

## Role types

In the preceding diagram, the dark labels group these responsibilities into typical roles that have common skill sets and career profiles. These groupings also help provide clarity on how industry trends affect security professionals:

- **Security leadership**: These roles frequently span across functions. They ensure that teams coordinate with each other, prioritize, and set cultural norms, policies, and standards for security.
- **Security architect**: These roles span across functions and provide a key governance capability to ensure all the technical functions work harmoniously within a consistent architecture.
- **Security posture and compliance**: This newer role type represents the increasing convergence of compliance reporting with traditional security disciplines like vulnerability management and configuration baselines. While the scope and audience are different for security and compliance reporting, they answer different versions of the question "How secure is the organization?" The way that question is answered is growing more similar via tools like Microsoft Secure Score and Microsoft Defender for Cloud:
    - The use of on-demand data feeds from cloud services reduces the time required to report compliance.
    - The increased scope of data available enables security governance to look beyond traditional software updates or patches and discover and track "vulnerabilities" from security configurations and operational practices.
- **Platform security engineer**: These technology roles focus on platforms that host multiple workloads, focused on access control and asset protection. These roles are often grouped into teams with specialized technical skill sets. They include network security, infrastructure and endpoints, and identity and key management. These teams work on preventive controls and detective controls, with detective controls being a partnership with SecOps and preventive controls being primarily a partnership with IT operations. For more information, see [Security integration](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/secure/security-integration).
- **Application security engineer**: These technology roles focus on security controls for specific workloads and support classic development models and modern DevOps/DevSecOps model. They blend application and development security skills for unique code and infrastructure skills for common technical components like VMs, databases, and containers. These roles might be in central IT or security organizations or within business and development teams based on organizational factors.

## Modernization

Security architecture is affected by different factors:

- **Continuous engagement model**: Continuous release of software updates and cloud features makes fixed engagement models obsolete. Architects should be engaged with all teams working in technical topic areas to guide decision making along those teams' capability lifecycles.
- **Security from the cloud**: Incorporate security capabilities from the cloud to reduce enablement time and ongoing maintenance costs like hardware, software, time, and effort.
- **Security of the cloud**: Ensure coverage of all cloud assets including software as a service (SaaS) applications, infrastructure as a service (IaaS) VMs, and platform as a service (PaaS) applications and services. Include discovery and security of both sanctioned and unsanctioned services.
- **Identity integration**: Security architects should ensure tight alignment with identity teams to help organizations meet the dual goals of enabling productivity and providing security assurances.
- **Integration of internal context in security designs such as context from posture management and incidents investigated by security operations [center]**: Include elements like relative risk scores of user accounts and devices, sensitivity of data, and key security isolation boundaries to actively defend.

## Recommended content

- [Microsoft Cybersecurity Reference Architectures (MCRA) - People](https://aka.ms/MCRA-IG-People) An interactive training guide for people who are new to security.
- [MCRA Security Roles - YouTube](https://www.youtube.com/watch?v=GlqjvlX93gY&list=PLtVMyW0H7aiOQwZSsn2d-tg2z729ce1BZ&index=13) Overview of the roles and responsibilities in a security program. Includes a discussion of how they're evolving to meet the needs of modern attacks, cloud technology, and Zero Trust principles. This top-to-bottom view of roles includes the board and executives.