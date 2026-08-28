---
authorization_urls:
- https://orders.modretro.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Modretro Scopes
name_suffix: OAuth Scopes
note: Derived from the RFC 8414 / OIDC discovery documents ModRetro serves at its own domain — there is no OpenAPI to derive from, and derive-oauth-scopes.py therefore has no input. The scope set is Shopify Customer Accounts scoped to ModRetro's shop (issuer 82920341806); ModRetro publishes no scope reference page of its own.
overview: 'ModRetro publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ModRetro API on a user''s behalf.


  Tokens are issued from https://orders.modretro.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ModRetro
provider_slug: modretro
schemes:
- flows:
  - authorizationUrl: https://orders.modretro.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://orders.modretro.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/modretro-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; issues an ID token for the authenticated customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in ModRetro customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API — the authenticated, customer-scoped agent surface, distinct from the anonymous UCP commerce MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: modretro-scopes
source_filename: modretro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://modretro.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the RFC 8414 / OIDC discovery documents ModRetro serves at its own domain — there is\n  no OpenAPI to derive from, and derive-oauth-scopes.py therefore has no input. The scope set is\n  Shopify Customer Accounts scoped to ModRetro's shop (issuer 82920341806); ModRetro publishes no\n  scope reference page of its own.\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/modretro-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://orders.modretro.com/authentication/oauth/authorize\n        tokenUrl: https://orders.modretro.com/authentication/oauth/token\n        pkce: S256\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope; issues an ID token for the authenticated customer.\n    flows: [authorizationCode]\n    sources: [well-known/modretro-oauth-authorization-server.json]\n\
  \  - scope: email\n    description: Releases the customer's email and email_verified claims.\n    flows: [authorizationCode]\n    sources: [well-known/modretro-oauth-authorization-server.json]\n  - scope: 'customer-account-api:full'\n    description: Full access to the Shopify Customer Account API for the signed-in ModRetro customer (orders, addresses, profile).\n    flows: [authorizationCode]\n    sources: [well-known/modretro-oauth-authorization-server.json]\n  - scope: 'customer-account-mcp-api:full'\n    description: Full access to the Shopify Customer Account MCP API — the authenticated, customer-scoped agent surface, distinct from the anonymous UCP commerce MCP endpoint.\n    flows: [authorizationCode]\n    sources: [well-known/modretro-oauth-authorization-server.json]\nscope_count: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modretro/refs/heads/main/scopes/modretro-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Electronics
- Gaming
- Retro Gaming
- Hardware
- E-Commerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Open Source Hardware
token_urls:
- https://orders.modretro.com/authentication/oauth/token
---
