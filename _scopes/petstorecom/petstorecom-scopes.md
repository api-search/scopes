---
authorization_urls:
- https://shopify.com/authentication/27249049675/oauth/authorize
description: ''
docs: https://petstore.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Petstorecom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Petstore.com publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Petstore.com API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/27249049675/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Petstore.com
provider_slug: petstorecom
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/27249049675/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/27249049675/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/petstorecom-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication — issue an ID token for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the buyer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the agent-facing surface used by UCP/MCP tools acting on the buyer's behalf.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: petstorecom-scopes
source_filename: petstorecom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://petstore.com/.well-known/openid-configuration\ndocs: https://petstore.com/.well-known/openid-configuration\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/petstorecom-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/27249049675/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/27249049675/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication — issue an ID token for the buyer.\n    flows: [authorizationCode]\n    sources: [well-known/petstorecom-openid-configuration.json]\n  - scope: email\n    description: Access the buyer's email address and verification status.\n    flows: [authorizationCode]\n    sources: [well-known/petstorecom-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account\
  \ API for the signed-in buyer.\n    flows: [authorizationCode]\n    sources: [well-known/petstorecom-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: >-\n      Full access to the Customer Account MCP API — the agent-facing surface used\n      by UCP/MCP tools acting on the buyer's behalf.\n    flows: [authorizationCode]\n    sources: [well-known/petstorecom-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petstorecom/refs/heads/main/scopes/petstorecom-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- E-commerce
- Retail
- Pet Supplies
- Agentic Commerce
- UCP
- MCP
- Shopify
token_urls:
- https://shopify.com/authentication/27249049675/oauth/token
---
