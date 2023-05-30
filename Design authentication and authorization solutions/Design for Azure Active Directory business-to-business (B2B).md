
Every organization needs to work with external users. [Azure AD business-to-business (B2B)](https://learn.microsoft.com/en-us/azure/active-directory/external-identities/what-is-b2b) is a feature of Azure AD that enables you to securely collaborate with external partners. Your partner users are invited as guest users. You remain in control of what they have access to, and for how long.

![Diagram that shows how business-to-business users are invited to Azure Active Directory.](https://learn.microsoft.com/en-us/training/wwl-azure/design-authentication-authorization-solutions/media/external-identities.png)

### Things to know about Azure AD B2B

Let's explore how the Azure AD B2B features can support external users in a business-to-business solution for Tailwind Traders.

- With Azure AD B2B, the external partner uses their own identity management solution. Azure AD isn't required.
    
- Tailwind Traders doesn't need to manage the _external_ accounts or passwords.
    
- Tailwind Traders doesn't need to sync the external accounts or manage the account lifecycles.
    
- External users use their identities to collaborate with the Tailwind Traders organization. The identities are managed by the partner themselves, or by another external identity provider on their behalf.
    
- Guest users sign in to the Tailwind Traders apps and services with their own work, school, or social identities.
    
- Azure AD B2B makes it possible for Tailwind Traders to collaborate with external partner users.
    
    ![Diagram that shows how guest users are invited to Azure Active Directory.](https://learn.microsoft.com/en-us/training/wwl-azure/design-authentication-authorization-solutions/media/business-to-business-guest-users.png)
    
    1. External users are invited as guest users to access the Tailwind Traders directory. You might fill in a form with the guest user's details and send them a custom invitation message.
        
    2. The guest user receives the Tailwind Traders invitation via email. The first time the invite link is used, the user is asked for consent. The user must accept the permissions needed by Azure AD B2B before they can gain access to Tailwind Traders.
        
    3. If you enabled multifactor authentication (MFA), the user provides the extra details for their account. When MFA is configured, the user must enter a verification code sent to their mobile device before they're granted access.
        
    4. The guest user is then forwarded to the access panel page for Tailwind Traders. The page shows all the apps and services that you shared with that user. These apps and services can be cloud-based, or on-premises.
        

### Things to consider when using Azure AD B2B

Tailwind Traders wants to provide identity management for partners, external vendors, and guest users. As the CTO, you'd like to use Azure AD B2B to implement this support. Here are some options to keep in mind.

- **Consider designating an app owner to manage guest users**. (Microsoft recommended) Delegate guest user access to Tailwind Traders app owners because the owners know best who should be given access to their apps.
    
- **Consider conditional access policies to control access**. Define conditional access policies to intelligently grant or deny access to users. Conditional access policies use factors that aren't credential-based. You might make it mandatory for users to be on specific device platforms like Android or Windows. You might block users from accessing Tailwind Traders, if they don't meet the required location criteria.
    
- **Consider the benefits of using MFA**. Set conditional access policies to require an [MFA process](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks), before the user can access Tailwind Traders apps. This action ensures that all users who access an app must pass an extra authentication challenge before accessing the app.
    
- **Consider integration with identity providers**. Integrate with identity providers so external users can sign in by using an existing account. Azure AD supports external identity providers like Facebook, Microsoft accounts, Google, or enterprise identity providers. You can set up federation for Tailwind Traders with identity providers so external users can use their existing social or enterprise account. External users won't have to create a new account just to access your Tailwind Traders apps.
    
- **Consider self-service sign-up user flow**. Create a self-service sign-up user flow for external users who want to access your Tailwind Traders apps. As part of the sign-up flow, you can provide options for different social or enterprise identity providers, and collect information about the user. You can also customize the onboarding experience for B2B guest users.