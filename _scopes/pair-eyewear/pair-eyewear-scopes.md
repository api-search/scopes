---
authorization_urls:
- https://shopify.com/authentication/11479910/oauth/authorize
description: ''
docs: https://paireyewear.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Pair Eyewear Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pair Eyewear publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pair Eyewear API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/11479910/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pair Eyewear
provider_slug: pair-eyewear
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/11479910/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/11479910/oauth/token
  name: shopify-customer-accounts-oidc
  source: well-known/pair-eyewear-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token identifying the customer
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's verified email address
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API (agent access to the signed-in customer's account)
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: pair-eyewear-scopes
source_filename: pair-eyewear-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://paireyewear.com/.well-known/openid-configuration\ndocs: https://paireyewear.com/.well-known/oauth-authorization-server\nschemes:\n- name: shopify-customer-accounts-oidc\n  source: well-known/pair-eyewear-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/11479910/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/11479910/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token identifying the customer\n  flows: [authorizationCode]\n  sources: [well-known/pair-eyewear-openid-configuration.json]\n- scope: email\n  description: Access the customer's verified email address\n  flows: [authorizationCode]\n  sources: [well-known/pair-eyewear-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer\n\
  \  flows: [authorizationCode]\n  sources: [well-known/pair-eyewear-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API (agent access to the signed-in customer's account)\n  flows: [authorizationCode]\n  sources: [well-known/pair-eyewear-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pair-eyewear/refs/heads/main/scopes/pair-eyewear-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Eyewear
- Ecommerce
- Retail
- Shopify
- Direct-to-Consumer
- Agent Commerce
- MCP
- UCP
token_urls:
- https://shopify.com/authentication/11479910/oauth/token
---
