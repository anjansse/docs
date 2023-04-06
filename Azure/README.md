# Azure Active Directory

Azure Active Directory (Azure AD) is a cloud-based identity and access management (IAM) service that provides authentication and authorization services for applications, services, and devices.
Azure AD can be used to manage users and groups, grant and revoke access to resources, and enforce access policies across cloud-based and on-premises applications.

Azure AD is the direct successor to AD (Active Directory), which was its on-premise equivalent at the time.

## Useful concepts & terminologies

### General

| Concept | Description |
|---------|-------------|
| Identity | A thing that can get authenticated. An identity can be a user with a username and password. Identities also include applications or other servers that might require authentication through secret keys or certificates. |
| Azure tenant | A dedicated and trusted instance of Azure AD. The tenant is automatically created when your organization signs up for a Microsoft cloud service subscription. An Azure tenant represents a single organization. |
| Multi-tenant | Azure tenants that access other services in a shared environment, across multiple organizations, are considered multi-tenant. |
| Single tenant | Azure tenants that access other services in a dedicated environment are considered single tenant. |
| Azure AD directory | Each Azure tenant has a dedicated and trusted Azure AD directory. The Azure AD directory includes the tenant's users, groups, and apps and is used to perform identity and access management functions for tenant resources. |
| Security Principal | Security principals are given permissions within an associated tenant, which define what a user is allowed to access. |
| Service Principal | This is a security principal, but for services rather than users. |

### Azure AD Apps

| Concept | Description |
|---------|-------------|
| Application | Representation of an application (e.g. web-app) in Azure AD. |
| App Registration | Application that have been registered with your Azure AD (yes the name is confusing). |
| App (client) ID | Unique ID of this application in your directory. |
| Tenant ID | Unique ID for the tenant hosting the application. |
| Object ID | Little bit trickier to understand, it's the unique identifier assigned to an Azure AD application that can be used to perform operations on the application and retrieve information about the associated service principal object. |
| Redirect URI | A Redirect URI is a URI used by Azure AD apps to redirect users back to the app after authentication. |

### Typical Auth flow

1. The user navigates to the website and attempts to access a protected resource.
2. The website <u>redirects the user to Azure AD for **authentication**</u>.
3. Azure AD authenticates the user and generates an access token.
4. The access token is sent back to the website, which validates it and grants access to the protected resource.
5. The user is granted access to the resource and can interact with it securely.

### Microsoft Identity Platform

Microsoft Identity Platform is Microsoft's core solution to provide a comprehensive identity and access management system for Microsoft

Azure AD is <u>built on top of the Microsoft Identity Platform</u> and provides additional features and services, such as single sign-on, multi-factor authentication, conditional access policies, and integration with other Microsoft cloud services. Microsoft Identity Platform provides 



## Further Reading

- [Azure AD vs AD](https://learn.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-compare-azure-ad-to-ad)
- [Terminology](https://learn.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-whatis#terminology)
