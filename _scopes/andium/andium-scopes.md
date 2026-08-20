---
authorization_urls:
- https://shopify.com/authentication/85535392078/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Andium Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Andium publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Andium API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/85535392078/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Andium
provider_slug: andium
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/85535392078/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/85535392078/oauth/token
  issuer: https://shopify.com/authentication/85535392078
  name: shopify-customer-accounts
  source: well-known/andium-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: andium-scopes
source_filename: andium-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://shop.andium.com/.well-known/openid-configuration\nsummary: >-\n  Scopes come from the Shopify Customer Accounts OpenID provider advertised on shop.andium.com.\n  The UCP/MCP shopping endpoint itself is not OAuth-scoped — it is anonymous for reads and gated\n  by buyer approval for payment.\nschemes:\n  - name: shopify-customer-accounts\n    issuer: https://shopify.com/authentication/85535392078\n    source: well-known/andium-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/85535392078/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/85535392078/oauth/token\n        pkce: S256\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issues an ID token for the signed-in customer.\n    flows: [authorizationCode]\n  - scope: email\n    description: Access to the customer's email address claim.\n   \
  \ flows: [authorizationCode]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n    flows: [authorizationCode]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.\n    flows: [authorizationCode]\nx-evidence:\n  - url: https://shop.andium.com/.well-known/openid-configuration\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andium/refs/heads/main/scopes/andium-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Energy
- Oil and Gas
- Industrial IoT
- Remote Monitoring
- Methane Detection
- Emissions
- Computer-Vision
- Edge Computing
- Commerce
- MCP
token_urls:
- https://shopify.com/authentication/85535392078/oauth/token
---
