---
authorization_urls:
- https://www.wyndhambusiness.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Wyndham Hotels Scopes
name_suffix: OAuth Scopes
note: 'The only OAuth surface anywhere on the Wyndham Hotels & Resorts estate is the authorization server bound to the WordPress MCP server on www.wyndhambusiness.com. Its published metadata advertises exactly one scope — `mcp` — on both the authorization server and the protected resource. There is no scopes or permissions reference page on any Wyndham property, no per-resource or per-operation scope decomposition, and no client-credentials surface, so this records the full and minimal real catalogue rather than a curated one. Nothing is inferred: a coarse single-scope catalogue is what the provider actually publishes.'
overview: 'Wyndham Hotels & Resorts publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wyndham Hotels & Resorts API on a user''s behalf.


  Tokens are issued from https://www.wyndhambusiness.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wyndham Hotels & Resorts
provider_slug: wyndham-hotels
schemes:
- flows:
  - authorizationUrl: https://www.wyndhambusiness.com/oauth/authorize
    flow: authorizationCode
    pkce: S256 (required)
    tokenUrl: https://www.wyndhambusiness.com/oauth/token
  issuer: https://www.wyndhambusiness.com
  name: wyndham-business-mcp-oauth
  source: well-known/wyndham-hotels-wyndhambusiness-oauth-authorization-server.json
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Bearer-token access to the WordPress MCP server at https://www.wyndhambusiness.com/wp-json/mcp/mcp-oauth-server. It is a single coarse capability scope covering the whole MCP surface — the underlying tool set (the site's registered wp-abilities) is itself gated and unreadable, so the effective permissions this scope confers cannot be enumerated from public data.
  flows:
  - authorizationCode
  scope: mcp
slug: wyndham-hotels-scopes
source_filename: wyndham-hotels-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://www.wyndhambusiness.com/.well-known/oauth-authorization-server (RFC\n  8414) and https://www.wyndhambusiness.com/.well-known/oauth-protected-resource\n  (RFC 9728), fetched 2026-07-28\ndocs: null\nnote: |\n  The only OAuth surface anywhere on the Wyndham Hotels & Resorts estate is the\n  authorization server bound to the WordPress MCP server on www.wyndhambusiness.com.\n  Its published metadata advertises exactly one scope — `mcp` — on both the\n  authorization server and the protected resource. There is no scopes or\n  permissions reference page on any Wyndham property, no per-resource or\n  per-operation scope decomposition, and no client-credentials surface, so this\n  records the full and minimal real catalogue rather than a curated one. Nothing is\n  inferred: a coarse single-scope catalogue is what the provider actually publishes.\nschemes:\n- name: wyndham-business-mcp-oauth\n  type: oauth2\n  source: well-known/wyndham-hotels-wyndhambusiness-oauth-authorization-server.json\n\
  \  issuer: https://www.wyndhambusiness.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wyndhambusiness.com/oauth/authorize\n    tokenUrl: https://www.wyndhambusiness.com/oauth/token\n    pkce: S256 (required)\nscopes:\n- scope: mcp\n  description: |\n    Bearer-token access to the WordPress MCP server at\n    https://www.wyndhambusiness.com/wp-json/mcp/mcp-oauth-server. It is a single\n    coarse capability scope covering the whole MCP surface — the underlying tool set\n    (the site's registered wp-abilities) is itself gated and unreadable, so the\n    effective permissions this scope confers cannot be enumerated from public data.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/wyndham-hotels-wyndhambusiness-oauth-authorization-server.json\n  - well-known/wyndham-hotels-wyndhambusiness-oauth-protected-resource.json\ncoverage:\n  scope_count: 1\n  data_scopes: 0\n  client_credentials_scopes: 0\n  read_write_split: false\ncross_references:\n  authentication:\
  \ authentication/wyndham-hotels-authentication.yml\n  mcp: mcp/wyndham-hotels-mcp.yml\n  well_known: well-known/wyndham-hotels-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyndham-hotels/refs/heads/main/scopes/wyndham-hotels-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Franchising
- Distribution
- Loyalty
- GDS
token_urls:
- https://www.wyndhambusiness.com/oauth/token
---
