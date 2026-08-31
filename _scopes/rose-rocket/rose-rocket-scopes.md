---
api_specs:
- filename: rose-rocket-boards-api-openapi.yml
  format: yaml
  label: Rose Rocket Boards API
  slug: rose-rocket-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-boards-api-openapi.yml
- filename: rose-rocket-events-api-openapi.yml
  format: yaml
  label: Rose Rocket Events API
  slug: rose-rocket-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-events-api-openapi.yml
- filename: rose-rocket-object-records-api-openapi.yml
  format: yaml
  label: Rose Rocket Object Records API
  slug: rose-rocket-object-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-object-records-api-openapi.yml
- filename: rose-rocket-user-groups-api-openapi.yml
  format: yaml
  label: Rose Rocket User Groups API
  slug: rose-rocket-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/openapi/rose-rocket-user-groups-api-openapi.yml
authorization_urls: []
description: 'Rose Rocket''s OAuth 2.0 layer carries NO API authorization scopes. The scopes the Authentication Guide tells you to request — `offline_access email profile` — are the standard OIDC identity scopes of the Auth0 authorization server at a.roserocket.com; none of them names a Rose Rocket resource or a permission on one. Authorization is enforced entirely server-side by the ROLE the token''s user or service account holds inside the organization, against a per-object, per-field permission matrix administered in the product. This is a real and reasonably granular authorization model, but it is invisible to a client: an agent holding a token cannot read from the token, or from any documented scope list, what it is allowed to do. It finds out by receiving a 403.'
docs: https://roserocket.readme.io/docs/roles-and-permissions
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Rose Rocket Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rose Rocket uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rose Rocket
provider_slug: rose-rocket
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rose-rocket-scopes
source_filename: rose-rocket-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://roserocket.readme.io/docs/rose-rocket-api-oauth-20-authentication-guide,\n  https://roserocket.readme.io/docs/roles-and-permissions, the\n  components.responses.GroupForbiddenResponse description inside\n  openapi/rose-rocket-platform-model-api.json, and the live discovery document at\n  https://a.roserocket.com/.well-known/openid-configuration (HTTP 200, probed\n  2026-08-26).\ndocs: https://roserocket.readme.io/docs/roles-and-permissions\ndescription: >-\n  Rose Rocket's OAuth 2.0 layer carries NO API authorization scopes. The scopes the\n  Authentication Guide tells you to request — `offline_access email profile` — are\n  the standard OIDC identity scopes of the Auth0 authorization server at\n  a.roserocket.com; none of them names a Rose Rocket resource or a permission on\n  one. Authorization is enforced entirely server-side by the ROLE the token's user\n  or service account holds inside the organization,\
  \ against a per-object,\n  per-field permission matrix administered in the product. This is a real and\n  reasonably granular authorization model, but it is invisible to a client: an\n  agent holding a token cannot read from the token, or from any documented scope\n  list, what it is allowed to do. It finds out by receiving a 403.\nmodel: role-based\nmodel_note: >-\n  Permissions are set per ROLE per objectKey, in three sections — Board (which\n  boards the role sees), Record (isCreateAllowed / isDeleteAllowed) and Data (full,\n  read-only, or per-field custom). They are administered at\n  Settings > Users, Roles, Groups > Roles, and can be written through\n  POST {base}/permissions/roles/{role}/objectKey/{object} — an endpoint documented\n  in the Roles and Permissions guide that is NOT present in the published OpenAPI.\nauthorization_server: https://a.roserocket.com/\naudience: https://roserocket.com\noauth_scopes_requested:\n  - name: offline_access\n    purpose: Issues a refresh token.\
  \ Required for any long-lived integration.\n    kind: oidc\n  - name: email\n    purpose: Adds the email claim to the ID token. Identity only; grants no API access.\n    kind: oidc\n  - name: profile\n    purpose: Adds profile claims to the ID token. Identity only; grants no API access.\n    kind: oidc\noauth_scopes_supported_by_authorization_server:\n  source: https://a.roserocket.com/.well-known/openid-configuration\n  note: >-\n    Advertised by the Auth0 tenant, not by Rose Rocket. Every entry is an OIDC\n    identity scope or claim; none is a Rose Rocket resource permission.\n  values: [openid, profile, offline_access, name, given_name, family_name, nickname,\n    email, email_verified, picture, created_at, identities, phone, address]\nresource_permissions_note: >-\n  The one named permission the published contract exposes. It appears only in the\n  403 response description for the user-group operations, and it uses a\n  viewer/editor level rather than an OAuth scope string.\nresource_permissions:\n\
  \  - name: userGroupResource\n    levels:\n      viewer: List, fetch, and view membership of user groups.\n      editor: Update, delete, and modify membership of user groups.\n    applies_to:\n      - GET /userGroups\n      - POST /userGroups\n      - GET /userGroups/{groupId}/members\n      - POST /userGroups/{groupId}/members\n      - POST /userGroups/search\n    evidence: components.responses.GroupForbiddenResponse.description\nbuilt_in_roles_source: https://roserocket.readme.io/docs/roles-and-permissions\nbuilt_in_roles:\n  - {name: Admin, description: Full access for account owners and system administrators.}\n  - {name: Manager, description: 'Almost full access, restricted from changing organizational or subscription settings. Service accounts default to this role.'}\n  - {name: Operations, description: Limited financial data access.}\n  - {name: Sales, description: Limited financial data access.}\n  - {name: Driver, description: Specific for company driver or owner operator.}\n\
  \  - {name: Customer (Guest), description: Limited access for your customers.}\n  - {name: Partner (Guest), description: Limited access to tracking and providing updates.}\n  - {name: Guest, description: Provides guests with limited access.}\n  - {name: External, description: For public viewing of shared information.}\n  - {name: Custom, description: Organizations can define additional roles; every built-in role is editable by an Admin.}\nscope_count: 0\nscope_count_note: >-\n  Zero API authorization scopes are published. Counted deliberately: the three OIDC\n  scopes above are identity scopes and are recorded separately so they are not\n  mistaken for resource permissions.\ngaps:\n  - The OpenAPI declares no components.securitySchemes at all, so no scope list is machine-readable.\n  - No token introspection surface is documented, so a client cannot enumerate its own effective permissions.\n  - The permissions write endpoint (POST /permissions/roles/{role}/objectKey/{object}) is documented\
  \ in prose but absent from the contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rose-rocket/refs/heads/main/scopes/rose-rocket-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Transportation
- Logistics
- freight
- trucking
- transportation-management-system
- Supply Chain
- dispatch
- Webhook
- Authentication
- canada
token_urls: []
---
