---
api_specs:
- filename: usergems-accounts-api-openapi.yml
  format: yaml
  label: UserGems Accounts API
  slug: usergems-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-accounts-api-openapi.yml
- filename: usergems-contacts-api-openapi.yml
  format: yaml
  label: UserGems Contacts API
  slug: usergems-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-contacts-api-openapi.yml
- filename: usergems-privacy-api-openapi.yml
  format: yaml
  label: UserGems Privacy API
  slug: usergems-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-privacy-api-openapi.yml
authorization_urls:
- https://app.usergems.com/mcp/oauth/authorize
description: UserGems' REST API has no OAuth surface — it authenticates with a single company-wide X-Api-Key header. The OAuth surface belongs entirely to the UserGems MCP server, whose RFC 8414 authorization-server metadata is served anonymously at app.usergems.com and declares exactly one scope. UserGems publishes no scope/permission reference page; the scope set below is read directly from the provider's own discovery document, not from prose.
docs: https://help.usergems.com/article/mcp-early-access-chatgpt
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Usergems Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'UserGems publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the UserGems API on a user''s behalf.


  Tokens are issued from https://app.usergems.com/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: UserGems
provider_slug: usergems
schemes:
- dynamic_client_registration: true
  flows:
  - authorizationUrl: https://app.usergems.com/mcp/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    refresh: true
    scopes:
      mcp:use: Call the UserGems MCP server on behalf of the signed-in UserGems user.
    tokenUrl: https://app.usergems.com/mcp/oauth/token
  issuer: https://app.usergems.com
  name: UserGemsMCP
  registration_endpoint: https://app.usergems.com/mcp/oauth/register
  source: well-known/usergems-oauth-authorization-server.json
  type: oauth2
scope_count: 1
scope_names:
- mcp:use
scopes:
- description: 'The single scope the UserGems authorization server advertises. It is coarse-grained: it does not separate read from write, so one grant covers account/prospect lookup as well as campaign creation, CRM writes and sequence enrollment.'
  flows:
  - authorizationCode
  scope: mcp:use
slug: usergems-scopes
source_filename: usergems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.usergems.com/.well-known/oauth-authorization-server\ndocs: https://help.usergems.com/article/mcp-early-access-chatgpt\ndescription: >-\n  UserGems' REST API has no OAuth surface — it authenticates with a single\n  company-wide X-Api-Key header. The OAuth surface belongs entirely to the\n  UserGems MCP server, whose RFC 8414 authorization-server metadata is served\n  anonymously at app.usergems.com and declares exactly one scope. UserGems\n  publishes no scope/permission reference page; the scope set below is read\n  directly from the provider's own discovery document, not from prose.\nschemes:\n  - name: UserGemsMCP\n    type: oauth2\n    source: well-known/usergems-oauth-authorization-server.json\n    issuer: https://app.usergems.com\n    registration_endpoint: https://app.usergems.com/mcp/oauth/register\n    dynamic_client_registration: true\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://app.usergems.com/mcp/oauth/authorize\n        tokenUrl: https://app.usergems.com/mcp/oauth/token\n        pkce: [S256]\n        refresh: true\n        scopes:\n          mcp:use: Call the UserGems MCP server on behalf of the signed-in UserGems user.\nscopes:\n  - scope: mcp:use\n    description: >-\n      The single scope the UserGems authorization server advertises. It is\n      coarse-grained: it does not separate read from write, so one grant covers\n      account/prospect lookup as well as campaign creation, CRM writes and\n      sequence enrollment.\n    flows: [authorizationCode]\n    sources:\n      - well-known/usergems-oauth-authorization-server.json\n      - well-known/usergems-oauth-protected-resource.json\n    resource: https://app.usergems.com/mcp/usergems\nauthorization_model:\n  granularity: single-scope\n  effective_permissions: >-\n    Delegated from the authorizing user's own UserGems account — \"Each person\n    still signs in with their own UserGems login\
  \ and their own permissions.\"\n    The scope does not narrow them further.\n  consequence: >-\n    Because there is no read-only scope, least-privilege for an agent cannot be\n    expressed at the token. UserGems' documented mitigation is client-side\n    approval prompts (Claude per-tool approval; ChatGPT permission tiers), which\n    is a client control, not a server-enforced one.\n  documented_gap: >-\n    Separately, the REST API has no scope model at all: \"there is one key per\n    company, shared across all integrations. There is no way to issue separate\n    keys per system, isolate a misbehaving integration, or create a sandbox key\n    for testing.\"\n    (https://help.usergems.com/article/using-the-usergems-api)\nx-evidence:\n  - fetched: '2026-08-13'\n    url: https://app.usergems.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://app.usergems.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/scopes/usergems-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Sales Intelligence
- Outbound
- Account Based Marketing
- Champion Tracking
- Job Changes
- Buying Signals
- AI Scoring
- Sales Engagement
- CRM
- Revenue Operations
- Go-To-Market
- MCP
- AI Agents
token_urls:
- https://app.usergems.com/mcp/oauth/token
---
