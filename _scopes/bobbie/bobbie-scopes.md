---
authorization_urls:
- https://account.hibobbie.com/authentication/oauth/authorize
description: Bobbie has no OpenAPI to derive scopes from. These are the scopes the authorization server behind Bobbie's customer accounts actually advertises in its OIDC/RFC 8414 discovery document (scopes_supported), fetched anonymously on 2026-08-02.
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bobbie Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bobbie publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bobbie API on a user''s behalf.


  Tokens are issued from https://account.hibobbie.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bobbie
provider_slug: bobbie
schemes:
- flows:
  - authorizationUrl: https://account.hibobbie.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.hibobbie.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/6622806101
  name: shopify-customer-accounts
  source: well-known/bobbie-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope — issues an ID token identifying the shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the email and email_verified claims for the authenticated shopper.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in shopper — orders, subscriptions, addresses and profile for that customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the authenticated, per-shopper MCP surface, distinct from the anonymous storefront MCP server at /api/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: bobbie-scopes
source_filename: bobbie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://www.hibobbie.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  Bobbie has no OpenAPI to derive scopes from. These are the scopes the authorization\n  server behind Bobbie's customer accounts actually advertises in its OIDC/RFC 8414\n  discovery document (scopes_supported), fetched anonymously on 2026-08-02.\nschemes:\n  - name: shopify-customer-accounts\n    source: well-known/bobbie-openid-configuration.json\n    issuer: https://shopify.com/authentication/6622806101\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.hibobbie.com/authentication/oauth/authorize\n        tokenUrl: https://account.hibobbie.com/authentication/oauth/token\n        pkce: S256\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope — issues an ID token identifying the shopper.\n    flows: [authorizationCode]\n    sources: [well-known/bobbie-openid-configuration.json]\n\
  \  - scope: email\n    description: Releases the email and email_verified claims for the authenticated shopper.\n    flows: [authorizationCode]\n    sources: [well-known/bobbie-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: >-\n      Full access to the Shopify Customer Account API on behalf of the signed-in\n      shopper — orders, subscriptions, addresses and profile for that customer.\n    flows: [authorizationCode]\n    sources: [well-known/bobbie-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: >-\n      Full access to the Customer Account MCP API — the authenticated, per-shopper MCP\n      surface, distinct from the anonymous storefront MCP server at /api/mcp.\n    flows: [authorizationCode]\n    sources: [well-known/bobbie-openid-configuration.json]\nnotes:\n  - >-\n    These scopes govern the SHOPPER-delegated surface only. The anonymous storefront\n    GraphQL and MCP endpoints require no scope at all.\n\
  \  - >-\n    Bobbie publishes no scope reference page of its own; the governing documentation is\n    Shopify's customer-accounts documentation.\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://www.hibobbie.com/.well-known/openid-configuration\n  http_status: 200\n  field: scopes_supported\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bobbie/refs/heads/main/scopes/bobbie-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Packaged Goods
- Infant Formula
- E-Commerce
- Direct to Consumer
- Retail
- Health
- Nutrition
- Agentic Commerce
- Shopify
- GraphQL
- MCP
token_urls:
- https://account.hibobbie.com/authentication/oauth/token
---
