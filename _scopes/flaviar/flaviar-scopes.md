---
authorization_urls:
- https://shopify.com/authentication/80863265050/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Flaviar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flaviar publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flaviar API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/80863265050/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flaviar
provider_slug: flaviar
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/80863265050/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/80863265050/oauth/token
  issuer: https://shopify.com/authentication/80863265050
  name: ShopifyCustomerAccount
  source: https://flaviar.com/.well-known/openid-configuration
  type: oauth2
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OIDC authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account GraphQL API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: flaviar-scopes
source_filename: flaviar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://flaviar.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Scopes are advertised by Shopify's Customer Account authorization server\n  (issuer https://shopify.com/authentication/80863265050) for the Flaviar\n  storefront. This is a Shopify-managed OIDC authorization server, not a\n  Flaviar-owned scope registry.\nschemes:\n  - name: ShopifyCustomerAccount\n    type: oauth2\n    source: https://flaviar.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/80863265050\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/80863265050/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/80863265050/oauth/token\n        pkce: S256\nscopes:\n  - scope: openid\n    description: OIDC authentication; issue an ID token for the customer.\n    flows: [authorizationCode]\n  - scope: email\n\
  \    description: Access the customer's email address claim.\n    flows: [authorizationCode]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account GraphQL API on behalf of the signed-in customer.\n    flows: [authorizationCode]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flaviar/refs/heads/main/scopes/flaviar-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Spirits
- Whiskey
- Ecommerce
- Retail
- Beverages
- Subscription
- Agent Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/80863265050/oauth/token
---
