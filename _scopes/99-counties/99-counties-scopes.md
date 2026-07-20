---
authorization_urls:
- https://account.wallacefarms.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: 99 Counties Scopes
name_suffix: OAuth Scopes
note: ''
overview: '99 Counties publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 99 Counties API on a user''s behalf.


  Tokens are issued from https://account.wallacefarms.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 99 Counties
provider_slug: 99-counties
schemes:
- flows:
  - authorizationUrl: https://account.wallacefarms.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.wallacefarms.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/99-counties-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the customer
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and verification status
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API (orders, addresses, subscriptions, membership)
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for agent-driven account operations
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: 99-counties-scopes
source_filename: 99-counties-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://99counties.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/99-counties-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.wallacefarms.com/authentication/oauth/authorize\n    tokenUrl: https://account.wallacefarms.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the customer\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the customer's email address and verification status\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API (orders, addresses, subscriptions, membership)\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer\
  \ Account MCP API for agent-driven account operations\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99-counties/refs/heads/main/scopes/99-counties-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Agent Commerce
- Regenerative Agriculture
- Food and Beverage
- Shopify
- Model Context Protocol
- Universal Commerce Protocol
token_urls:
- https://account.wallacefarms.com/authentication/oauth/token
---
