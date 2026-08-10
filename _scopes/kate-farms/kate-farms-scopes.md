---
authorization_urls:
- https://shopify.com/authentication/2056802/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Kate Farms Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kate Farms publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kate Farms API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/2056802/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kate Farms
provider_slug: kate-farms
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/2056802/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/2056802/oauth/token
  issuer: https://shopify.com/authentication/2056802
  name: CustomerAccountsOIDC
  source: well-known/kate-farms-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OIDC scope; requests an ID token identifying the signed-in Kate Farms shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the shopper's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Customer Account API on behalf of the signed-in shopper — orders, subscriptions, addresses and profile for this store.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the agent-facing projection of the shopper's account, which is what lets an enrolled agent act on a Kate Farms customer's behalf.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: kate-farms-scopes
source_filename: kate-farms-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://shop.katefarms.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: CustomerAccountsOIDC\n  source: well-known/kate-farms-openid-configuration.json\n  issuer: https://shopify.com/authentication/2056802\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/2056802/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/2056802/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OIDC scope; requests an ID token identifying the signed-in\n    Kate Farms shopper.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/kate-farms-openid-configuration.json\n- scope: email\n  description: Releases the shopper's email and email_verified claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/kate-farms-openid-configuration.json\n- scope: 'customer-account-api:full'\n  description: Full\
  \ access to the Customer Account API on behalf of the signed-in\n    shopper — orders, subscriptions, addresses and profile for this store.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/kate-farms-openid-configuration.json\n- scope: 'customer-account-mcp-api:full'\n  description: Full access to the Customer Account MCP API — the agent-facing projection\n    of the shopper's account, which is what lets an enrolled agent act on a Kate Farms\n    customer's behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/kate-farms-openid-configuration.json\nnotes:\n- Only four scopes are advertised, and two of them are coarse \":full\" grants. There\n  is no read-only variant of either the Customer Account API or the Customer Account\n  MCP API on this discovery document, so an agent acting for a shopper is granted\n  the whole account surface or nothing.\n- These are the shopper-identity scopes. Anonymous storefront reads (catalog, collections,\n  search, blog, pages)\
  \ need no scope at all.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://shop.katefarms.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kate-farms/refs/heads/main/scopes/kate-farms-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Nutrition
- Medical Nutrition
- Health
- Food and Beverage
- Consumer Packaged Goods
- E-Commerce
- Agentic Commerce
- Retail
- Shopify
- GraphQL
token_urls:
- https://shopify.com/authentication/2056802/oauth/token
---
