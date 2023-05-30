
[Conditional Access](https://learn.microsoft.com/en-us/azure/active-directory/conditional-access/overview) is a tool that Azure Active Directory uses to allow (or deny) access to resources. When a user signs in, Conditional Access examines who the user is, where the user is, and from what device the user is requesting access. Based on these signals, Conditional Access can allow access, enforce multifactor authentication (MFA), or deny access.

![Diagram that shows how the Conditional Access tool evaluates conditions and determines access.](https://learn.microsoft.com/en-us/training/wwl-azure/design-authentication-authorization-solutions/media/conditions-actions.png)

### Things to know about Conditional Access

As you plan the solution for Tailwind Traders, review these characteristics of Conditional Access.

- MFA supports granular control. You can use MFA selectively and require it for certain users only.
    
- Azure AD allows named locations to be used with app policies to control access.
    
- Service access can be restricted through approved client apps only.
    
- Access to apps can be limited to [managed devices](https://learn.microsoft.com/en-us/azure/active-directory/conditional-access/concept-condition-filters-for-devices) that meet your security and compliance standards.
    
- Untrusted sources can be blocked, such as sources from an unknown or unexpected location.
    
- [Report-only mode](https://learn.microsoft.com/en-us/azure/active-directory/conditional-access/concept-conditional-access-report-only) helps admins evaluate the impact of Conditional Access policies before enabling them in their environment.
    
- The [What If](https://learn.microsoft.com/en-us/azure/active-directory/conditional-access/what-if-tool) tool helps you plan and troubleshoot Conditional Access policies.
    

 Note

To use Conditional Access, you need an Azure AD Premium P1 or P2 license. If you have a Microsoft 365 Business Premium license, you also have access to Conditional Access features.

### Things to consider when using Conditional Access

Tailwind Traders wants to implement Conditional Access into their identity solution. Review the following scenarios to determine the best options for your use of the Conditional Access tool.

- **Consider MFA for more granular control**. Implement selective MFA and provide a more granular experience for Tailwind Traders users. If a user is from a known location, you might not require extra authentication. For users from unknown or unexpected locations, you can challenge them to supply the second authentication factor.
    
- **Consider preventing access from specific geographic areas**. Exclude geographic areas that you don't expect Tailwind Traders to interact with. Use Azure AD to create named locations for the geographic areas. Create a policy for all apps to block sign-in attempts from the named locations. Be sure to exempt your admins from this policy!
    
- **Consider access only from managed devices**. Tailwind Traders supports access to their cloud resources from a proliferation of devices, which helps user productivity. Protect the environment by restricting devices with an unknown protection level to access only certain resources. Require user access from only managed devices that meet Tailwind Traders standards for security and compliance.
    
- **Consider access only from approved client apps.** Protect Tailwind Traders corporate data by enabling access to services through approved client apps only. Employees use their mobile devices for both personal and work tasks. You must decide whether to manage the entire device or just the data on it. If you manage only the data and access, you can require access from only approved cloud apps.
    
- **Consider using policies to handle compromised accounts.** Enable one or more default policies to handle compromised accounts:
    
    - Require all users to register for MFA.
    - Require a password change for users who are high-risk.
    - Require MFA for users with medium or high sign-in risk.
- **Consider blocking access.** Block access to override all other assignments for a user. You can block your entire Tailwind Traders organization from signing on to your tenant. Blocking can be helpful when you're migrating an app to Azure AD, but you aren't ready for anyone to sign-in yet. You can also block certain network locations from accessing your cloud apps, or block apps that use legacy authentication from accessing your tenant resources.
    
- **Consider blocking legacy authentication protocols**. Attackers exploit weaknesses in older protocols every day, particularly for password spray attacks. Configure Conditional Access to [block legacy protocols](https://learn.microsoft.com/en-us/azure/active-directory/conditional-access/howto-conditional-access-policy-block-legacy) from accessing Tailwind Traders apps.
    
- **Consider running Report-only mode**. Run Report-only mode to predict the number and names of Tailwind Traders users who will be affected by common deployment initiatives. Use Report-only mode to test blocking legacy authentication, requiring MFA, and implementing sign-in risk policies.
    
- **Consider using the What If tool**. Use the What If tool to test your proposed Conditional Access policies before you implement them.
