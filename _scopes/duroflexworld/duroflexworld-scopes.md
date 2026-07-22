---
authorization_urls:
- https://account.duroflexworld.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Duroflexworld Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Duroflexworld publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Duroflexworld API on a user''s behalf.


  Tokens are issued from https://account.duroflexworld.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Duroflexworld
provider_slug: duroflexworld
schemes:
- flows:
  - authorizationUrl: https://account.duroflexworld.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.duroflexworld.com/authentication/oauth/token
  name: shopify-customer-account-oauth2
  source: well-known/duroflexworld-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven customer-account operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: duroflexworld-scopes
source_filename: duroflexworld-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: well-known/duroflexworld-openid-configuration.json\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: shopify-customer-account-oauth2\n  source: well-known/duroflexworld-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.duroflexworld.com/authentication/oauth/authorize\n    tokenUrl: https://account.duroflexworld.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the customer's email address and verification status.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile).\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access\
  \ to the Customer Account MCP API surface for agent-driven customer-account operations.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duroflexworld/refs/heads/main/scopes/duroflexworld-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Ecommerce
- Retail
- Sleep
- Mattresses
- Furniture
- Shopify
- MCP
- Consumer Goods
- India
token_urls:
- https://account.duroflexworld.com/authentication/oauth/token
---
