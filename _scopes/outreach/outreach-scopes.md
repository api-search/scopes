---
api_specs:
- filename: outreach-openapi.yml
  format: yaml
  label: Outreach REST API
  slug: outreach-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outreach/refs/heads/main/openapi/outreach-openapi.yml
- filename: outreach-webhooks-asyncapi.yml
  format: yaml
  label: Outreach Webhooks
  slug: outreach-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/outreach/refs/heads/main/webhooks/outreach-webhooks-asyncapi.yml
authorization_urls:
- https://api.outreach.io/oauth/authorize
- https://api.outreach.io/mcpOAuth/authorize
description: ''
docs:
- https://developers.outreach.io/api/getting-started#authorization
- https://developers.outreach.io/api/s2s-access
- https://developers.outreach.io/api/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Outreach Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Outreach publishes 46 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Outreach API on a user''s behalf.


  Tokens are issued from https://api.outreach.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Outreach
provider_slug: outreach
schemes:
- credentials: separate development and production client credentials per Outreach app
  flows:
  - authorizationUrl: https://api.outreach.io/oauth/authorize
    flow: authorizationCode
    refresh: grant_type=refresh_token against the same token URL
    tokenUrl: https://api.outreach.io/oauth/token
  name: OAuth 2.0 (REST API)
  source: https://developers.outreach.io/api/oauth
- flows:
  - authorizationUrl: https://api.outreach.io/mcpOAuth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.outreach.io/mcpOAuth/register
    tokenUrl: https://api.outreach.io/mcpOAuth/token
  name: OAuth 2.1 + Dynamic Client Registration (MCP server)
  source: https://api.outreach.io/.well-known/oauth-authorization-server
- name: S2S application token
  note: Server-to-server; carries application identity, not user identity. Scope set is a strict subset of the OAuth scopes.
  source: https://developers.outreach.io/api/s2s-access
  type: JWT signed with a customer-registered RSA public key
scope_count: 46
scope_names:
- prospects.all
- prospects.read
- prospects.write
- prospects.delete
- accounts.all
- accounts.read
- accounts.write
- accounts.delete
- auditLogs.read
- calls.all
- calls.read
- calls.write
- calls.delete
- events.all
- events.read
- events.write
- imports.all
- imports.read
- imports.write
- kaiaRecordings.read
- mailings.read
- opportunities.all
- opportunities.read
- opportunities.write
- opportunities.delete
- sequenceStates.all
- sequenceStates.read
- sequenceStates.write
- sequenceStates.delete
- sequences.all
- sequences.read
- sequences.write
- sequences.delete
- snippets.read
- tasks.all
- tasks.read
- tasks.write
- tasks.delete
- templates.read
- users.read
- webhooks.all
- webhooks.read
- webhooks.write
- webhooks.delete
- batches.read
- batches.write
scopes:
- description: Full read, write and delete access to prospects.
  flows: []
  scope: prospects.all
- description: Read access to prospects.
  flows: []
  scope: prospects.read
- description: Write access to prospects.
  flows: []
  scope: prospects.write
- description: Delete access to prospects.
  flows: []
  scope: prospects.delete
- description: ''
  flows: []
  scope: accounts.all
- description: ''
  flows: []
  scope: accounts.read
- description: ''
  flows: []
  scope: accounts.write
- description: ''
  flows: []
  scope: accounts.delete
- description: ''
  flows: []
  scope: auditLogs.read
- description: ''
  flows: []
  scope: calls.all
- description: ''
  flows: []
  scope: calls.read
- description: ''
  flows: []
  scope: calls.write
- description: ''
  flows: []
  scope: calls.delete
- description: ''
  flows: []
  scope: events.all
- description: ''
  flows: []
  scope: events.read
- description: ''
  flows: []
  scope: events.write
- description: ''
  flows: []
  scope: imports.all
- description: ''
  flows: []
  scope: imports.read
- description: ''
  flows: []
  scope: imports.write
- description: ''
  flows: []
  scope: kaiaRecordings.read
- description: ''
  flows: []
  scope: mailings.read
- description: ''
  flows: []
  scope: opportunities.all
- description: ''
  flows: []
  scope: opportunities.read
- description: ''
  flows: []
  scope: opportunities.write
- description: ''
  flows: []
  scope: opportunities.delete
- description: ''
  flows: []
  scope: sequenceStates.all
- description: ''
  flows: []
  scope: sequenceStates.read
- description: ''
  flows: []
  scope: sequenceStates.write
- description: ''
  flows: []
  scope: sequenceStates.delete
- description: ''
  flows: []
  scope: sequences.all
- description: ''
  flows: []
  scope: sequences.read
- description: ''
  flows: []
  scope: sequences.write
- description: ''
  flows: []
  scope: sequences.delete
- description: ''
  flows: []
  scope: snippets.read
- description: ''
  flows: []
  scope: tasks.all
- description: ''
  flows: []
  scope: tasks.read
- description: ''
  flows: []
  scope: tasks.write
- description: ''
  flows: []
  scope: tasks.delete
- description: ''
  flows: []
  scope: templates.read
- description: ''
  flows: []
  scope: users.read
- description: ''
  flows: []
  scope: webhooks.all
- description: ''
  flows: []
  scope: webhooks.read
- description: ''
  flows: []
  scope: webhooks.write
- description: ''
  flows: []
  scope: webhooks.delete
- description: Required alongside the target resource's write scope to run bulk/batch actions.
  flows: []
  scope: batches.read
- description: Required alongside the target resource's write scope to run bulk/batch actions.
  flows: []
  scope: batches.write
slug: outreach-scopes
source_filename: outreach-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.outreach.io/api/getting-started#authorization\ndocs:\n- https://developers.outreach.io/api/getting-started#authorization\n- https://developers.outreach.io/api/s2s-access\n- https://developers.outreach.io/api/oauth\nprovider: Outreach\nproviderId: outreach\nnotes: >-\n  The published OpenAPI declares NO oauth2 securityScheme — it models only `bearerAuth` and `s2sAuthToken`\n  as plain HTTP bearer JWTs — so `derive-oauth-scopes.py` finds zero scopes. The scope model is real and\n  fully documented in prose, and the OAuth 2.1 authorization-server metadata at\n  https://api.outreach.io/.well-known/oauth-authorization-server declares its own `scopes_supported`. This\n  file therefore comes from the docs, not the spec. Outreach does not publish a single enumerated table of\n  every OAuth scope; the authoritative list is rendered in the Outreach app's \"API access\" configuration\n  tab, which is behind a customer\
  \ login. Only scopes Outreach actually names in public are recorded below —\n  nothing was extrapolated across resources.\ngrammar:\n  form: <pluralResource>.<level>\n  levels:\n  - read\n  - write\n  - delete\n  - all\n  additive: false\n  additive_note: Scopes are NOT additive — `prospects.write` grants no read access. `all` implies\n    read + write + delete.\n  request_form: space-separated, URL-encoded, in the `scope` query parameter of /oauth/authorize\n  on_missing_scope: 403 with error id `unauthorizedOauthScope`\n  post_scope_check: OAuth scope is the front gate only; the user's Outreach governance/RBAC profile is\n    evaluated separately and returns 403 `unauthorizedRequest` on failure.\nschemes:\n- name: OAuth 2.0 (REST API)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.outreach.io/oauth/authorize\n    tokenUrl: https://api.outreach.io/oauth/token\n    refresh: grant_type=refresh_token against the same token URL\n  credentials: separate development\
  \ and production client credentials per Outreach app\n  source: https://developers.outreach.io/api/oauth\n- name: OAuth 2.1 + Dynamic Client Registration (MCP server)\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://api.outreach.io/mcpOAuth/authorize\n    tokenUrl: https://api.outreach.io/mcpOAuth/token\n    registrationUrl: https://api.outreach.io/mcpOAuth/register\n  source: https://api.outreach.io/.well-known/oauth-authorization-server\n- name: S2S application token\n  type: JWT signed with a customer-registered RSA public key\n  note: Server-to-server; carries application identity, not user identity. Scope set is a strict subset of\n    the OAuth scopes.\n  source: https://developers.outreach.io/api/s2s-access\nscopes:\n- scope: prospects.all\n  description: Full read, write and delete access to prospects.\n  declared_in:\n  - authorization-server metadata (scopes_supported)\n  - S2S available scopes\n  - docs example\n  surfaces:\n  - rest\n  -\
  \ mcp\n  - s2s\n- scope: prospects.read\n  description: Read access to prospects.\n  surfaces:\n  - rest\n  - s2s\n- scope: prospects.write\n  description: Write access to prospects.\n  surfaces:\n  - rest\n  - s2s\n- scope: prospects.delete\n  description: Delete access to prospects.\n  surfaces:\n  - rest\n  - s2s\n- scope: accounts.all\n  surfaces: [rest, s2s]\n- scope: accounts.read\n  surfaces: [rest, s2s]\n- scope: accounts.write\n  surfaces: [rest, s2s]\n- scope: accounts.delete\n  surfaces: [rest, s2s]\n- scope: auditLogs.read\n  surfaces: [rest, s2s]\n- scope: calls.all\n  surfaces: [rest, s2s]\n- scope: calls.read\n  surfaces: [rest, s2s]\n- scope: calls.write\n  surfaces: [rest, s2s]\n- scope: calls.delete\n  surfaces: [rest, s2s]\n- scope: events.all\n  surfaces: [rest, s2s]\n- scope: events.read\n  surfaces: [rest, s2s]\n- scope: events.write\n  surfaces: [rest, s2s]\n- scope: imports.all\n  surfaces: [rest, s2s]\n- scope: imports.read\n  surfaces: [rest, s2s]\n- scope: imports.write\n\
  \  surfaces: [rest, s2s]\n- scope: kaiaRecordings.read\n  surfaces: [rest, s2s]\n- scope: mailings.read\n  surfaces: [rest, s2s]\n- scope: opportunities.all\n  surfaces: [rest, s2s]\n- scope: opportunities.read\n  surfaces: [rest, s2s]\n- scope: opportunities.write\n  surfaces: [rest, s2s]\n- scope: opportunities.delete\n  surfaces: [rest, s2s]\n- scope: sequenceStates.all\n  surfaces: [rest, s2s]\n- scope: sequenceStates.read\n  surfaces: [rest, s2s]\n- scope: sequenceStates.write\n  surfaces: [rest, s2s]\n- scope: sequenceStates.delete\n  surfaces: [rest, s2s]\n- scope: sequences.all\n  surfaces: [rest, s2s]\n- scope: sequences.read\n  surfaces: [rest, s2s]\n- scope: sequences.write\n  surfaces: [rest, s2s]\n- scope: sequences.delete\n  surfaces: [rest, s2s]\n- scope: snippets.read\n  surfaces: [rest, s2s]\n- scope: tasks.all\n  surfaces: [rest, s2s]\n- scope: tasks.read\n  surfaces: [rest, s2s]\n- scope: tasks.write\n  surfaces: [rest, s2s]\n- scope: tasks.delete\n  surfaces: [rest,\
  \ s2s]\n- scope: templates.read\n  surfaces: [rest, s2s]\n- scope: users.read\n  surfaces: [rest, s2s]\n- scope: webhooks.all\n  surfaces: [rest, s2s]\n- scope: webhooks.read\n  surfaces: [rest, s2s]\n- scope: webhooks.write\n  surfaces: [rest, s2s]\n- scope: webhooks.delete\n  surfaces: [rest, s2s]\n- scope: batches.read\n  description: Required alongside the target resource's write scope to run bulk/batch actions.\n  surfaces: [rest]\n  source: https://developers.outreach.io/api/bulk-api\n- scope: batches.write\n  description: Required alongside the target resource's write scope to run bulk/batch actions.\n  surfaces: [rest]\n  source: https://developers.outreach.io/api/bulk-api\nscope_source_note: >-\n  Every scope above is published by Outreach. The `<resource>.<level>` rows for accounts, auditLogs, calls,\n  events, imports, kaiaRecordings, mailings, opportunities, prospects, sequenceStates, sequences, snippets,\n  tasks, templates, users and webhooks are the S2S \"Available scopes\"\
  \ table transcribed verbatim from\n  https://developers.outreach.io/api/s2s-access — Outreach states S2S scopes are a SUBSET of the OAuth\n  scopes, so each also exists on the OAuth surface. `batches.read`/`batches.write` come from the Bulk API\n  page. `prospects.all` is additionally declared machine-readably in the authorization-server metadata.\ngaps:\n- The REST API exposes 51 tagged resources but only 16 resource families appear in any published scope list;\n  scopes for the remaining resources exist but are enumerated only inside the authenticated app-configuration\n  UI.\n- The OpenAPI declares no oauth2 securityScheme and no per-operation scope requirements, so a generated\n  client cannot tell which scope any given call needs.\n- The MCP authorization-server metadata advertises only the prospects.all scope in scopes_supported, which\n  does not cover the 41 tools it serves (accounts, opportunities, sequences, tasks, teams, users, Kaia).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outreach/refs/heads/main/scopes/outreach-scopes.yml
summary_line: 46 scopes · authorizationCode
tags:
- Sales
- Sales Engagement
- Sequences
- CRM
- Email
- Revenue Operations
- Sales Execution
- Prospecting
- Agents
- MCP
token_urls:
- https://api.outreach.io/oauth/token
- https://api.outreach.io/mcpOAuth/token
---
