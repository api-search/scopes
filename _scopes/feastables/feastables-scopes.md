---
authorization_urls:
- https://shopify.com/authentication/55160602784/oauth/authorize
description: Feastables publishes no OpenAPI and no scopes reference page. These scopes come from the scopes_supported array in the store's own OpenID Connect discovery document, which is served from feastables.com and points at the Shopify hosted authentication issuer for this shop.
docs: https://feastables.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Feastables Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Feastables publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Feastables API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/55160602784/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Feastables
provider_slug: feastables
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/55160602784/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/55160602784/oauth/token
  issuer: https://shopify.com/authentication/55160602784
  name: shopify-customer-account
  source: well-known/feastables-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer - orders, addresses, profile and subscriptions on this store.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface for the authenticated customer. This scope is the only published evidence of an authenticated customer-account MCP server behind the Shopify authentication issuer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: feastables-scopes
source_filename: feastables-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: well-known/feastables-openid-configuration.json\ndocs: https://feastables.com/.well-known/openid-configuration\ndescription: >-\n  Feastables publishes no OpenAPI and no scopes reference page. These scopes come\n  from the scopes_supported array in the store's own OpenID Connect discovery\n  document, which is served from feastables.com and points at the Shopify hosted\n  authentication issuer for this shop.\nschemes:\n  - name: shopify-customer-account\n    source: well-known/feastables-openid-configuration.json\n    issuer: https://shopify.com/authentication/55160602784\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/55160602784/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/55160602784/oauth/token\n        code_challenge_methods: [S256]\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issues an ID token for the customer.\n\
  \    flows: [authorizationCode]\n    sources: [well-known/feastables-openid-configuration.json]\n  - scope: email\n    description: Access to the customer's email address and email_verified claim.\n    flows: [authorizationCode]\n    sources: [well-known/feastables-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: >-\n      Full access to the Shopify Customer Account API for the authenticated\n      customer - orders, addresses, profile and subscriptions on this store.\n    flows: [authorizationCode]\n    sources: [well-known/feastables-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: >-\n      Full access to the customer-account MCP surface for the authenticated\n      customer. This scope is the only published evidence of an authenticated\n      customer-account MCP server behind the Shopify authentication issuer.\n    flows: [authorizationCode]\n    sources: [well-known/feastables-openid-configuration.json]\nnotes:\n\
  \  - >-\n    The UCP Shopping MCP server does not use OAuth scopes - it gates on a\n    UCP-Agent profile URI instead. See authentication/feastables-authentication.yml.\n  - >-\n    Scope descriptions are written from the scope names and the Shopify\n    customer-account model; Feastables publishes no per-scope documentation.\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://feastables.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feastables/refs/heads/main/scopes/feastables-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- Chocolate
- E-Commerce
- Retail
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
token_urls:
- https://shopify.com/authentication/55160602784/oauth/token
---
