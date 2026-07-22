---
authorization_urls:
- https://shopify.com/authentication/69560926386/oauth/authorize
description: ''
docs: https://wanelo.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Wanelo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'wanelo publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the wanelo API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/69560926386/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: wanelo
provider_slug: wanelo
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/69560926386/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/69560926386/oauth/token
  name: shopifyCustomerAccount
  source: well-known/wanelo-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (issue an ID token).
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on the buyer's behalf.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API (agent-driven customer/commerce actions).
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: wanelo-scopes
source_filename: wanelo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://wanelo.com/.well-known/openid-configuration\ndocs: https://wanelo.com/.well-known/openid-configuration\nschemes:\n  - name: shopifyCustomerAccount\n    source: well-known/wanelo-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/69560926386/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/69560926386/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (issue an ID token).\n    flows: [authorizationCode]\n    sources: [well-known/wanelo-openid-configuration.json]\n  - scope: email\n    description: Access the customer's email address and verification status.\n    flows: [authorizationCode]\n    sources: [well-known/wanelo-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on the buyer's behalf.\n    flows:\
  \ [authorizationCode]\n    sources: [well-known/wanelo-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API (agent-driven customer/commerce actions).\n    flows: [authorizationCode]\n    sources: [well-known/wanelo-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wanelo/refs/heads/main/scopes/wanelo-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Shopping
- Ecommerce
- Retail
- Commerce
- Agent Commerce
- MCP
- Shopify
- AI
token_urls:
- https://shopify.com/authentication/69560926386/oauth/token
---
