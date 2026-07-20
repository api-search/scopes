---
authorization_urls:
- https://account.everlane.com/authentication/oauth/authorize
description: ''
docs: https://everlane.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Everlane Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'everlane publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the everlane API on a user''s behalf.


  Tokens are issued from https://account.everlane.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: everlane
provider_slug: everlane
schemes:
- flows:
  - authorizationUrl: https://account.everlane.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.everlane.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/everlane-openid-configuration.json
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
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer (orders, profile, addresses).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven customer-account operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: everlane-scopes
source_filename: everlane-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://everlane.com/.well-known/openid-configuration\ndocs: https://everlane.com/.well-known/openid-configuration\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/everlane-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.everlane.com/authentication/oauth/authorize\n    tokenUrl: https://account.everlane.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n  sources: ['well-known/everlane-openid-configuration.json']\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: ['well-known/everlane-openid-configuration.json']\n- scope: 'customer-account-api:full'\n  description: Full access to the Shopify Customer Account API for the authenticated customer (orders,\
  \ profile, addresses).\n  flows: [authorizationCode]\n  sources: ['well-known/everlane-openid-configuration.json']\n- scope: 'customer-account-mcp-api:full'\n  description: Full access to the Shopify Customer Account MCP API for agent-driven customer-account operations.\n  flows: [authorizationCode]\n  sources: ['well-known/everlane-openid-configuration.json']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everlane/refs/heads/main/scopes/everlane-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Fashion
- Direct-to-Consumer
- Shopify
- Agentic Commerce
token_urls:
- https://account.everlane.com/authentication/oauth/token
---
