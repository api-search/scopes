---
api_specs:
- filename: amigo-classic-openapi-original.json
  format: json
  label: Amigo Classic API
  slug: amigo-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/openapi/amigo-classic-openapi-original.json
- filename: amigo-platform-openapi-original.json
  format: json
  label: Amigo Platform API
  slug: amigo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/openapi/amigo-platform-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.amigo.ai/developer-guide/platform-api/platform-api/oauth2.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Amigo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Amigo publishes 53 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Amigo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Amigo
provider_slug: amigo
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  source: https://api.platform.amigo.ai/.well-known/openid-configuration
  tokenUrl: https://identity.platform.amigo.ai/token
  token_lifetime_seconds: 3600
  type: oauth2
scope_count: 53
scope_names:
- agents:read
- agents:write
- audit:read
- calls:initiate
- calls:inject
- calls:read
- context_graphs:read
- context_graphs:write
- conversations:approve_own
- conversations:close_own
- conversations:create
- conversations:read_own
- conversations:turn
- credentials:read
- credentials:write
- data_sources:read
- data_sources:sync
- data_sources:write
- entities:delete
- entities:read
- entities:write
- events:read
- events:write
- external_user_sessions:create
- identity:admin
- identity:e2e-auth:read
- phone_numbers:provision
- phone_numbers:read
- platform:admin
- provider_scribe_sessions:create
- review:approve
- review:read
- scribe:access:manage
- scribe:appointments:read_own
- scribe:encounters:read_own
- scribe:impersonate
- scribe:notes:rw_own
- scribe:records:delete
- scribe:sessions:read_all
- scribe:sessions:read_own
- scribe:sessions:write
- services:read
- services:write
- sessions:create
- skills:read
- skills:write
- surfaces:read
- surfaces:write
- tools:execute
- tools:test
- tools:write
- workspaces:read
- workspaces:write
scopes:
- description: ''
  flows: []
  scope: agents:read
- description: ''
  flows: []
  scope: agents:write
- description: ''
  flows: []
  scope: audit:read
- description: ''
  flows: []
  scope: calls:initiate
- description: ''
  flows: []
  scope: calls:inject
- description: ''
  flows: []
  scope: calls:read
- description: ''
  flows: []
  scope: context_graphs:read
- description: ''
  flows: []
  scope: context_graphs:write
- description: ''
  flows: []
  scope: conversations:approve_own
- description: ''
  flows: []
  scope: conversations:close_own
- description: ''
  flows: []
  scope: conversations:create
- description: ''
  flows: []
  scope: conversations:read_own
- description: ''
  flows: []
  scope: conversations:turn
- description: ''
  flows: []
  scope: credentials:read
- description: ''
  flows: []
  scope: credentials:write
- description: ''
  flows: []
  scope: data_sources:read
- description: ''
  flows: []
  scope: data_sources:sync
- description: ''
  flows: []
  scope: data_sources:write
- description: ''
  flows: []
  scope: entities:delete
- description: ''
  flows: []
  scope: entities:read
- description: ''
  flows: []
  scope: entities:write
- description: ''
  flows: []
  scope: events:read
- description: ''
  flows: []
  scope: events:write
- description: ''
  flows: []
  scope: external_user_sessions:create
- description: ''
  flows: []
  scope: identity:admin
- description: ''
  flows: []
  scope: identity:e2e-auth:read
- description: ''
  flows: []
  scope: phone_numbers:provision
- description: ''
  flows: []
  scope: phone_numbers:read
- description: ''
  flows: []
  scope: platform:admin
- description: ''
  flows: []
  scope: provider_scribe_sessions:create
- description: ''
  flows: []
  scope: review:approve
- description: ''
  flows: []
  scope: review:read
- description: ''
  flows: []
  scope: scribe:access:manage
- description: ''
  flows: []
  scope: scribe:appointments:read_own
- description: ''
  flows: []
  scope: scribe:encounters:read_own
- description: ''
  flows: []
  scope: scribe:impersonate
- description: ''
  flows: []
  scope: scribe:notes:rw_own
- description: ''
  flows: []
  scope: scribe:records:delete
- description: ''
  flows: []
  scope: scribe:sessions:read_all
- description: ''
  flows: []
  scope: scribe:sessions:read_own
- description: ''
  flows: []
  scope: scribe:sessions:write
- description: ''
  flows: []
  scope: services:read
- description: ''
  flows: []
  scope: services:write
- description: ''
  flows: []
  scope: sessions:create
- description: ''
  flows: []
  scope: skills:read
- description: ''
  flows: []
  scope: skills:write
- description: ''
  flows: []
  scope: surfaces:read
- description: ''
  flows: []
  scope: surfaces:write
- description: ''
  flows: []
  scope: tools:execute
- description: ''
  flows: []
  scope: tools:test
- description: ''
  flows: []
  scope: tools:write
- description: ''
  flows: []
  scope: workspaces:read
- description: ''
  flows: []
  scope: workspaces:write
slug: amigo-scopes
source_filename: amigo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://api.platform.amigo.ai/.well-known/openid-configuration\ndocs: https://docs.amigo.ai/developer-guide/platform-api/platform-api/oauth2.md\nnotes: Amigo Platform API supports OAuth2 client_credentials (machine-to-machine). Token endpoint https://identity.platform.amigo.ai/token\n  (also documented as POST /v1/oauth/token). Scopes below are the authoritative scopes_supported list published in the OpenID\n  Connect discovery document. Wildcard patterns (e.g. sms:*) are supported for low-privilege scopes; high-privilege scopes\n  require exact match. Granted scope = intersection of requested and granted.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://identity.platform.amigo.ai/token\n  token_lifetime_seconds: 3600\n  source: https://api.platform.amigo.ai/.well-known/openid-configuration\ngrant_types_supported:\n- api_key\n- client_credentials\n- personal_access_token\n\
  - agent_session\n- google_oauth\n- email_otp\n- magic_link\n- refresh_token\n- urn:ietf:params:oauth:grant-type:device_code\nscope_count: 53\nscopes:\n- scope: agents:read\n  resource: agents\n  action: read\n- scope: agents:write\n  resource: agents\n  action: write\n- scope: audit:read\n  resource: audit\n  action: read\n- scope: calls:initiate\n  resource: calls\n  action: initiate\n- scope: calls:inject\n  resource: calls\n  action: inject\n- scope: calls:read\n  resource: calls\n  action: read\n- scope: context_graphs:read\n  resource: context_graphs\n  action: read\n- scope: context_graphs:write\n  resource: context_graphs\n  action: write\n- scope: conversations:approve_own\n  resource: conversations\n  action: approve_own\n- scope: conversations:close_own\n  resource: conversations\n  action: close_own\n- scope: conversations:create\n  resource: conversations\n  action: create\n- scope: conversations:read_own\n  resource: conversations\n  action: read_own\n- scope: conversations:turn\n\
  \  resource: conversations\n  action: turn\n- scope: credentials:read\n  resource: credentials\n  action: read\n- scope: credentials:write\n  resource: credentials\n  action: write\n- scope: data_sources:read\n  resource: data_sources\n  action: read\n- scope: data_sources:sync\n  resource: data_sources\n  action: sync\n- scope: data_sources:write\n  resource: data_sources\n  action: write\n- scope: entities:delete\n  resource: entities\n  action: delete\n- scope: entities:read\n  resource: entities\n  action: read\n- scope: entities:write\n  resource: entities\n  action: write\n- scope: events:read\n  resource: events\n  action: read\n- scope: events:write\n  resource: events\n  action: write\n- scope: external_user_sessions:create\n  resource: external_user_sessions\n  action: create\n- scope: identity:admin\n  resource: identity\n  action: admin\n- scope: identity:e2e-auth:read\n  resource: identity\n  action: e2e-auth:read\n- scope: phone_numbers:provision\n  resource: phone_numbers\n\
  \  action: provision\n- scope: phone_numbers:read\n  resource: phone_numbers\n  action: read\n- scope: platform:admin\n  resource: platform\n  action: admin\n- scope: provider_scribe_sessions:create\n  resource: provider_scribe_sessions\n  action: create\n- scope: review:approve\n  resource: review\n  action: approve\n- scope: review:read\n  resource: review\n  action: read\n- scope: scribe:access:manage\n  resource: scribe\n  action: access:manage\n- scope: scribe:appointments:read_own\n  resource: scribe\n  action: appointments:read_own\n- scope: scribe:encounters:read_own\n  resource: scribe\n  action: encounters:read_own\n- scope: scribe:impersonate\n  resource: scribe\n  action: impersonate\n- scope: scribe:notes:rw_own\n  resource: scribe\n  action: notes:rw_own\n- scope: scribe:records:delete\n  resource: scribe\n  action: records:delete\n- scope: scribe:sessions:read_all\n  resource: scribe\n  action: sessions:read_all\n- scope: scribe:sessions:read_own\n  resource: scribe\n  action:\
  \ sessions:read_own\n- scope: scribe:sessions:write\n  resource: scribe\n  action: sessions:write\n- scope: services:read\n  resource: services\n  action: read\n- scope: services:write\n  resource: services\n  action: write\n- scope: sessions:create\n  resource: sessions\n  action: create\n- scope: skills:read\n  resource: skills\n  action: read\n- scope: skills:write\n  resource: skills\n  action: write\n- scope: surfaces:read\n  resource: surfaces\n  action: read\n- scope: surfaces:write\n  resource: surfaces\n  action: write\n- scope: tools:execute\n  resource: tools\n  action: execute\n- scope: tools:test\n  resource: tools\n  action: test\n- scope: tools:write\n  resource: tools\n  action: write\n- scope: workspaces:read\n  resource: workspaces\n  action: read\n- scope: workspaces:write\n  resource: workspaces\n  action: write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/scopes/amigo-scopes.yml
summary_line: 53 scopes
tags:
- Company
- Ai
- Healthcare
- AI Agents
- Voice
- Clinical
- Conversational AI
- FHIR
- EHR
- HIPAA
token_urls: []
---
