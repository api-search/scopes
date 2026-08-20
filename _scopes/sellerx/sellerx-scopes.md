---
authorization_urls:
- https://mcp.sellerx.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sellerx Scopes
name_suffix: OAuth Scopes
note: Not derived from OpenAPI — SellerX publishes none. These scopes are read verbatim from scopes_supported in the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata served by the SellerX MCP host. SellerX publishes no scopes/permissions reference page, so no description beyond the scope string itself exists publicly. Nothing is inferred.
overview: 'SellerX publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SellerX API on a user''s behalf.


  Tokens are issued from https://mcp.sellerx.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SellerX
provider_slug: sellerx
schemes:
- flows:
  - authorizationUrl: https://mcp.sellerx.com/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.sellerx.com/token
  issuer: https://mcp.sellerx.com/
  name: OAuth2
  source: well-known/sellerx-oauth-authorization-server.json
scope_count: 1
scope_names:
- read
scopes:
- description: Advertised in scopes_supported by both the authorization-server metadata and the protected-resource metadata for https://mcp.sellerx.com/mcp. SellerX publishes no definition of what this scope grants.
  flows:
  - authorizationCode
  scope: read
slug: sellerx-scopes
source_filename: sellerx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://mcp.sellerx.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Not derived from OpenAPI — SellerX publishes none. These scopes are read\n  verbatim from scopes_supported in the RFC 8414 authorization-server metadata\n  and the RFC 9728 protected-resource metadata served by the SellerX MCP host.\n  SellerX publishes no scopes/permissions reference page, so no description\n  beyond the scope string itself exists publicly. Nothing is inferred.\n\nschemes:\n- name: OAuth2\n  source: well-known/sellerx-oauth-authorization-server.json\n  issuer: https://mcp.sellerx.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.sellerx.com/authorize\n    tokenUrl: https://mcp.sellerx.com/token\n\nscopes:\n- scope: read\n  description: >-\n    Advertised in scopes_supported by both the authorization-server metadata and\n    the protected-resource metadata for https://mcp.sellerx.com/mcp. SellerX\n\
  \    publishes no definition of what this scope grants.\n  flows: [authorizationCode]\n  sources:\n  - well-known/sellerx-oauth-authorization-server.json\n  - well-known/sellerx-oauth-protected-resource.json\n\nresources:\n- resource: https://mcp.sellerx.com/mcp\n  authorization_servers: [https://mcp.sellerx.com/]\n  scopes_supported: [read]\n\nx-evidence:\n  fetched: '2026-08-05'\n  probed:\n  - url: https://mcp.sellerx.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.sellerx.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sellerx/refs/heads/main/scopes/sellerx-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- E-Commerce
- Consumer Brands
- Retail
- Amazon Aggregator
- Marketplace-Seller
- Consumer Packaged Goods
- Germany
token_urls:
- https://mcp.sellerx.com/token
---
