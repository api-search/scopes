---
authorization_urls:
- https://account.jolyn.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Jolynclothing Scopes
name_suffix: OAuth Scopes
note: OAuth/OIDC scopes advertised by the Shopify Customer Account API OIDC discovery document served for the JOLYN store. Captured verbatim from scopes_supported; descriptions per the Shopify Customer Account API documentation.
overview: 'JOLYN publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the JOLYN API on a user''s behalf.


  Tokens are issued from https://account.jolyn.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: JOLYN
provider_slug: jolynclothing
schemes:
- flows:
  - authorizationUrl: https://account.jolyn.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.jolyn.com/authentication/oauth/token
  name: ShopifyCustomerAccount
  source: well-known/jolynclothing-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication — issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven, buyer-authorized commerce.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: jolynclothing-scopes
source_filename: jolynclothing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://jolyn.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  OAuth/OIDC scopes advertised by the Shopify Customer Account API OIDC discovery document\n  served for the JOLYN store. Captured verbatim from scopes_supported; descriptions per the\n  Shopify Customer Account API documentation.\nschemes:\n  - name: ShopifyCustomerAccount\n    source: well-known/jolynclothing-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.jolyn.com/authentication/oauth/authorize\n        tokenUrl: https://account.jolyn.com/authentication/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication — issue an ID token for the customer.\n    flows: [authorizationCode]\n  - scope: email\n    description: Access the customer's email address claim.\n    flows: [authorizationCode]\n  - scope: customer-account-api:full\n\
  \    description: Full access to the Shopify Customer Account API for the authenticated customer (orders, addresses, profile).\n    flows: [authorizationCode]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Customer Account MCP API surface for agent-driven, buyer-authorized commerce.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jolynclothing/refs/heads/main/scopes/jolynclothing-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Swimwear
- Direct-to-Consumer
- Shopify
- Agentic Commerce
token_urls:
- https://account.jolyn.com/authentication/oauth/token
---
