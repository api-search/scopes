---
api_specs:
- filename: azure-ad-graph-applications-openapi.yml
  format: yaml
  label: Azure Active Directory Applications API
  slug: azure-ad-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-applications-openapi.yml
- filename: azure-ad-graph-identity-directorymanagement-openapi.yml
  format: yaml
  label: Azure Active Directory Directory API
  slug: azure-ad-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-directorymanagement-openapi.yml
- filename: azure-ad-graph-groups-openapi.yml
  format: yaml
  label: Azure Active Directory Groups API
  slug: azure-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-groups-openapi.yml
- filename: azure-ad-me-api-openapi.yml
  format: yaml
  label: Azure Active Directory Me API
  slug: azure-ad-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/azure-ad-me-api-openapi.yml
- filename: azure-ad-graph-users-openapi.yml
  format: yaml
  label: Azure Active Directory Users API
  slug: azure-ad-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-users-openapi.yml
- filename: azure-ad-graph-identity-signins-openapi.yml
  format: yaml
  label: Microsoft Entra ID Sign-Ins and Policies API
  slug: azure-ad-signins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-signins-openapi.yml
- filename: azure-ad-graph-identity-governance-openapi.yml
  format: yaml
  label: Microsoft Entra ID Governance API
  slug: azure-ad-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-governance-openapi.yml
- filename: azure-ad-graph-directoryobjects-openapi.yml
  format: yaml
  label: Microsoft Entra ID Directory Objects API
  slug: azure-ad-directory-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-directoryobjects-openapi.yml
- filename: azure-ad-graph-changenotifications-openapi.yml
  format: yaml
  label: Microsoft Entra ID Change Notifications API
  slug: azure-ad-change-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-changenotifications-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
description: ''
docs: https://learn.microsoft.com/en-us/graph/permissions-reference
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Azure Ad Scopes
name_suffix: OAuth Scopes
note: Microsoft Graph publishes TWO disjoint permission sets for the same resources — delegated (the app acts as a signed-in user, effective access is the intersection of the scope and the user's own privileges) and application (the app acts as itself, admin consent always required, no user context). The `types` field on each entry says which sets a name appears in. The full published catalogue is 583 delegated and 527 application permissions; the entries below are the Entra ID directory subset that this record covers, not the whole list.
overview: 'Microsoft Entra ID (formerly Azure AD) publishes 39 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Entra ID (formerly Azure AD) API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Entra ID (formerly Azure AD)
provider_slug: azure-ad
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    flow: authorizationCode
    permission_set: delegated
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - flow: clientCredentials
    note: Request scope https://graph.microsoft.com/.default; individual scopes are not requested at token time.
    permission_set: application
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - deviceAuthorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/devicecode
    flow: deviceCode
    permission_set: delegated
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: azureaadv2
  sources:
  - openapi/_original/azure-ad-graph-users-openapi.yml
  - well-known/azure-ad-openid-configuration.json
  type: oauth2
scope_count: 39
scope_names:
- openid
- profile
- email
- offline_access
- User.Read
- User.ReadBasic.All
- User.Read.All
- User.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All
- Group.Read.All
- Group.ReadWrite.All
- GroupMember.Read.All
- GroupMember.ReadWrite.All
- Application.Read.All
- Application.ReadWrite.All
- Application.ReadWrite.OwnedBy
- AppRoleAssignment.ReadWrite.All
- RoleManagement.Read.Directory
- RoleManagement.ReadWrite.Directory
- Policy.Read.All
- Policy.ReadWrite.ConditionalAccess
- AuditLog.Read.All
- Device.Read.All
- Device.ReadWrite.All
- EntitlementManagement.Read.All
- EntitlementManagement.ReadWrite.All
- AccessReview.Read.All
- AccessReview.ReadWrite.All
- UserAuthenticationMethod.Read.All
- UserAuthenticationMethod.ReadWrite.All
- PrivilegedAccess.Read.AzureADGroup
- Organization.Read.All
- Domain.Read.All
- AdministrativeUnit.Read.All
- IdentityProvider.Read.All
- IdentityRiskEvent.Read.All
- Subscription.Read.All
scopes:
- description: Allows users to sign in to the app with their work or school accounts and allows the app to see basic user profile information.
  flows: []
  scope: openid
- description: Allows the app to see your users' basic profile (e.g., name, picture, user name, email address)
  flows: []
  scope: profile
- description: Allows the app to read your users' primary email address
  flows: []
  scope: email
- description: Allows the app to see and update the data you gave it access to, even when users are not currently using the app. This does not give the app any additional permissions.
  flows: []
  scope: offline_access
- description: Allows users to sign-in to the app, and allows the app to read the profile of signed-in users. It also allows the app to read basic company information of signed-in users.
  flows: []
  scope: User.Read
- description: Allows the app to read a basic set of profile properties of other users in your organization on behalf of the signed-in user. This includes display name, first and last name, email address, photo, id and security identifier. Also allows the app to read the full profile of the signed-in user.
  flows: []
  scope: User.ReadBasic.All
- description: Allows the app to read the full set of user properties of all users in the organization and read company properties, on behalf of the signed-in user.
  flows: []
  scope: User.Read.All
- description: Allows the app to read and write the full set of profile properties, reports, and managers of other users in your organization, and read basic company properties, on behalf of the signed-in user.
  flows: []
  scope: User.ReadWrite.All
- description: Allows the app to read data in your organization's directory, such as users, groups and apps.
  flows: []
  scope: Directory.Read.All
- description: Allows the app to read and write data in your organization's directory, such as users, and groups. It does not allow the app to delete users or groups, or reset user passwords.
  flows: []
  scope: Directory.ReadWrite.All
- description: Allows the app to have the same access to information in the directory as the signed-in user.
  flows: []
  scope: Directory.AccessAsUser.All
- description: Allows the app to list groups, and to read their properties and all group memberships on behalf of the signed-in user. Also allows the app to read calendar, conversations, files, and other group content for all groups the signed-in user can access.
  flows: []
  scope: Group.Read.All
- description: Allows the app to create groups and read all group properties and memberships on behalf of the signed-in user. Additionally allows group owners to manage their groups and allows group members to update group content.
  flows: []
  scope: Group.ReadWrite.All
- description: Allows the app to list groups, read basic group properties and read membership of all groups the signed-in user has access to.
  flows: []
  scope: GroupMember.Read.All
- description: Allows the app to list groups, read basic properties, read and update the membership of the groups the signed-in user has access to. Group properties and owners cannot be updated and groups cannot be deleted.
  flows: []
  scope: GroupMember.ReadWrite.All
- description: Allows the app to read applications and service principals on behalf of the signed-in user.
  flows: []
  scope: Application.Read.All
- description: Allows the app to create, read, update and delete applications and service principals on behalf of the signed-in user. Does not allow management of consent grants.
  flows: []
  scope: Application.ReadWrite.All
- description: Allows the app to create other applications, and fully manage those applications (read, update, update application secrets and delete), without a signed-in user. It cannot update any apps that it is not an owner of.
  flows: []
  scope: Application.ReadWrite.OwnedBy
- description: Allows the app to manage permission grants for application permissions to any API (including Microsoft Graph) and application assignments for any app, on behalf of the signed-in user.
  flows: []
  scope: AppRoleAssignment.ReadWrite.All
- description: Allows the app to read the role-based access control (RBAC) settings for your company's directory, on behalf of the signed-in user. This includes reading directory role templates, directory roles and memberships.
  flows: []
  scope: RoleManagement.Read.Directory
- description: Allows the app to read and manage the role-based access control (RBAC) settings for your company's directory, on behalf of the signed-in user. This includes instantiating directory roles and managing directory role membership, and reading directory role templates, directory roles and memberships.
  flows: []
  scope: RoleManagement.ReadWrite.Directory
- description: Allows the app to read your organization's policies on behalf of the signed-in user.
  flows: []
  scope: Policy.Read.All
- description: Allows the app to read and write your organization's conditional access policies on behalf of the signed-in user.
  flows: []
  scope: Policy.ReadWrite.ConditionalAccess
- description: Allows the app to read and query your audit log activities, on behalf of the signed-in user.
  flows: []
  scope: AuditLog.Read.All
- description: Allows the app to read your organization's devices' configuration information on behalf of the signed-in user.
  flows: []
  scope: Device.Read.All
- description: Allows the app to read and write all device properties without a signed in user. Does not allow device creation, device deletion or update of device alternative security identifiers.
  flows: []
  scope: Device.ReadWrite.All
- description: Allows the app to read access packages and related entitlement management resources on behalf of the signed-in user.
  flows: []
  scope: EntitlementManagement.Read.All
- description: Allows the app to request access to and management of access packages and related entitlement management resources on behalf of the signed-in user.
  flows: []
  scope: EntitlementManagement.ReadWrite.All
- description: Allows the app to read access reviews, reviewers, decisions and settings that the signed-in user has access to in the organization.
  flows: []
  scope: AccessReview.Read.All
- description: Allows the app to read, update, delete and perform actions on access reviews, reviewers, decisions and settings that the signed-in user has access to in the organization.
  flows: []
  scope: AccessReview.ReadWrite.All
- description: Allows the app to read authentication methods of all users in your organization that the signed-in user has access to. Authentication methods include things like a user's phone numbers and Authenticator app settings. This does not allow the app to see secret information like passwords, or to sign-in or otherwise use the authentication methods.
  flows: []
  scope: UserAuthenticationMethod.Read.All
- description: Allows the app to read and write authentication methods of all users in your organization that the signed-in user has access to. Authentication methods include things like a user's phone numbers and Authenticator app settings. This does not allow the app to see secret information like passwords, or to sign-in or otherwise use the authentication methods.
  flows: []
  scope: UserAuthenticationMethod.ReadWrite.All
- description: Allows the app to read time-based assignment and just-in-time elevation (including scheduled elevation) of Azure AD groups, on behalf of the signed-in user.
  flows: []
  scope: PrivilegedAccess.Read.AzureADGroup
- description: Allows the app to read the organization and related resources, on behalf of the signed-in user. Related resources include things like subscribed skus and tenant branding information.
  flows: []
  scope: Organization.Read.All
- description: Allows the app to read all domain properties on behalf of the signed-in user.
  flows: []
  scope: Domain.Read.All
- description: Allows the app to read administrative units and administrative unit membership on behalf of the signed-in user.
  flows: []
  scope: AdministrativeUnit.Read.All
- description: Allows the app to read your organization's identity (authentication) providers' properties on behalf of the user.
  flows: []
  scope: IdentityProvider.Read.All
- description: Allows the app to read identity risk event information for all users in your organization on behalf of the signed-in user.
  flows: []
  scope: IdentityRiskEvent.Read.All
- description: Allows the app to read all webhook subscriptions on behalf of the signed-in user.
  flows: []
  scope: Subscription.Read.All
slug: azure-ad-scopes
source_filename: azure-ad-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/graph/permissions-reference (docs) and the first-party machine-readable\n  permission catalogue at https://raw.githubusercontent.com/microsoftgraph/microsoft-graph-devx-content/dev/permissions/permissions-descriptions.json\n  (fetched 200, 2026-09-06) — the same file that powers the consent UI in Graph Explorer. Scheme endpoints\n  corroborated by https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration and by\n  the azureaadv2 securityScheme in every harvested spec in openapi/_original/.\ndocs: https://learn.microsoft.com/en-us/graph/permissions-reference\nprovider: Azure Active Directory (Microsoft Entra ID)\nproviderId: azure-ad\nsupersedes: The 2026-07-11 derived file, which carried 7 scopes read out of a hand-written scaffold spec.\n  Descriptions below are Microsoft's own admin-consent text, quoted verbatim.\nnote: Microsoft Graph publishes TWO disjoint permission\
  \ sets for the same resources — delegated (the app\n  acts as a signed-in user, effective access is the intersection of the scope and the user's own privileges)\n  and application (the app acts as itself, admin consent always required, no user context). The `types`\n  field on each entry says which sets a name appears in. The full published catalogue is 583 delegated\n  and 527 application permissions; the entries below are the Entra ID directory subset that this record\n  covers, not the whole list.\nschemes:\n- name: azureaadv2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    permission_set: delegated\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    permission_set: application\n    note: Request scope https://graph.microsoft.com/.default; individual scopes\
  \ are not requested at token\n      time.\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/devicecode\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    permission_set: delegated\n  sources:\n  - openapi/_original/azure-ad-graph-users-openapi.yml\n  - well-known/azure-ad-openid-configuration.json\noidc_scopes:\n- openid\n- profile\n- email\n- offline_access\noidc_scopes_source: scopes_supported in well-known/azure-ad-openid-configuration.json\nconsent:\n  delegated: User consent for low-privilege scopes; admin consent required for any *.All scope.\n  application: Always admin consent, granted tenant-wide.\n  least_privilege_guidance: https://learn.microsoft.com/en-us/graph/permissions-overview\n  note: The published catalogue flags a least-privilege permission per operation; Graph Explorer surfaces\n    it per query in the Modify permissions tab.\ncatalogue_totals:\n  delegated: 583\n  application: 527\n\
  scopes:\n- scope: openid\n  display_name: Sign users in\n  description: Allows users to sign in to the app with their work or school accounts and allows the app\n    to see basic user profile information.\n  types:\n  - delegated\n  admin_consent_required_delegated: false\n- scope: profile\n  display_name: View users' basic profile\n  description: Allows the app to see your users' basic profile (e.g., name, picture, user name, email\n    address)\n  types:\n  - delegated\n  admin_consent_required_delegated: false\n- scope: email\n  display_name: View users' email address\n  description: Allows the app to read your users' primary email address\n  types:\n  - delegated\n  admin_consent_required_delegated: false\n- scope: offline_access\n  display_name: Maintain access to data you have given it access to\n  description: Allows the app to see and update the data you gave it access to, even when users are not\n    currently using the app. This does not give the app any additional permissions.\n\
  \  types:\n  - delegated\n  admin_consent_required_delegated: false\n- scope: User.Read\n  display_name: Sign in and read user profile\n  description: Allows users to sign-in to the app, and allows the app to read the profile of signed-in\n    users. It also allows the app to read basic company information of signed-in users.\n  types:\n  - delegated\n  admin_consent_required_delegated: false\n- scope: User.ReadBasic.All\n  display_name: Read all users' basic profiles\n  description: Allows the app to read a basic set of profile properties of other users in your organization\n    on behalf of the signed-in user. This includes display name, first and last name, email address, photo,\n    id and security identifier. Also allows the app to read the full profile of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: false\n- scope: User.Read.All\n  display_name: Read all users' full profiles and company properties\n  description: Allows the app\
  \ to read the full set of user properties of all users in the organization\n    and read company properties, on behalf of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: User.ReadWrite.All\n  display_name: Read and write all users' full profiles\n  description: Allows the app to read and write the full set of profile properties, reports, and managers\n    of other users in your organization, and read basic company properties, on behalf of the signed-in\n    user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Directory.Read.All\n  display_name: Read directory data\n  description: Allows the app to read data in your organization's directory, such as users, groups and\n    apps.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Directory.ReadWrite.All\n  display_name: Read and write directory data\n  description: Allows the app to read\
  \ and write data in your organization's directory, such as users,\n    and groups.  It does not allow the app to delete users or groups, or reset user passwords.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Directory.AccessAsUser.All\n  display_name: Access directory as the signed in user\n  description: Allows the app to have the same access to information in the directory as the signed-in\n    user.\n  types:\n  - delegated\n  admin_consent_required_delegated: true\n- scope: Group.Read.All\n  display_name: Read all groups\n  description: 'Allows the app to list groups, and to read their properties and all group memberships\n    on behalf of the signed-in user.  Also allows the app to read calendar, conversations, files, and\n    other group content for all groups the signed-in user can access. '\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Group.ReadWrite.All\n  display_name: Read and write\
  \ all groups\n  description: Allows the app to create groups and read all group properties and memberships on behalf\n    of the signed-in user.  Additionally allows group owners to manage their groups and allows group members\n    to update group content.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: GroupMember.Read.All\n  display_name: Read group memberships\n  description: Allows the app to list groups, read basic group properties and read membership of all groups\n    the signed-in user has access to.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: GroupMember.ReadWrite.All\n  display_name: Read and write group memberships\n  description: Allows the app to list groups, read basic properties, read and update the membership of\n    the groups the signed-in user has access to. Group properties and owners cannot be updated and groups\n    cannot be deleted.\n  types:\n  - delegated\n  - application\n\
  \  admin_consent_required_delegated: true\n- scope: Application.Read.All\n  display_name: Read applications\n  description: Allows the app to read applications and service principals on behalf of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Application.ReadWrite.All\n  display_name: Read and write all applications\n  description: Allows the app to create, read, update and delete applications and service principals on\n    behalf of the signed-in user. Does not allow management of consent grants.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Application.ReadWrite.OwnedBy\n  display_name: Manage apps that this app creates or owns\n  description: Allows the app to create other applications, and fully manage those applications (read,\n    update, update application secrets and delete), without a signed-in user.  It cannot update any apps\n    that it is not an owner of.\n  types:\n\
  \  - application\n- scope: AppRoleAssignment.ReadWrite.All\n  display_name: Manage app permission grants and app role assignments\n  description: Allows the app to manage permission grants for application permissions to any API (including\n    Microsoft Graph) and application assignments for any app, on behalf of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: RoleManagement.Read.Directory\n  display_name: Read directory RBAC settings\n  description: Allows the app to read the role-based access control (RBAC) settings for your company's\n    directory, on behalf of the signed-in user.  This includes reading directory role templates, directory\n    roles and memberships.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: RoleManagement.ReadWrite.Directory\n  display_name: Read and write directory RBAC settings\n  description: Allows the app to read and manage the role-based access\
  \ control (RBAC) settings for your\n    company's directory, on behalf of the signed-in user. This includes instantiating directory roles\n    and managing directory role membership, and reading directory role templates, directory roles and\n    memberships.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Policy.Read.All\n  display_name: Read your organization's policies\n  description: Allows the app to read your organization's policies on behalf of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Policy.ReadWrite.ConditionalAccess\n  display_name: Read and write your organization's conditional access policies\n  description: Allows the app to read and write your organization's conditional access policies on behalf\n    of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: AuditLog.Read.All\n  display_name: Read audit\
  \ log data\n  description: Allows the app to read and query your audit log activities, on behalf of the signed-in\n    user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Device.Read.All\n  display_name: Read all devices\n  description: Allows the app to read your organization's devices' configuration information on behalf\n    of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Device.ReadWrite.All\n  display_name: Read and write devices\n  description: Allows the app to read and write all device properties without a signed in user.  Does\n    not allow device creation, device deletion or update of device alternative security identifiers.\n  types:\n  - application\n- scope: EntitlementManagement.Read.All\n  display_name: Read all entitlement management resources\n  description: Allows the app to read access packages and related entitlement management resources on\n    behalf\
  \ of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: EntitlementManagement.ReadWrite.All\n  display_name: Read and write entitlement management resources\n  description: Allows the app to request access to and management of access packages and related entitlement\n    management resources on behalf of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: AccessReview.Read.All\n  display_name: Read all access reviews that user can access\n  description: Allows the app to read access reviews, reviewers, decisions and settings that the signed-in\n    user has access to in the organization.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: AccessReview.ReadWrite.All\n  display_name: Manage all access reviews that user can access\n  description: Allows the app to read, update, delete and perform actions on access reviews, reviewers,\n\
  \    decisions and settings that the signed-in user has access to in the organization.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: UserAuthenticationMethod.Read.All\n  display_name: Read all users' authentication methods\n  description: Allows the app to read authentication methods of all users in your organization that the\n    signed-in user has access to. Authentication methods include things like a user's phone numbers and\n    Authenticator app settings. This does not allow the app to see secret information like passwords,\n    or to sign-in or otherwise use the authentication methods.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: UserAuthenticationMethod.ReadWrite.All\n  display_name: Read and write all users' authentication methods\n  description: ' Allows the app to read and write authentication methods of all users in your organization\n    that the signed-in user has access to. \
  \                      Authentication methods include things\n    like a user''s phone numbers and Authenticator app settings. This                      does not allow\n    the app to see secret information like passwords, or to sign-in or otherwise use the authentication\n    methods.'\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: PrivilegedAccess.Read.AzureADGroup\n  display_name: Read privileged access to Azure AD groups\n  description: Allows the app to read time-based assignment and just-in-time elevation (including scheduled\n    elevation) of Azure AD groups, on behalf of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Organization.Read.All\n  display_name: Read organization information\n  description: Allows the app to read the organization and related resources, on behalf of the signed-in\n    user. Related resources include things like subscribed skus and tenant branding\
  \ information.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Domain.Read.All\n  display_name: Read domains\n  description: Allows the app to read all domain properties on behalf of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: AdministrativeUnit.Read.All\n  display_name: Read administrative units\n  description: Allows the app to read administrative units and administrative unit membership on behalf\n    of the signed-in user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: IdentityProvider.Read.All\n  display_name: Read identity providers\n  description: Allows the app to read your organization's identity (authentication) providers' properties\n    on behalf of the user.\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: IdentityRiskEvent.Read.All\n  display_name: Read identity risk\
  \ event information\n  description: 'Allows the app to read identity risk event information for all users in your organization\n    on behalf of the signed-in user. '\n  types:\n  - delegated\n  - application\n  admin_consent_required_delegated: true\n- scope: Subscription.Read.All\n  display_name: Read all webhook subscriptions\n  description: Allows the app to read all webhook subscriptions on behalf of the signed-in user.\n  types:\n  - delegated\n  admin_consent_required_delegated: true\nscope_count: 39\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/scopes/azure-ad-scopes.yml
summary_line: 39 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Authentication
- Authorization
- Identity
- OpenID Connect
- Single Sign-On
token_urls:
- https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
---
