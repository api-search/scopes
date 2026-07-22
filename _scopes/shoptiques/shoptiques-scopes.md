---
authorization_urls:
- https://account.shoptiques.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Shoptiques Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Shoptiques publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Shoptiques API on a user''s behalf.


  Tokens are issued from https://account.shoptiques.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shoptiques
provider_slug: shoptiques
schemes:
- flows:
  - authorizationUrl: https://account.shoptiques.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.shoptiques.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/shoptiques-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the buyer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven, buyer-authorized actions.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: shoptiques-scopes
source_filename: shoptiques-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://shoptiques.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/shoptiques-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.shoptiques.com/authentication/oauth/authorize\n        tokenUrl: https://account.shoptiques.com/authentication/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the buyer.\n    flows: [authorizationCode]\n    sources: [well-known/shoptiques-openid-configuration.json]\n  - scope: email\n    description: Access to the buyer's email address and verification status.\n    flows: [authorizationCode]\n    sources: [well-known/shoptiques-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of\
  \ the buyer.\n    flows: [authorizationCode]\n    sources: [well-known/shoptiques-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API for agent-driven, buyer-authorized actions.\n    flows: [authorizationCode]\n    sources: [well-known/shoptiques-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoptiques/refs/heads/main/scopes/shoptiques-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Retail
- Marketplace
- Boutiques
- Fashion
- Agentic Commerce
- Shopify
- MCP
- UCP
token_urls:
- https://account.shoptiques.com/authentication/oauth/token
---
