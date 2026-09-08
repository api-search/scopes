---
api_specs:
- filename: openapi.json
  format: json
  label: 0xArchive REST API
  slug: 0xarchive-rest-api
  spec_type: OpenAPI
  url: https://0xarchive.io/openapi.json
authorization_urls: []
description: ''
docs: https://docs.0xarchive.io/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: 0Xarchive Scopes
name_suffix: OAuth Scopes
note: 'These scopes govern the hosted MCP surface ONLY, not the REST API. The REST API uses an X-API-Key header with no scope model at all - 0-working/derive-oauth-scopes.py correctly found zero oauth2 securitySchemes in the OpenAPI, because there are none. The scopes below are read from the provider''s live RFC 8414 authorization-server metadata, which is why this file is method: searched rather than derived. Two facts about this list are worth reading together. First, the authorization server advertises SIX scopes covering market data, account bootstrap and creation, key read and revoke, and billing subscription - a full self-serve account-lifecycle scope set. Second, the MCP resource itself advertises exactly ONE of them: scopes_supported is ["mcp:market.read"] in the protected-resource metadata, and both the docs and llms.txt state twice that "the server advertises mcp:market.read only". So an agent connecting to the hosted MCP today gets read-only market data and nothing else; the remaining
  five scopes exist at the authorization server but are not reachable through the MCP resource. That is a deliberately narrow blast radius for an autonomous client, and it should be described as such rather than as five missing capabilities.'
overview: '0xArchive uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 0xArchive
provider_slug: 0xarchive
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: 0xarchive-scopes
source_filename: 0xarchive-scopes.yml
source_heading: OAuth Scopes
source_url: https://api.0xarchive.io/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://api.0xarchive.io/.well-known/oauth-authorization-server\ndocs: https://docs.0xarchive.io/mcp-server\nsources:\n- https://api.0xarchive.io/.well-known/oauth-authorization-server\n- https://mcp.0xarchive.io/.well-known/oauth-protected-resource\n- https://docs.0xarchive.io/mcp-server\n- https://0xarchive.io/llms.txt\nnote: >-\n  These scopes govern the hosted MCP surface ONLY, not the REST API. The REST API uses an\n  X-API-Key header with no scope model at all - 0-working/derive-oauth-scopes.py correctly found\n  zero oauth2 securitySchemes in the OpenAPI, because there are none. The scopes below are read\n  from the provider's live RFC 8414 authorization-server metadata, which is why this file is\n  method: searched rather than derived.\n  Two facts about this list are worth reading together. First, the authorization server advertises\n  SIX scopes covering market data, account bootstrap and creation, key read and revoke,\
  \ and\n  billing subscription - a full self-serve account-lifecycle scope set. Second, the MCP resource\n  itself advertises exactly ONE of them: scopes_supported is [\"mcp:market.read\"] in the\n  protected-resource metadata, and both the docs and llms.txt state twice that \"the server\n  advertises mcp:market.read only\". So an agent connecting to the hosted MCP today gets read-only\n  market data and nothing else; the remaining five scopes exist at the authorization server but\n  are not reachable through the MCP resource. That is a deliberately narrow blast radius for an\n  autonomous client, and it should be described as such rather than as five missing capabilities.\nissuer: https://auth.0xarchive.io\nauthorization_endpoint: https://auth.0xarchive.io/oauth/authorize\ntoken_endpoint: https://auth.0xarchive.io/oauth/token\nrevocation_endpoint: https://auth.0xarchive.io/oauth/revoke\nregistration_endpoint: https://auth.0xarchive.io/oauth/register\njwks_uri: https://auth.0xarchive.io/.well-known/jwks.json\n\
  grant_types:\n- authorization_code\n- refresh_token\nresponse_types:\n- code\npkce:\n  required_methods:\n  - S256\ntoken_endpoint_auth_methods:\n- none\ndynamic_client_registration: true\nresource: https://mcp.0xarchive.io/mcp\nresource_scopes_supported:\n- mcp:market.read\nscopes:\n- name: mcp:market.read\n  description: >-\n    Read market data through the hosted MCP server - instruments, order books (L2/L3/L4), trades,\n    candles, funding, open interest, liquidations, outcome markets, spot and data-quality routes.\n  reachable_via_mcp: true\n  grants: read\n- name: mcp:account.bootstrap\n  description: Bootstrap an account for a caller that does not yet have one.\n  reachable_via_mcp: false\n  grants: write\n- name: mcp:account.create\n  description: Create a 0xArchive account.\n  reachable_via_mcp: false\n  grants: write\n- name: mcp:keys.read\n  description: List the API keys on the account.\n  reachable_via_mcp: false\n  grants: read\n- name: mcp:keys.revoke\n  description: Revoke\
  \ an API key. Irreversible - see the reversibility block in conventions/.\n  reachable_via_mcp: false\n  grants: write\n- name: mcp:billing.subscribe\n  description: Start a paid subscription. Spends money - see the reversibility block in conventions/.\n  reachable_via_mcp: false\n  grants: write\nservice_documentation: https://0xarchive.io/docs/mcp\nextras:\n  authorization_response_iss_parameter_supported: true\n  note: RFC 9207 issuer identification is enabled, which defends against mix-up attacks on a multi-AS client.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0xarchive/refs/heads/main/scopes/0xarchive-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- market data
- historical data
- crypto
- DeFi
- perpetuals
- derivatives
- order book
- Hyperliquid
- Lighter
- HIP-3
- HIP-4
- prediction markets
- WebSocket
- streaming
- historical replay
- Parquet
- bulk data
- MCP
- agent-native
- x402
- OpenAPI
- REST
token_urls: []
---
