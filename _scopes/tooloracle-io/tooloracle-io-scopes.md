---
api_specs:
- filename: tooloracle-io-mcp-platform-openapi.yml
  format: yaml
  label: ToolOracle MCP Platform API
  slug: tooloracle-mcp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-mcp-platform-openapi.yml
- filename: tooloracle-io-x402-v2-openapi.yml
  format: yaml
  label: ToolOracle x402 v2 Compliance, Evidence & Agent-Safety API
  slug: tooloracle-x402-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-x402-v2-openapi.yml
- filename: tooloracle-io-feedoracle-compliance-evidence-openapi.yml
  format: yaml
  label: FeedOracle Compliance Evidence API
  slug: feedoracle-compliance-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-feedoracle-compliance-evidence-openapi.yml
authorization_urls:
- https://feedoracle.io/mcp/authorize
description: ''
docs: https://feedoracle.io/docs/mcp-auth.html
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Tooloracle Io Scopes
name_suffix: OAuth Scopes
note: None of the three OpenAPIs declares an oauth2 securityScheme (derive-oauth-scopes.py found 0), so this file is built from the RFC 8414 / RFC 9728 discovery documents both brands serve. The scopes are NAMED in scopes_supported but the provider publishes no per-scope description anywhere that was fetched; `meaning` below is what the name states and nothing more.
overview: 'FeedOracle Technologies publishes 8 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the FeedOracle Technologies API on a user''s behalf.


  Tokens are issued from https://feedoracle.io/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FeedOracle Technologies
provider_slug: tooloracle-io
schemes:
- flows:
  - authorizationUrl: https://feedoracle.io/mcp/authorize
    flow: authorizationCode
    pkce: S256 (only method supported)
    tokenUrl: https://feedoracle.io/mcp/token
  - flow: clientCredentials
    note: 'documented one-call flow in llms.txt: register at /mcp/register, then grant_type=client_credentials&scope=mcp:read -> 1-hour bearer (prefix fo_cc_)'
    tokenUrl: https://feedoracle.io/mcp/token
  - flow: refreshToken
    tokenUrl: https://feedoracle.io/mcp/token
  issuer: https://feedoracle.io
  jwks: https://feedoracle.io/.well-known/jwks.json
  name: OAuth 2.1 (feedoracle.io issuer, used by both brands)
  registration: https://feedoracle.io/mcp/register (RFC 7591 dynamic client registration)
  revocation: https://feedoracle.io/mcp/revoke
  source: well-known/tooloracle-io-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
scope_count: 8
scope_names:
- mcp:read
- mcp:tools:read
- mcp:oracles:read
- mcp:compliance:read
- mcp:risk:read
- mcp:macro:read
- mcp:verified-reports:read
- openid
scopes:
- description: ''
  flows: []
  scope: mcp:read
- description: ''
  flows: []
  scope: mcp:tools:read
- description: ''
  flows: []
  scope: mcp:oracles:read
- description: ''
  flows: []
  scope: mcp:compliance:read
- description: ''
  flows: []
  scope: mcp:risk:read
- description: ''
  flows: []
  scope: mcp:macro:read
- description: ''
  flows: []
  scope: mcp:verified-reports:read
- description: ''
  flows: []
  scope: openid
slug: tooloracle-io-scopes
source_filename: tooloracle-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://tooloracle.io/.well-known/oauth-authorization-server, https://tooloracle.io/.well-known/oauth-protected-resource, https://feedoracle.io/.well-known/oauth-authorization-server, https://feedoracle.io/.well-known/openid-configuration, https://feedoracle.io/.well-known/oauth-protected-resource, https://tooloracle.io/llms.txt\ndocs: https://feedoracle.io/docs/mcp-auth.html\nnote: >-\n  None of the three OpenAPIs declares an oauth2 securityScheme (derive-oauth-scopes.py found 0), so this file is built from the\n  RFC 8414 / RFC 9728 discovery documents both brands serve. The scopes are NAMED in scopes_supported but the provider publishes\n  no per-scope description anywhere that was fetched; `meaning` below is what the name states and nothing more.\nschemes:\n- name: OAuth 2.1 (feedoracle.io issuer, used by both brands)\n  issuer: https://feedoracle.io\n  source: well-known/tooloracle-io-oauth-authorization-server.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://feedoracle.io/mcp/authorize\n    tokenUrl: https://feedoracle.io/mcp/token\n    pkce: S256 (only method supported)\n  - flow: clientCredentials\n    tokenUrl: https://feedoracle.io/mcp/token\n    note: 'documented one-call flow in llms.txt: register at /mcp/register, then grant_type=client_credentials&scope=mcp:read -> 1-hour bearer (prefix fo_cc_)'\n  - flow: refreshToken\n    tokenUrl: https://feedoracle.io/mcp/token\n  registration: https://feedoracle.io/mcp/register (RFC 7591 dynamic client registration)\n  revocation: https://feedoracle.io/mcp/revoke\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n  jwks: https://feedoracle.io/.well-known/jwks.json\nscopes:\n- {scope: 'mcp:read', meaning: baseline MCP read access; the scope llms.txt uses in its example, resources: [tooloracle.io, feedoracle.io], sources: [tooloracle.io AS, feedoracle.io AS, both PRM docs]}\n- {scope: 'mcp:tools:read',\
  \ meaning: read/list tools (name only), resources: [tooloracle.io], sources: [tooloracle.io AS, tooloracle.io PRM]}\n- {scope: 'mcp:oracles:read', meaning: read oracle catalog (name only), resources: [tooloracle.io], sources: [tooloracle.io AS, tooloracle.io PRM]}\n- {scope: 'mcp:compliance:read', meaning: compliance oracle tools (name only), resources: [tooloracle.io, feedoracle.io], sources: [both AS, both PRM]}\n- {scope: 'mcp:risk:read', meaning: stablecoin/RWA risk server (name only), resources: [feedoracle.io], sources: [tooloracle.io AS, feedoracle.io AS, feedoracle.io PRM]}\n- {scope: 'mcp:macro:read', meaning: macro intelligence server (name only), resources: [feedoracle.io], sources: [tooloracle.io AS, feedoracle.io AS, feedoracle.io PRM]}\n- {scope: 'mcp:verified-reports:read', meaning: verified reports API (name only), resources: [feedoracle.io], sources: [tooloracle.io AS, feedoracle.io AS, feedoracle.io PRM]}\n- {scope: openid, meaning: OIDC id_token (ES256K), resources:\
  \ [feedoracle.io], sources: [feedoracle.io openid-configuration]}\nresource_scope_matrix:\n  note: The tooloracle.io protected-resource document accepts only mcp:read, mcp:tools:read, mcp:oracles:read and mcp:compliance:read; a token carrying mcp:risk:read or mcp:macro:read is meaningful only on feedoracle.io resources.\nother_scope_systems:\n- name: AgentGuard role scopes\n  note: '\"6 role scopes (admin/compliance/trader/auditor/developer/readonly)\" and \"144 scopes\" (homepage, /trust/) — an AgentGuard policy vocabulary, not OAuth scopes; the AgentGuard endpoints were 404 on the probe day so it could not be captured.'\n- name: KYA trust levels\n  note: 'docs/mcp-auth.html: 0 UNVERIFIED (free tools), 1 KNOWN (all tools), 2 TRUSTED (+reports), 3 CERTIFIED (+priority SLA) — gates access alongside scopes.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/scopes/tooloracle-io-scopes.yml
summary_line: 8 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- MCP
- Agent Infrastructure
- A2A
- x402
- Micropayments
- Compliance
- RegTech
- Blockchain
- Sanctions Screening
- Agent Discovery
- Germany
token_urls:
- https://feedoracle.io/mcp/token
---
