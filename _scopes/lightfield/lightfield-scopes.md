---
api_specs:
- filename: lightfield-openapi-original.yml
  format: yaml
  label: Lightfield API
  slug: lightfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/openapi/lightfield-openapi-original.yml
authorization_urls: []
description: ''
docs: https://docs.lightfield.app/using-the-api/scopes/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Lightfield Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lightfield publishes 26 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lightfield API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lightfield
provider_slug: lightfield
schemes:
- key_prefix: sk_lf_
  management_url: https://crm.lightfield.app/crm/settings/api-keys
  name: bearerAuth
  scheme: bearer
  scope_binding: at key creation (admin only)
  source: openapi/lightfield-openapi-original.yml
  type: http
scope_count: 26
scope_names:
- accounts:create
- accounts:update
- accounts:read
- contacts:create
- contacts:update
- contacts:read
- opportunities:create
- opportunities:update
- opportunities:read
- meetings:create
- meetings:update
- meetings:read
- tasks:create
- tasks:update
- tasks:read
- notes:create
- notes:update
- notes:read
- lists:create
- lists:update
- lists:read
- files:create
- files:read
- emails:create
- emails:read
- members:read
scopes:
- description: Create accounts
  flows: []
  scope: accounts:create
- description: Update accounts
  flows: []
  scope: accounts:update
- description: Read accounts
  flows: []
  scope: accounts:read
- description: Create contacts
  flows: []
  scope: contacts:create
- description: Update contacts
  flows: []
  scope: contacts:update
- description: Read contacts
  flows: []
  scope: contacts:read
- description: Create opportunities
  flows: []
  scope: opportunities:create
- description: Update opportunities
  flows: []
  scope: opportunities:update
- description: Read opportunities
  flows: []
  scope: opportunities:read
- description: Create meetings
  flows: []
  scope: meetings:create
- description: Update meetings
  flows: []
  scope: meetings:update
- description: Read meetings
  flows: []
  scope: meetings:read
- description: Create tasks
  flows: []
  scope: tasks:create
- description: Update tasks
  flows: []
  scope: tasks:update
- description: Read tasks
  flows: []
  scope: tasks:read
- description: Create notes
  flows: []
  scope: notes:create
- description: Update notes
  flows: []
  scope: notes:update
- description: Read notes
  flows: []
  scope: notes:read
- description: Create lists
  flows: []
  scope: lists:create
- description: Update lists
  flows: []
  scope: lists:update
- description: Read lists
  flows: []
  scope: lists:read
- description: Create, complete, and cancel file uploads
  flows: []
  scope: files:create
- description: Read files and signed download URLs
  flows: []
  scope: files:read
- description: Send emails through connected mailboxes
  flows: []
  scope: emails:create
- description: Read synced emails
  flows: []
  scope: emails:read
- description: Read members
  flows: []
  scope: members:read
slug: lightfield-scopes
source_filename: lightfield-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lightfield-openapi-original.yml\ndocs: https://docs.lightfield.app/using-the-api/scopes/\nmodel: api-key-scopes\nnotes: >-\n  Lightfield's REST API does not use OAuth 2 — the mechanical OAuth derivation over the OpenAPI\n  found no oauth2 security scheme. Scopes are nonetheless a real, published permission surface:\n  they are selected at API-key creation time and bound to the key, following an\n  `<object>:<permission>` naming convention. A key's effective access is the intersection of its\n  granted scopes and the roles of the admin who created it. Separately, the hosted MCP server at\n  mcp.lightfield.app uses OAuth 2.1 with its own (much smaller) scope set — recorded below under\n  oauth_scopes.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  key_prefix: sk_lf_\n  source: openapi/lightfield-openapi-original.yml\n  scope_binding: at key creation (admin only)\n  management_url: https://crm.lightfield.app/crm/settings/api-keys\n\
  scope_convention: '<object>:<create|update|read>'\nscopes:\n- scope: accounts:create\n  description: Create accounts\n- scope: accounts:update\n  description: Update accounts\n- scope: accounts:read\n  description: Read accounts\n- scope: contacts:create\n  description: Create contacts\n- scope: contacts:update\n  description: Update contacts\n- scope: contacts:read\n  description: Read contacts\n- scope: opportunities:create\n  description: Create opportunities\n- scope: opportunities:update\n  description: Update opportunities\n- scope: opportunities:read\n  description: Read opportunities\n- scope: meetings:create\n  description: Create meetings\n- scope: meetings:update\n  description: Update meetings\n- scope: meetings:read\n  description: Read meetings\n- scope: tasks:create\n  description: Create tasks\n- scope: tasks:update\n  description: Update tasks\n- scope: tasks:read\n  description: Read tasks\n- scope: notes:create\n  description: Create notes\n- scope: notes:update\n  description:\
  \ Update notes\n- scope: notes:read\n  description: Read notes\n- scope: lists:create\n  description: Create lists\n- scope: lists:update\n  description: Update lists\n- scope: lists:read\n  description: Read lists\n- scope: files:create\n  description: Create, complete, and cancel file uploads\n- scope: files:read\n  description: Read files and signed download URLs\n- scope: emails:create\n  description: Send emails through connected mailboxes\n- scope: emails:read\n  description: Read synced emails\n- scope: members:read\n  description: Read members\nscope_count: 26\noauth_scopes:\n  context: hosted MCP server (https://mcp.lightfield.app/mcp)\n  issuer: https://api.stytch.lightfield.app\n  metadata: well-known/lightfield-oauth-authorization-server.json\n  scopes:\n  - scope: openid\n    description: OpenID Connect authentication\n  - scope: offline_access\n    description: Refresh-token issuance for long-lived agent sessions\nenforcement:\n  insufficient_scope_status: 403\n  insufficient_scope_type:\
  \ forbidden\nguidance:\n- Grant only the scopes an integration requires; restrict to read-only scopes where no mutation is\n  needed.\n- Create dedicated keys per integration so access can be revoked independently.\n- Rotate keys periodically; revocation is immediate and permanent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightfield/refs/heads/main/scopes/lightfield-scopes.yml
summary_line: 26 scopes
tags:
- Company
- Applications
- CRM
- Sales
- Artificial Intelligence
- Agents
- Customer Relationship Management
- Go To Market
- Productivity
- SaaS
token_urls: []
---
