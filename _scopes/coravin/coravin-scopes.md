---
authorization_urls:
- https://shopify.com/authentication/83805208849/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coravin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Coravin publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coravin API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/83805208849/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coravin
provider_slug: coravin
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/83805208849/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/83805208849/oauth/token
  name: ShopifyCustomerAccounts
  source: well-known/coravin-openid-configuration.json
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
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for agentic-commerce operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: coravin-scopes
source_filename: coravin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.coravin.com/.well-known/openid-configuration\nnotes: >-\n  OAuth 2.0 / OIDC scopes advertised by Coravin's Shopify Customer Accounts\n  authorization server (scopes_supported in the OIDC discovery document).\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n  - name: ShopifyCustomerAccounts\n    source: well-known/coravin-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/83805208849/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/83805208849/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the customer.\n    flows: [authorizationCode]\n    sources: [well-known/coravin-openid-configuration.json]\n  - scope: email\n    description: Access the customer's email address and verification status.\n    flows: [authorizationCode]\n    sources: [well-known/coravin-openid-configuration.json]\n\
  \  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n    flows: [authorizationCode]\n    sources: [well-known/coravin-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Customer Account MCP API for agentic-commerce operations.\n    flows: [authorizationCode]\n    sources: [well-known/coravin-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coravin/refs/heads/main/scopes/coravin-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Wine
- Beverage
- Consumer Products
- Ecommerce
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Wine Preservation
token_urls:
- https://shopify.com/authentication/83805208849/oauth/token
---
