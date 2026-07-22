---
authorization_urls:
- https://shopify.com/authentication/26757464148/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Baublebar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BaubleBar publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BaubleBar API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/26757464148/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BaubleBar
provider_slug: baublebar
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/26757464148/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/26757464148/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/baublebar-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven customer-account interactions.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: baublebar-scopes
source_filename: baublebar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.baublebar.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  OAuth scopes advertised by the shop's Shopify Customer Account API OIDC\n  discovery document (scopes_supported). Transcribed verbatim.\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/baublebar-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/26757464148/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/26757464148/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the signed-in customer.\n    flows: [authorizationCode]\n    sources: [well-known/baublebar-openid-configuration.json]\n  - scope: email\n    description: Access the customer's email address and email_verified claim.\n    flows: [authorizationCode]\n    sources:\
  \ [well-known/baublebar-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile).\n    flows: [authorizationCode]\n    sources: [well-known/baublebar-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API for agent-driven customer-account interactions.\n    flows: [authorizationCode]\n    sources: [well-known/baublebar-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baublebar/refs/heads/main/scopes/baublebar-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Retail
- E-commerce
- Jewelry
- Accessories
- Fashion
- Shopify
- MCP
token_urls:
- https://shopify.com/authentication/26757464148/oauth/token
---
