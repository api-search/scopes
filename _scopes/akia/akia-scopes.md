---
authorization_urls:
- https://sys.akia.com/oauth/authorize
- https://sys.akia.ai/oauth/authorize
description: ''
docs: https://api.akia.com/docs/scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Akia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Akia publishes 16 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Akia API on a user''s behalf.


  Tokens are issued from https://api.akia.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Akia
provider_slug: akia
schemes:
- flows:
  - authorizationUrl: https://sys.akia.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.akia.com/oauth/token
    tokenUrl: https://api.akia.com/oauth/token
  - authorizationUrl: https://sys.akia.ai/oauth/authorize
    flow: authorizationCode
    note: The RFC 8414 authorization-server metadata advertises sys.akia.ai as the issuer for the MCP resource; the developer docs describe sys.akia.com for the REST API dialog. Both are recorded as observed.
    source: well-known/akia-oauth-authorization-server.json
    tokenUrl: https://sys.akia.ai/oauth/token
  name: OAuth2
  source: https://api.akia.com/docs/authentication
  type: oauth2
scope_count: 16
scope_names:
- audiences:write
- customers:read
- customers:write
- messages:read
- messages:write
- mini_apps:partner_products
- mini_apps:read
- mini_apps:write
- offices:read
- offices:write
- properties:read
- properties:write
- reports:read
- tasks:read
- users:read
- users:write
scopes:
- description: Developer will be create and manage audiences on user's account.
  flows: []
  scope: audiences:write
- description: Developer will be able to see information about user's customers.
  flows: []
  scope: customers:read
- description: Developer will be able to see create and modify user's customers.
  flows: []
  scope: customers:write
- description: Developer will be able to see messages sent and received to user's customers.
  flows: []
  scope: messages:read
- description: Developer will be able to send messages to user's customers.
  flows: []
  scope: messages:write
- description: Developer will be able to provide products guests can purchase through mini apps.
  flows: []
  scope: mini_apps:partner_products
- description: Developer will be able to read data and resources from user's mini apps.
  flows: []
  scope: mini_apps:read
- description: Developer will be able to create and update user's mini apps.
  flows: []
  scope: mini_apps:write
- description: Developer will be able to see information about user's office.
  flows: []
  scope: offices:read
- description: Developer will be able to modify and delete information about user's office.
  flows: []
  scope: offices:write
- description: Developer will be able to see information about user's property.
  flows: []
  scope: properties:read
- description: Developer will be able to modify and delete information about user's property.
  flows: []
  scope: properties:write
- description: Developer will be able to read data and metadata of reports.
  flows: []
  scope: reports:read
- description: Developer will be able to read tasks and task queues on user's account.
  flows: []
  scope: tasks:read
- description: Developer will be able to see staff and departments of user's property.
  flows: []
  scope: users:read
- description: Developer will be able to create, modify, and delete staff and departments.
  flows: []
  scope: users:write
slug: akia-scopes
source_filename: akia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://api.akia.com/docs/scopes\ndocs: https://api.akia.com/docs/scopes\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://api.akia.com/docs/authentication\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sys.akia.com/oauth/authorize\n    tokenUrl: https://api.akia.com/oauth/token\n    refreshUrl: https://api.akia.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://sys.akia.ai/oauth/authorize\n    tokenUrl: https://sys.akia.ai/oauth/token\n    source: well-known/akia-oauth-authorization-server.json\n    note: 'The RFC 8414 authorization-server metadata advertises sys.akia.ai as the\n      issuer for the MCP resource; the developer docs describe sys.akia.com for the\n      REST API dialog. Both are recorded as observed.'\nscope_delimiter: ','\nscopes:\n- scope: audiences:write\n  label: Audiences\n  description: Developer will be create and manage audiences on user's account.\n\
  - scope: customers:read\n  label: Customers (Read)\n  description: Developer will be able to see information about user's customers.\n- scope: customers:write\n  label: Customers\n  description: Developer will be able to see create and modify user's customers.\n- scope: messages:read\n  label: Messages (Read)\n  description: Developer will be able to see messages sent and received to user's\n    customers.\n- scope: messages:write\n  label: Messages\n  description: Developer will be able to send messages to user's customers.\n- scope: mini_apps:partner_products\n  label: Partner Products\n  description: Developer will be able to provide products guests can purchase through\n    mini apps.\n- scope: mini_apps:read\n  label: Apps (Read)\n  description: Developer will be able to read data and resources from user's mini\n    apps.\n- scope: mini_apps:write\n  label: Apps\n  description: Developer will be able to create and update user's mini apps.\n- scope: offices:read\n  label: Offices (Read)\n\
  \  description: Developer will be able to see information about user's office.\n- scope: offices:write\n  label: Offices\n  description: Developer will be able to modify and delete information about user's\n    office.\n- scope: properties:read\n  label: Properties (Read)\n  description: Developer will be able to see information about user's property.\n- scope: properties:write\n  label: Properties\n  description: Developer will be able to modify and delete information about user's\n    property.\n- scope: reports:read\n  label: Reports\n  description: Developer will be able to read data and metadata of reports.\n- scope: tasks:read\n  label: Tasks (Read)\n  description: Developer will be able to read tasks and task queues on user's account.\n- scope: users:read\n  label: Users (Read)\n  description: Developer will be able to see staff and departments of user's property.\n- scope: users:write\n  label: Users\n  description: Developer will be able to create, modify, and delete staff and\n\
  \    departments.\nmcp_resource_scopes:\n  resource: https://sys.akia.ai/mcp\n  scopes_supported:\n  - customers:read\n  - messages:read\n  source: well-known/akia-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://api.akia.com/docs/scopes\n  http_status: 200\n  content_type: text/html; charset=utf-8\n  note: 'The scope table is server-rendered HTML on Akia''s own developer docs; the\n    16 scopes above are transcribed verbatim from it. No OpenAPI declares them.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akia/refs/heads/main/scopes/akia-scopes.yml
summary_line: 16 scopes · authorizationCode
tags:
- Company
- Hospitality
- Hotels
- Vacation Rentals
- Guest Experience
- Messaging
- Artificial Intelligence
- Agents
- Property Management
- Check-In
token_urls:
- https://api.akia.com/oauth/token
- https://sys.akia.ai/oauth/token
---
