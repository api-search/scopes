---
authorization_urls: []
description: ''
docs: https://help.cerby.com/developer-tools/cerby-api/generate-an-api-key
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cerby Scopes
name_suffix: OAuth Scopes
note: These are Cerby API KEY scopes, not OAuth 2.0 scopes. Cerby publishes no oauth2 security scheme and no authorization/token endpoint for its public API — authorization is a scope set attached to an X-API-Key at generation time, selected in the Cerby web app, and updatable afterwards. Scopes are recorded here because they are the provider's real, published authorization vocabulary. Display names are quoted verbatim from the developer portal; a machine identifier is recorded ONLY where Cerby published one.
overview: 'Cerby publishes 17 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cerby API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cerby
provider_slug: cerby
schemes:
- in: header
  name: CerbyApiKey
  parameter_name: X-API-Key
  source: https://developer.cerby.com/#authentication
  type: apiKey
scope_count: 17
scope_names:
- Read activities
- Read items
- Read accounts
- Read secrets
- Read users
- Read integrations
- Read automated jobs
- Read vaults
- Read teams
- Write accounts
- Write secrets
- Write users
- Write integrations
- Write automated jobs
- Write collections
- Write teams
- Delete teams
scopes:
- description: Enables reading activity data.
  flows: []
  scope: Read activities
- description: Enables reading account, secret, and collection data.
  flows: []
  scope: Read items
- description: Enables reading account data.
  flows: []
  scope: Read accounts
- description: Enables reading secret data.
  flows: []
  scope: Read secrets
- description: Enables reading user and team data.
  flows: []
  scope: Read users
- description: Enables reading integration and entitlement data.
  flows: []
  scope: Read integrations
- description: Enables reading automated job data.
  flows: []
  scope: Read automated jobs
- description: Enables reading vault data.
  flows: []
  scope: Read vaults
- description: Enables reading team data.
  flows: []
  scope: Read teams
- description: Enables writing account data.
  flows: []
  scope: Write accounts
- description: Enables writing secret data.
  flows: []
  scope: Write secrets
- description: Enables writing user data.
  flows: []
  scope: Write users
- description: Enables writing integration and entitlement data.
  flows: []
  scope: Write integrations
- description: Enables writing automated job data.
  flows: []
  scope: Write automated jobs
- description: Enables writing collection and subcollection data.
  flows: []
  scope: Write collections
- description: Enables writing team data.
  flows: []
  scope: Write teams
- description: Enables deleting team data.
  flows: []
  scope: Delete teams
slug: cerby-scopes
source_filename: cerby-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://developer.cerby.com/#authentication\ndocs: https://help.cerby.com/developer-tools/cerby-api/generate-an-api-key\nscheme_type: apiKey\nnote: >-\n  These are Cerby API KEY scopes, not OAuth 2.0 scopes. Cerby publishes no\n  oauth2 security scheme and no authorization/token endpoint for its public API\n  — authorization is a scope set attached to an X-API-Key at generation time,\n  selected in the Cerby web app, and updatable afterwards. Scopes are recorded\n  here because they are the provider's real, published authorization vocabulary.\n  Display names are quoted verbatim from the developer portal; a machine\n  identifier is recorded ONLY where Cerby published one.\nschemes:\n- name: CerbyApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  source: https://developer.cerby.com/#authentication\nenforcement:\n  missing_or_wrong_scope: 401\n  insufficient_permission: 403\n  note: >-\n    Scopes are necessary\
  \ but not sufficient. RBAC is enforced on top: a key only\n    reaches items whose Owner role its creating user holds. All-Access Mode is\n    not honored by the API.\nscopes:\n- scope: Read activities\n  description: Enables reading activity data.\n  access: read\n- scope: Read items\n  description: Enables reading account, secret, and collection data.\n  access: read\n- scope: Read accounts\n  description: Enables reading account data.\n  access: read\n- scope: Read secrets\n  description: Enables reading secret data.\n  access: read\n- scope: Read users\n  description: Enables reading user and team data.\n  access: read\n- scope: Read integrations\n  description: Enables reading integration and entitlement data.\n  access: read\n- scope: Read automated jobs\n  identifier: read:automations\n  description: Enables reading automated job data.\n  access: read\n  identifier_source: https://help.cerby.com/developer-tools/cerby-webhooks/implement-a-webhook-receiver\n- scope: Read vaults\n\
  \  description: Enables reading vault data.\n  access: read\n- scope: Read teams\n  description: Enables reading team data.\n  access: read\n- scope: Write accounts\n  description: Enables writing account data.\n  access: write\n- scope: Write secrets\n  description: Enables writing secret data.\n  access: write\n- scope: Write users\n  description: Enables writing user data.\n  access: write\n- scope: Write integrations\n  description: Enables writing integration and entitlement data.\n  access: write\n- scope: Write automated jobs\n  description: Enables writing automated job data.\n  access: write\n- scope: Write collections\n  description: Enables writing collection and subcollection data.\n  access: write\n- scope: Write teams\n  description: Enables writing team data.\n  access: write\n- scope: Delete teams\n  description: Enables deleting team data.\n  access: delete\nsummary:\n  total: 17\n  read: 9\n  write: 7\n  delete: 1\nx-evidence:\n- url: https://developer.cerby.com/\n  http_status:\
  \ 200\n  fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerby/refs/heads/main/scopes/cerby-scopes.yml
summary_line: 17 scopes
tags:
- Identity
- Access Management
- Security
- Password Management
- Provisioning
- SCIM
- Identity Governance
- Nonfederated Applications
- Automation
- Webhook
token_urls: []
---
