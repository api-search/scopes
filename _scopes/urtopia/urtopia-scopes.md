---
authorization_urls:
- https://shopify.com/authentication/58358104213/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Urtopia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Urtopia publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Urtopia API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/58358104213/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Urtopia
provider_slug: urtopia
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/58358104213/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/58358104213/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/urtopia-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: urtopia-scopes
source_filename: urtopia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://newurtopia.com/.well-known/openid-configuration\nnotes: >-\n  Scopes published in the OIDC discovery document served on newurtopia.com.\n  The issuer is Shopify Customer Account authentication\n  (https://shopify.com/authentication/58358104213) — the store's native\n  customer login and Customer Account API/MCP access, not a\n  Urtopia-proprietary OAuth surface.\nschemes:\n  - name: ShopifyCustomerAccountOIDC\n    source: well-known/urtopia-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/58358104213/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/58358104213/oauth/token\n        pkce: S256\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication.\n    flows: [authorizationCode]\n    sources: [well-known/urtopia-openid-configuration.json]\n  - scope: email\n    description: Access to the customer's\
  \ email address claims.\n    flows: [authorizationCode]\n    sources: [well-known/urtopia-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API for the authenticated customer.\n    flows: [authorizationCode]\n    sources: [well-known/urtopia-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API for the authenticated customer.\n    flows: [authorizationCode]\n    sources: [well-known/urtopia-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urtopia/refs/heads/main/scopes/urtopia-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- E-Bikes
- Electric Vehicles
- Cycling
- Smart Hardware
- Mobility
- eCommerce
token_urls:
- https://shopify.com/authentication/58358104213/oauth/token
---
