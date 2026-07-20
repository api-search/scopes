---
authorization_urls:
- https://account.grubblyfarms.com/authentication/oauth/authorize
description: ''
docs: https://account.grubblyfarms.com/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Grubbly Farms Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Grubbly Farms publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Grubbly Farms API on a user''s behalf.


  Tokens are issued from https://account.grubblyfarms.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Grubbly Farms
provider_slug: grubbly-farms
schemes:
- flows:
  - authorizationUrl: https://account.grubblyfarms.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.grubblyfarms.com/authentication/oauth/token
  name: shopify-customer-account-oauth2
  source: well-known/grubbly-farms-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer (orders, addresses, profile, subscriptions).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API, exposing customer-account operations to agents over the Model Context Protocol.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: grubbly-farms-scopes
source_filename: grubbly-farms-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://grubblyfarms.com/.well-known/openid-configuration\ndocs: https://account.grubblyfarms.com/\nschemes:\n- name: shopify-customer-account-oauth2\n  source: well-known/grubbly-farms-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.grubblyfarms.com/authentication/oauth/authorize\n    tokenUrl: https://account.grubblyfarms.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the customer.\n  flows: [authorizationCode]\n  sources: [well-known/grubbly-farms-openid-configuration.json]\n- scope: email\n  description: Access to the authenticated customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/grubbly-farms-openid-configuration.json]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account\
  \ API for the authenticated customer\n    (orders, addresses, profile, subscriptions).\n  flows: [authorizationCode]\n  sources: [well-known/grubbly-farms-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Shopify Customer Account MCP API, exposing customer-account\n    operations to agents over the Model Context Protocol.\n  flows: [authorizationCode]\n  sources: [well-known/grubbly-farms-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubbly-farms/refs/heads/main/scopes/grubbly-farms-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Retail
- Consumer Packaged Goods
- Pet & Animal
- Poultry
- Sustainability
- Shopify
- MCP
- Agentic Commerce
token_urls:
- https://account.grubblyfarms.com/authentication/oauth/token
---
