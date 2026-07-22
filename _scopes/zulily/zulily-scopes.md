---
authorization_urls:
- https://account.zulily.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Zulily Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zulily publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zulily API on a user''s behalf.


  Tokens are issued from https://account.zulily.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zulily
provider_slug: zulily
schemes:
- flows:
  - authorizationUrl: https://account.zulily.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.zulily.com/authentication/oauth/token
  name: ShopifyCustomerAccount
  source: well-known/zulily-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication — issue an ID token identifying the customer
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API (orders, addresses, profile) on behalf of the customer
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full agent/MCP access to the customer account surface via the Customer Account MCP API
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: zulily-scopes
source_filename: zulily-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.zulily.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n  - name: ShopifyCustomerAccount\n    source: well-known/zulily-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.zulily.com/authentication/oauth/authorize\n        tokenUrl: https://account.zulily.com/authentication/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication — issue an ID token identifying the customer\n    flows: [authorizationCode]\n    sources: [well-known/zulily-openid-configuration.json]\n  - scope: email\n    description: Access the customer's email address and email_verified claim\n    flows: [authorizationCode]\n    sources: [well-known/zulily-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API (orders, addresses, profile)\
  \ on behalf of the customer\n    flows: [authorizationCode]\n    sources: [well-known/zulily-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full agent/MCP access to the customer account surface via the Customer Account MCP API\n    flows: [authorizationCode]\n    sources: [well-known/zulily-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zulily/refs/heads/main/scopes/zulily-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Ecommerce
- Retail
- Shopping
- Commerce
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
token_urls:
- https://account.zulily.com/authentication/oauth/token
---
