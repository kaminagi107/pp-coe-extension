# pp-coe-extension
This samples is a component for exntending [Microsoft Power Platform Center of Excellence (CoE) Starter Kit](https://github.com/microsoft/coe-starter-kit).

# Updates
Version | Notes
-|-
v1.0.0 | New version of CoE Starter Kit Extension. This release contains a flow for sync "Data Gateways" in your organization.

## Sync Template (Data Gateways)

### What this component can do
The flow records the Data Gateways in the organization to Microsoft Dataverse table. (Currently only name, id and type)

### Prerequisite
If you use this component, create Azure AD App for Power BI REST APIs from [here](https://dev.powerbi.com/apps).

**Required API access**
- Read all gateways

### Custom connector security setting example
**Authentication type**
- OAuth 2.0

Item | Value
-|-
ID Provider | Azure Active Directory
Client id | {Your Azure AD App id}
Client secret | {Your Azure AD App secret}
Login URL | https://login.windows.net
Tenant ID | {Your tenant id}
Resource URL | https://analysis.windows.net/powerbi/api
Enable on-behalf-of login | false
Scope | openid
