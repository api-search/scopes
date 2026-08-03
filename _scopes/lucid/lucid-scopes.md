---
api_specs:
- filename: lucid-rest-api-openapi.yml
  format: yaml
  label: Lucid REST API
  slug: lucid-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-rest-api-openapi.yml
- filename: lucid-data-api-openapi.yml
  format: yaml
  label: Lucid Data API
  slug: lucid-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-data-api-openapi.yml
- filename: lucid-scim-api-openapi.yml
  format: yaml
  label: Lucid SCIM API
  slug: lucid-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-scim-api-openapi.yml
- filename: lucid-chatgpt-plugin-openapi.yaml
  format: yaml
  label: Lucid ChatGPT Plugin API
  slug: lucid-chatgpt-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-chatgpt-plugin-openapi.yaml
authorization_urls:
- https://lucid.app/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lucid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lucid publishes 143 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lucid API on a user''s behalf.


  Tokens are issued from https://api.lucid.co/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lucid
provider_slug: lucid
schemes:
- flows:
  - authorizationUrl: https://lucid.app/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.lucid.co/oauth2/token
  name: OAuth2
  source: openapi/lucid-data-api-openapi.yml
- flows:
  - authorizationUrl: https://lucid.app/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.lucid.co/oauth2/token
  name: OAuth2
  source: openapi/lucid-rest-api-openapi.yml
scope_count: 143
scope_names:
- account.audit.logs
- account.info
- account.legalhold
- account.legalhold.users
- account.legalhold.users:readonly
- account.legalhold:readonly
- account.settings:readonly
- account.user
- account.user.transfercontent
- account.user:readonly
- account.users:admin.readonly
- cloud.credential
- cloud.credential:readonly
- cloud.datasource
- cloud.datasource:readonly
- cloud.model
- data-service.admin
- document.app
- document.app.folder
- document.app.picker
- document.app.picker:readonly
- document.content
- document.content:readonly
- folder
- folder:admin
- folder:admin.readonly
- folder:readonly
- invitation
- invitation.accept
- licenses:admin
- licenses:admin.readonly
- lucid.document.accessRequest
- lucid.document.app
- lucid.document.app.folder
- lucid.document.app.picker
- lucid.document.app.picker.share
- lucid.document.app.picker.share.collaborator
- lucid.document.app.picker.share.collaborator:readonly
- lucid.document.app.picker.share.embed
- lucid.document.app.picker.share.embed:readonly
- lucid.document.app.picker.share.link
- lucid.document.app.picker.share.link:readonly
- lucid.document.app.picker.share:readonly
- lucid.document.app.picker:readonly
- lucid.document.content
- lucid.document.content.share
- lucid.document.content.share.collaborator
- lucid.document.content.share.collaborator:readonly
- lucid.document.content.share.embed
- lucid.document.content.share.embed:readonly
- lucid.document.content.share.link
- lucid.document.content.share.link:readonly
- lucid.document.content.share:readonly
- lucid.document.content:admin
- lucid.document.content:admin.readonly
- lucid.document.content:readonly
- lucid.document.storage:admin.readonly
- lucidchart.document.accessRequest
- lucidchart.document.app
- lucidchart.document.app.folder
- lucidchart.document.app.picker
- lucidchart.document.app.picker.share
- lucidchart.document.app.picker.share.collaborator
- lucidchart.document.app.picker.share.collaborator:readonly
- lucidchart.document.app.picker.share.embed
- lucidchart.document.app.picker.share.embed:readonly
- lucidchart.document.app.picker.share.link
- lucidchart.document.app.picker.share.link:readonly
- lucidchart.document.app.picker.share:readonly
- lucidchart.document.app.picker:readonly
- lucidchart.document.content
- lucidchart.document.content.share
- lucidchart.document.content.share.collaborator
- lucidchart.document.content.share.collaborator:readonly
- lucidchart.document.content.share.embed
- lucidchart.document.content.share.embed:readonly
- lucidchart.document.content.share.link
- lucidchart.document.content.share.link:readonly
- lucidchart.document.content.share:readonly
- lucidchart.document.content:admin
- lucidchart.document.content:admin.readonly
- lucidchart.document.content:readonly
- lucidchart.document.storage:admin.readonly
- lucidscale.document.accessRequest
- lucidscale.document.app
- lucidscale.document.app.folder
- lucidscale.document.app.picker
- lucidscale.document.app.picker.share
- lucidscale.document.app.picker.share.collaborator
- lucidscale.document.app.picker.share.collaborator:readonly
- lucidscale.document.app.picker.share.embed
- lucidscale.document.app.picker.share.embed:readonly
- lucidscale.document.app.picker.share.link
- lucidscale.document.app.picker.share.link:readonly
- lucidscale.document.app.picker.share:readonly
- lucidscale.document.app.picker:readonly
- lucidscale.document.content
- lucidscale.document.content.share
- lucidscale.document.content.share.collaborator
- lucidscale.document.content.share.collaborator:readonly
- lucidscale.document.content.share.embed
- lucidscale.document.content.share.embed:readonly
- lucidscale.document.content.share.link
- lucidscale.document.content.share.link:readonly
- lucidscale.document.content.share:readonly
- lucidscale.document.content:admin
- lucidscale.document.content:admin.readonly
- lucidscale.document.content:readonly
- lucidscale.document.storage:admin.readonly
- lucidspark.document.accessRequest
- lucidspark.document.app
- lucidspark.document.app.folder
- lucidspark.document.app.picker
- lucidspark.document.app.picker.share
- lucidspark.document.app.picker.share.collaborator
- lucidspark.document.app.picker.share.collaborator:readonly
- lucidspark.document.app.picker.share.embed
- lucidspark.document.app.picker.share.embed:readonly
- lucidspark.document.app.picker.share.link
- lucidspark.document.app.picker.share.link:readonly
- lucidspark.document.app.picker.share:readonly
- lucidspark.document.app.picker:readonly
- lucidspark.document.content
- lucidspark.document.content.share
- lucidspark.document.content.share.collaborator
- lucidspark.document.content.share.collaborator:readonly
- lucidspark.document.content.share.embed
- lucidspark.document.content.share.embed:readonly
- lucidspark.document.content.share.link
- lucidspark.document.content.share.link:readonly
- lucidspark.document.content.share:readonly
- lucidspark.document.content:admin
- lucidspark.document.content:admin.readonly
- lucidspark.document.content:readonly
- lucidspark.document.storage:admin.readonly
- offline_access
- repository
- repository:admin
- repository:readonly
- teams
- teams:admin
- teams:readonly
- user.profile
scopes:
- description: View audit logs on your account.
  flows:
  - authorizationCode
  scope: account.audit.logs
- description: View basic information about your account (e.g., account ID and account name) .
  flows:
  - authorizationCode
  scope: account.info
- description: Create, view, and expire legal holds on your account.
  flows:
  - authorizationCode
  scope: account.legalhold
- description: Manage legal hold users on your account.
  flows:
  - authorizationCode
  scope: account.legalhold.users
- description: View legal hold users on your account.
  flows:
  - authorizationCode
  scope: account.legalhold.users:readonly
- description: View legal holds on your account.
  flows:
  - authorizationCode
  scope: account.legalhold:readonly
- description: View settings on your account.
  flows:
  - authorizationCode
  scope: account.settings:readonly
- description: Create, view, edit, and delete users on your account.
  flows:
  - authorizationCode
  scope: account.user
- description: Transfer ownership of a user's resources to another user on your account.
  flows:
  - authorizationCode
  scope: account.user.transfercontent
- description: View users on your account.
  flows:
  - authorizationCode
  scope: account.user:readonly
- description: View all users and their roles on your account.
  flows:
  - authorizationCode
  scope: account.users:admin.readonly
- description: Manage cloud credentials.
  flows:
  - authorizationCode
  scope: cloud.credential
- description: View cloud credentials.
  flows:
  - authorizationCode
  scope: cloud.credential:readonly
- description: Manage cloud data sources.
  flows:
  - authorizationCode
  scope: cloud.datasource
- description: View cloud data sources.
  flows:
  - authorizationCode
  scope: cloud.datasource:readonly
- description: Manage cloud models.
  flows:
  - authorizationCode
  scope: cloud.model
- description: Scope needed for access to the Data APIs.
  flows:
  - authorizationCode
  scope: data-service.admin
- description: View, edit, and manage any Lucidchart document selected for this third-party application. Create, view, edit, and manage any Lucidchart document within its app-specific folder.
  flows:
  - authorizationCode
  scope: document.app
- description: Create, view, edit, and manage any Lucidchart document within its app-specific folder.
  flows:
  - authorizationCode
  scope: document.app.folder
- description: View, edit, and manage any Lucidchart document selected for this third-party application.
  flows:
  - authorizationCode
  scope: document.app.picker
- description: View and download any Lucidchart document selected for this third-party application.
  flows:
  - authorizationCode
  scope: document.app.picker:readonly
- description: Create, view, edit, and delete any Lucidchart document on your account.
  flows:
  - authorizationCode
  scope: document.content
- description: View and download any Lucidchart document on your account.
  flows:
  - authorizationCode
  scope: document.content:readonly
- description: Create, view, edit, share, and delete your folders. Organize your folders and their contents.
  flows:
  - authorizationCode
  scope: folder
- description: Perform admin actions on folders belonging to the account.
  flows:
  - authorizationCode
  scope: folder:admin
- description: View all folders belonging to the account with admin permissions.
  flows:
  - authorizationCode
  scope: folder:admin.readonly
- description: View any of your folders and list their contents.
  flows:
  - authorizationCode
  scope: folder:readonly
- description: Accept document and folder share links.
  flows:
  - authorizationCode
  scope: invitation
- description: Accept document and folder share links.
  flows:
  - authorizationCode
  scope: invitation.accept
- description: Perform admin actions on licenses and subscriptions belonging to the account.
  flows:
  - authorizationCode
  scope: licenses:admin
- description: View licenses and subscriptions belonging to the account with admin permissions.
  flows:
  - authorizationCode
  scope: licenses:admin.readonly
- description: Request access to Lucid documents.
  flows:
  - authorizationCode
  scope: lucid.document.accessRequest
- description: View, edit, create, and manage folders and documents within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app
- description: Create, view, edit, and manage any Lucid document within its app-specific folder.
  flows:
  - authorizationCode
  scope: lucid.document.app.folder
- description: View, edit, and manage any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker
- description: Create, view, edit, and delete document collaborators, embeds, and share links for any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker.share
- description: Create, view, edit, and delete document collaborators for any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker.share.collaborator
- description: View document collaborators for any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker.share.collaborator:readonly
- description: Create, view, edit, and delete document embeds for any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker.share.embed
- description: View document embeds for any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker.share.embed:readonly
- description: Create, view, edit, and delete share links for any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker.share.link
- description: View share links for any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker.share.link:readonly
- description: View document collaborators, embeds, and share links for any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker.share:readonly
- description: View and download any Lucid document selected within an app.
  flows:
  - authorizationCode
  scope: lucid.document.app.picker:readonly
- description: Create, view, edit, and delete any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content
- description: Create, view, edit, and delete document collaborators, embeds, and share links for any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content.share
- description: Create, view, edit, and delete document collaborators for any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content.share.collaborator
- description: View document collaborators for any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content.share.collaborator:readonly
- description: Create, view, edit, and delete document embeds for any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content.share.embed
- description: View document embeds for any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content.share.embed:readonly
- description: Create, view, edit, and delete share links for any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content.share.link
- description: View share links for any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content.share.link:readonly
- description: View document collaborators, embeds, and share links for any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content.share:readonly
- description: Perform admin actions on Lucid documents belonging to the account.
  flows:
  - authorizationCode
  scope: lucid.document.content:admin
- description: View all Lucid documents belonging to the account with admin permissions.
  flows:
  - authorizationCode
  scope: lucid.document.content:admin.readonly
- description: View and download any Lucid document accessible by the user.
  flows:
  - authorizationCode
  scope: lucid.document.content:readonly
- description: Perform admin actions backing up Lucid documents belonging to the account.
  flows:
  - authorizationCode
  scope: lucid.document.storage:admin.readonly
- description: Request access to Lucidchart documents.
  flows:
  - authorizationCode
  scope: lucidchart.document.accessRequest
- description: View, edit, and manage any Lucidchart document selected for this third-party application. Create, view, edit, and manage any Lucidchart document within its app-specific folder.
  flows:
  - authorizationCode
  scope: lucidchart.document.app
- description: Create, view, edit, and manage any Lucidchart document within its app-specific folder.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.folder
- description: View, edit, and manage any Lucidchart document selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker
- description: Create, view, edit, and delete document collaborators, embeds, and share links for any Lucidchart document selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker.share
- description: Create, view, edit, and delete collaborators and invitations of any Lucidchart document on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker.share.collaborator
- description: View collaborators and invitations of any Lucidchart document on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker.share.collaborator:readonly
- description: Create, view, edit, and delete embeds of any Lucidchart document on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker.share.embed
- description: View embeds of any Lucidchart document on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker.share.embed:readonly
- description: Create, view, edit, and delete the third party application's share links of any Lucidchart document on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker.share.link
- description: View the third party application's share links of any Lucidchart document on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker.share.link:readonly
- description: View document collaborators, embeds, and share links for any Lucidchart document selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker.share:readonly
- description: View and download any Lucidchart document selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidchart.document.app.picker:readonly
- description: Create, view, edit, and delete any Lucidchart document on your account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content
- description: Create, view, edit, and delete document collaborators, embeds, and share links for any of your Lucidchart documents.
  flows:
  - authorizationCode
  scope: lucidchart.document.content.share
- description: Create, view, edit, and delete collaborators and invitations for any of your Lucidchart documents on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content.share.collaborator
- description: View collaborators and invitations for any of your Lucidchart documents on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content.share.collaborator:readonly
- description: Create, view, edit, and delete embeds for any of your Lucidchart documents on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content.share.embed
- description: View embeds for any of your Lucidchart documents on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content.share.embed:readonly
- description: Create, view, edit, and delete the third party application's share links for any of your Lucidchart documents on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content.share.link
- description: View the third party application's share links for any of your Lucidchart documents on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content.share.link:readonly
- description: View document collaborators, embeds, and share links for any of your Lucidchart documents.
  flows:
  - authorizationCode
  scope: lucidchart.document.content.share:readonly
- description: Perform admin actions on Lucidchart documents belonging to the account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content:admin
- description: View all Lucidchart documents belonging to the account with admin permissions.
  flows:
  - authorizationCode
  scope: lucidchart.document.content:admin.readonly
- description: View and download any Lucidchart document on your account.
  flows:
  - authorizationCode
  scope: lucidchart.document.content:readonly
- description: Perform admin actions backing up Lucidchart documents belonging to the account.
  flows:
  - authorizationCode
  scope: lucidchart.document.storage:admin.readonly
- description: Request access to Lucidscale models.
  flows:
  - authorizationCode
  scope: lucidscale.document.accessRequest
- description: View, edit, and manage any Lucidscale model selected for this third-party application. Create, view, edit, and manage any Lucidscale model within its app-specific folder.
  flows:
  - authorizationCode
  scope: lucidscale.document.app
- description: Create, view, edit, and manage any Lucidscale model within its app-specific folder.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.folder
- description: View, edit, and manage any Lucidscale model selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker
- description: Create, view, edit, and delete document collaborators, embeds, and share links for any Lucidscale model selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker.share
- description: Create, view, edit, and delete collaborators and invitations of any Lucidscale model on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker.share.collaborator
- description: View collaborators and invitations of any Lucidscale model on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker.share.collaborator:readonly
- description: Create, view, edit, and delete embeds of any Lucidscale model on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker.share.embed
- description: View embeds of any Lucidscale model on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker.share.embed:readonly
- description: Create, view, edit, and delete the third party application's share links of any Lucidscale model on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker.share.link
- description: View the third party application's share links of any Lucidscale model on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker.share.link:readonly
- description: View document collaborators, embeds, and share links for any Lucidscale model selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker.share:readonly
- description: View and download any Lucidscale model selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidscale.document.app.picker:readonly
- description: Create, view, edit, and delete any Lucidscale model on your account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content
- description: Create, view, edit, and delete document collaborators, embeds, and share links for any of your Lucidscale models.
  flows:
  - authorizationCode
  scope: lucidscale.document.content.share
- description: Create, view, edit, and delete collaborators and invitations for any of your Lucidscale models on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content.share.collaborator
- description: View collaborators and invitations for any of your Lucidscale models on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content.share.collaborator:readonly
- description: Create, view, edit, and delete embeds for any of your Lucidscale models on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content.share.embed
- description: View embeds for any of your Lucidscale models on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content.share.embed:readonly
- description: Create, view, edit, and delete the third party application's share links for any of your Lucidscale models on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content.share.link
- description: View the third party application's share links for any of your Lucidscale models on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content.share.link:readonly
- description: View document collaborators, embeds, and share links for any of your Lucidscale models.
  flows:
  - authorizationCode
  scope: lucidscale.document.content.share:readonly
- description: Perform admin actions on Lucidscale models belonging to the account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content:admin
- description: View all Lucidscale models belonging to the account with admin permissions.
  flows:
  - authorizationCode
  scope: lucidscale.document.content:admin.readonly
- description: View and download any Lucidscale model on your account.
  flows:
  - authorizationCode
  scope: lucidscale.document.content:readonly
- description: Perform admin actions backing up Lucidscale models belonging to the account.
  flows:
  - authorizationCode
  scope: lucidscale.document.storage:admin.readonly
- description: Request access to Lucidspark boards.
  flows:
  - authorizationCode
  scope: lucidspark.document.accessRequest
- description: View, edit, and manage any Lucidspark board selected for this third-party application. Create, view, edit, and manage any Lucidspark board within its app-specific folder.
  flows:
  - authorizationCode
  scope: lucidspark.document.app
- description: Create, view, edit, and manage any Lucidspark board within its app-specific folder.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.folder
- description: View, edit, and manage any Lucidspark board selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker
- description: Create, view, edit, and delete document collaborators, embeds, and share links for any Lucidspark board selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker.share
- description: Create, view, edit, and delete collaborators and invitations of any Lucidspark board on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker.share.collaborator
- description: View collaborators and invitations of any Lucidspark board on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker.share.collaborator:readonly
- description: Create, view, edit, and delete embeds of any Lucidspark board on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker.share.embed
- description: View embeds of any Lucidspark board on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker.share.embed:readonly
- description: Create, view, edit, and delete the third party application's share links of any Lucidspark board on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker.share.link
- description: View the third party application's share links of any Lucidspark board on your team or enterprise account selected for the third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker.share.link:readonly
- description: View document collaborators, embeds, and share links for any Lucidspark board selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker.share:readonly
- description: View and download any Lucidspark board selected for this third-party application.
  flows:
  - authorizationCode
  scope: lucidspark.document.app.picker:readonly
- description: Create, view, edit, and delete any Lucidspark board on your account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content
- description: Create, view, edit, and delete document collaborators, embeds, and share links for any of your Lucidspark boards.
  flows:
  - authorizationCode
  scope: lucidspark.document.content.share
- description: Create, view, edit, and delete collaborators and invitations for any of your Lucidspark boards on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content.share.collaborator
- description: View collaborators and invitations for any of your Lucidspark boards on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content.share.collaborator:readonly
- description: Create, view, edit, and delete embeds for any of your Lucidspark boards on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content.share.embed
- description: View embeds for any of your Lucidspark boards on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content.share.embed:readonly
- description: Create, view, edit, and delete the third party application's share links for any of your Lucidspark boards on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content.share.link
- description: View the third party application's share links for any of your Lucidspark boards on your team or enterprise account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content.share.link:readonly
- description: View document collaborators, embeds, and share links for any of your Lucidspark boards.
  flows:
  - authorizationCode
  scope: lucidspark.document.content.share:readonly
- description: Perform admin actions on Lucidspark boards belonging to the account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content:admin
- description: View all Lucidspark boards belonging to the account with admin permissions.
  flows:
  - authorizationCode
  scope: lucidspark.document.content:admin.readonly
- description: View and download any Lucidspark board on your account.
  flows:
  - authorizationCode
  scope: lucidspark.document.content:readonly
- description: Perform admin actions backing up Lucidspark boards belonging to the account.
  flows:
  - authorizationCode
  scope: lucidspark.document.storage:admin.readonly
- description: Continue to perform authorized actions when you're not logged in (required to refresh tokens).
  flows:
  - authorizationCode
  scope: offline_access
- description: Manage repositories.
  flows:
  - authorizationCode
  scope: repository
- description: Perform admin actions on repositories.
  flows:
  - authorizationCode
  scope: repository:admin
- description: View repositories.
  flows:
  - authorizationCode
  scope: repository:readonly
- description: Create, view, and edit, archive, and restore any teams on your account. Control which users belong to teams.
  flows:
  - authorizationCode
  scope: teams
- description: Manage teams on your account.
  flows:
  - authorizationCode
  scope: teams:admin
- description: View any teams on your account and list which users belong to them.
  flows:
  - authorizationCode
  scope: teams:readonly
- description: Allow applications to view basic information about you (e.g., full name, username, and email).
  flows:
  - authorizationCode
  scope: user.profile
slug: lucid-scopes
source_filename: lucid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/lucid-data-api-openapi.yml, openapi/lucid-rest-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/lucid-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lucid.app/oauth2/authorize\n    tokenUrl: https://api.lucid.co/oauth2/token\n- name: OAuth2\n  source: openapi/lucid-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lucid.app/oauth2/authorize\n    tokenUrl: https://api.lucid.co/oauth2/token\nscopes:\n- scope: account.audit.logs\n  description: View audit logs on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.info\n  description: View basic information about your account (e.g., account ID and account name)\n    .\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.legalhold\n  description: Create, view, and\
  \ expire legal holds on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.legalhold.users\n  description: Manage legal hold users on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.legalhold.users:readonly\n  description: View legal hold users on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.legalhold:readonly\n  description: View legal holds on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.settings:readonly\n  description: View settings on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.user\n  description: Create, view, edit, and delete users on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n\
  - scope: account.user.transfercontent\n  description: Transfer ownership of a user's resources to another user on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.user:readonly\n  description: View users on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: account.users:admin.readonly\n  description: View all users and their roles on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: cloud.credential\n  description: Manage cloud credentials.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: cloud.credential:readonly\n  description: View cloud credentials.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: cloud.datasource\n  description: Manage cloud data sources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n\
  - scope: cloud.datasource:readonly\n  description: View cloud data sources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: cloud.model\n  description: Manage cloud models.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: data-service.admin\n  description: Scope needed for access to the Data APIs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-data-api-openapi.yml\n- scope: document.app\n  description: View, edit, and manage any Lucidchart document selected for this third-party\n    application. Create, view, edit, and manage any Lucidchart document within its app-specific\n    folder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: document.app.folder\n  description: Create, view, edit, and manage any Lucidchart document within its app-specific\n    folder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n\
  - scope: document.app.picker\n  description: View, edit, and manage any Lucidchart document selected for this third-party\n    application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: document.app.picker:readonly\n  description: View and download any Lucidchart document selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: document.content\n  description: Create, view, edit, and delete any Lucidchart document on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: document.content:readonly\n  description: View and download any Lucidchart document on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: folder\n  description: Create, view, edit, share, and delete your folders. Organize your folders and\n    their contents.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: folder:admin\n  description: Perform admin actions on folders belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: folder:admin.readonly\n  description: View all folders belonging to the account with admin permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: folder:readonly\n  description: View any of your folders and list their contents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: invitation\n  description: Accept document and folder share links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: invitation.accept\n  description: Accept document and folder share links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: licenses:admin\n  description: Perform admin actions\
  \ on licenses and subscriptions belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: licenses:admin.readonly\n  description: View licenses and subscriptions belonging to the account with admin permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.accessRequest\n  description: Request access to Lucid documents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app\n  description: View, edit, create, and manage folders and documents within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.folder\n  description: Create, view, edit, and manage any Lucid document within its app-specific folder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker\n  description:\
  \ View, edit, and manage any Lucid document selected within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker.share\n  description: Create, view, edit, and delete document collaborators, embeds, and share links\n    for any Lucid document selected within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker.share.collaborator\n  description: Create, view, edit, and delete document collaborators for any Lucid document\n    selected within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker.share.collaborator:readonly\n  description: View document collaborators for any Lucid document selected within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker.share.embed\n  description: Create,\
  \ view, edit, and delete document embeds for any Lucid document selected\n    within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker.share.embed:readonly\n  description: View document embeds for any Lucid document selected within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker.share.link\n  description: Create, view, edit, and delete share links for any Lucid document selected within\n    an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker.share.link:readonly\n  description: View share links for any Lucid document selected within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker.share:readonly\n  description: View document collaborators, embeds, and share links for any Lucid\
  \ document selected\n    within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.app.picker:readonly\n  description: View and download any Lucid document selected within an app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content\n  description: Create, view, edit, and delete any Lucid document accessible by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content.share\n  description: Create, view, edit, and delete document collaborators, embeds, and share links\n    for any Lucid document accessible by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content.share.collaborator\n  description: Create, view, edit, and delete document collaborators for any Lucid document\n    accessible by the user.\n  flows:\n  -\
  \ authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content.share.collaborator:readonly\n  description: View document collaborators for any Lucid document accessible by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content.share.embed\n  description: Create, view, edit, and delete document embeds for any Lucid document accessible\n    by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content.share.embed:readonly\n  description: View document embeds for any Lucid document accessible by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content.share.link\n  description: Create, view, edit, and delete share links for any Lucid document accessible\n    by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n\
  - scope: lucid.document.content.share.link:readonly\n  description: View share links for any Lucid document accessible by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content.share:readonly\n  description: View document collaborators, embeds, and share links for any Lucid document accessible\n    by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content:admin\n  description: Perform admin actions on Lucid documents belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content:admin.readonly\n  description: View all Lucid documents belonging to the account with admin permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.content:readonly\n  description: View and download any Lucid document accessible\
  \ by the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucid.document.storage:admin.readonly\n  description: Perform admin actions backing up Lucid documents belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.accessRequest\n  description: Request access to Lucidchart documents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app\n  description: View, edit, and manage any Lucidchart document selected for this third-party\n    application. Create, view, edit, and manage any Lucidchart document within its app-specific\n    folder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.folder\n  description: Create, view, edit, and manage any Lucidchart document within its app-specific\n    folder.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker\n  description: View, edit, and manage any Lucidchart document selected for this third-party\n    application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker.share\n  description: Create, view, edit, and delete document collaborators, embeds, and share links\n    for any Lucidchart document selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker.share.collaborator\n  description: Create, view, edit, and delete collaborators and invitations of any Lucidchart\n    document on your team or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker.share.collaborator:readonly\n  description:\
  \ View collaborators and invitations of any Lucidchart document on your team or\n    enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker.share.embed\n  description: Create, view, edit, and delete embeds of any Lucidchart document on your team\n    or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker.share.embed:readonly\n  description: View embeds of any Lucidchart document on your team or enterprise account selected\n    for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker.share.link\n  description: Create, view, edit, and delete the third party application's share links of any\n    Lucidchart document on your team\
  \ or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker.share.link:readonly\n  description: View the third party application's share links of any Lucidchart document on\n    your team or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker.share:readonly\n  description: View document collaborators, embeds, and share links for any Lucidchart document\n    selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.app.picker:readonly\n  description: View and download any Lucidchart document selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope:\
  \ lucidchart.document.content\n  description: Create, view, edit, and delete any Lucidchart document on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content.share\n  description: Create, view, edit, and delete document collaborators, embeds, and share links\n    for any of your Lucidchart documents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content.share.collaborator\n  description: Create, view, edit, and delete collaborators and invitations for any of your\n    Lucidchart documents on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content.share.collaborator:readonly\n  description: View collaborators and invitations for any of your Lucidchart documents on your\n    team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content.share.embed\n  description: Create, view, edit, and delete embeds for any of your Lucidchart documents on\n    your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content.share.embed:readonly\n  description: View embeds for any of your Lucidchart documents on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content.share.link\n  description: Create, view, edit, and delete the third party application's share links for\n    any of your Lucidchart documents on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content.share.link:readonly\n  description: View the third party application's share links for any of your Lucidchart\
  \ documents\n    on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content.share:readonly\n  description: View document collaborators, embeds, and share links for any of your Lucidchart\n    documents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content:admin\n  description: Perform admin actions on Lucidchart documents belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content:admin.readonly\n  description: View all Lucidchart documents belonging to the account with admin permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.content:readonly\n  description: View and download any Lucidchart document on your account.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidchart.document.storage:admin.readonly\n  description: Perform admin actions backing up Lucidchart documents belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.accessRequest\n  description: Request access to Lucidscale models.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app\n  description: View, edit, and manage any Lucidscale model selected for this third-party application.\n    Create, view, edit, and manage any Lucidscale model within its app-specific folder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.folder\n  description: Create, view, edit, and manage any Lucidscale model within its app-specific folder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope:\
  \ lucidscale.document.app.picker\n  description: View, edit, and manage any Lucidscale model selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker.share\n  description: Create, view, edit, and delete document collaborators, embeds, and share links\n    for any Lucidscale model selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker.share.collaborator\n  description: Create, view, edit, and delete collaborators and invitations of any Lucidscale\n    model on your team or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker.share.collaborator:readonly\n  description: View collaborators and invitations of any Lucidscale model on your\
  \ team or enterprise\n    account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker.share.embed\n  description: Create, view, edit, and delete embeds of any Lucidscale model on your team or\n    enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker.share.embed:readonly\n  description: View embeds of any Lucidscale model on your team or enterprise account selected\n    for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker.share.link\n  description: Create, view, edit, and delete the third party application's share links of any\n    Lucidscale model on your team or enterprise account selected for the third-party application.\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker.share.link:readonly\n  description: View the third party application's share links of any Lucidscale model on your\n    team or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker.share:readonly\n  description: View document collaborators, embeds, and share links for any Lucidscale model\n    selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.app.picker:readonly\n  description: View and download any Lucidscale model selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content\n  description: Create, view, edit, and delete any Lucidscale\
  \ model on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content.share\n  description: Create, view, edit, and delete document collaborators, embeds, and share links\n    for any of your Lucidscale models.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content.share.collaborator\n  description: Create, view, edit, and delete collaborators and invitations for any of your\n    Lucidscale models on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content.share.collaborator:readonly\n  description: View collaborators and invitations for any of your Lucidscale models on your\n    team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content.share.embed\n  description:\
  \ Create, view, edit, and delete embeds for any of your Lucidscale models on your\n    team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content.share.embed:readonly\n  description: View embeds for any of your Lucidscale models on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content.share.link\n  description: Create, view, edit, and delete the third party application's share links for\n    any of your Lucidscale models on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content.share.link:readonly\n  description: View the third party application's share links for any of your Lucidscale models\n    on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n\
  - scope: lucidscale.document.content.share:readonly\n  description: View document collaborators, embeds, and share links for any of your Lucidscale\n    models.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content:admin\n  description: Perform admin actions on Lucidscale models belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content:admin.readonly\n  description: View all Lucidscale models belonging to the account with admin permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.content:readonly\n  description: View and download any Lucidscale model on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidscale.document.storage:admin.readonly\n  description: Perform admin actions backing up Lucidscale\
  \ models belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.accessRequest\n  description: Request access to Lucidspark boards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app\n  description: View, edit, and manage any Lucidspark board selected for this third-party application.\n    Create, view, edit, and manage any Lucidspark board within its app-specific folder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.folder\n  description: Create, view, edit, and manage any Lucidspark board within its app-specific folder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker\n  description: View, edit, and manage any Lucidspark board selected for this third-party application.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker.share\n  description: Create, view, edit, and delete document collaborators, embeds, and share links\n    for any Lucidspark board selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker.share.collaborator\n  description: Create, view, edit, and delete collaborators and invitations of any Lucidspark\n    board on your team or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker.share.collaborator:readonly\n  description: View collaborators and invitations of any Lucidspark board on your team or enterprise\n    account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope:\
  \ lucidspark.document.app.picker.share.embed\n  description: Create, view, edit, and delete embeds of any Lucidspark board on your team or\n    enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker.share.embed:readonly\n  description: View embeds of any Lucidspark board on your team or enterprise account selected\n    for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker.share.link\n  description: Create, view, edit, and delete the third party application's share links of any\n    Lucidspark board on your team or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker.share.link:readonly\n  description: View the third party\
  \ application's share links of any Lucidspark board on your\n    team or enterprise account selected for the third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker.share:readonly\n  description: View document collaborators, embeds, and share links for any Lucidspark board\n    selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.app.picker:readonly\n  description: View and download any Lucidspark board selected for this third-party application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content\n  description: Create, view, edit, and delete any Lucidspark board on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content.share\n  description:\
  \ Create, view, edit, and delete document collaborators, embeds, and share links\n    for any of your Lucidspark boards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content.share.collaborator\n  description: Create, view, edit, and delete collaborators and invitations for any of your\n    Lucidspark boards on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content.share.collaborator:readonly\n  description: View collaborators and invitations for any of your Lucidspark boards on your\n    team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content.share.embed\n  description: Create, view, edit, and delete embeds for any of your Lucidspark boards on your\n    team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content.share.embed:readonly\n  description: View embeds for any of your Lucidspark boards on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content.share.link\n  description: Create, view, edit, and delete the third party application's share links for\n    any of your Lucidspark boards on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content.share.link:readonly\n  description: View the third party application's share links for any of your Lucidspark boards\n    on your team or enterprise account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content.share:readonly\n  description: View document collaborators, embeds, and share links for any of your Lucidspark\n\
  \    boards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content:admin\n  description: Perform admin actions on Lucidspark boards belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content:admin.readonly\n  description: View all Lucidspark boards belonging to the account with admin permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.content:readonly\n  description: View and download any Lucidspark board on your account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: lucidspark.document.storage:admin.readonly\n  description: Perform admin actions backing up Lucidspark boards belonging to the account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: offline_access\n\
  \  description: Continue to perform authorized actions when you're not logged in (required to\n    refresh tokens).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: repository\n  description: Manage repositories.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scope: repository:admin\n  description: Perform admin actions on repositories.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n- scop\n\n# --- truncated at 32 KB (32 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/scopes/lucid-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/scopes/lucid-scopes.yml
summary_line: 143 scopes · authorizationCode
tags:
- Visual Collaboration
- Diagramming
- Whiteboarding
- Productivity
- SaaS
- Cloud Visualization
- SCIM
- Identity
- Data
- MCP
token_urls:
- https://api.lucid.co/oauth2/token
---
