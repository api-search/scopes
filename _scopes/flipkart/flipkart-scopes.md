---
authorization_urls:
- https://api.flipkart.net/oauth-service/oauth/authorize
description: ''
docs: https://seller.flipkart.com/api-docs/FMSAPI.html
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Flipkart Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flipkart publishes 2 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flipkart API on a user''s behalf.


  Tokens are issued from https://api.flipkart.net/oauth-service/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flipkart
provider_slug: flipkart
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.flipkart.net/oauth-service/oauth/token
  - authorizationUrl: https://api.flipkart.net/oauth-service/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.flipkart.net/oauth-service/oauth/token
  name: OAuth2
  source: https://seller.flipkart.com/api-docs/FMSAPI.html
scope_count: 2
scope_names:
- Seller_Api
- Default
scopes:
- description: Access to the Flipkart Marketplace Seller APIs (listings, orders, shipments, returns, reports).
  flows:
  - clientCredentials
  - authorizationCode
  scope: Seller_Api
- description: Default scope granted for basic authenticated access to the seller platform.
  flows:
  - clientCredentials
  - authorizationCode
  scope: Default
slug: flipkart-scopes
source_filename: flipkart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://seller.flipkart.com/api-docs/FMSAPI.html\ndocs: https://seller.flipkart.com/api-docs/FMSAPI.html\nschemes:\n- name: OAuth2\n  source: https://seller.flipkart.com/api-docs/FMSAPI.html\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flipkart.net/oauth-service/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.flipkart.net/oauth-service/oauth/authorize\n    tokenUrl: https://api.flipkart.net/oauth-service/oauth/token\nscopes:\n- scope: Seller_Api\n  description: Access to the Flipkart Marketplace Seller APIs (listings, orders, shipments, returns, reports).\n  flows:\n  - clientCredentials\n  - authorizationCode\n- scope: Default\n  description: Default scope granted for basic authenticated access to the seller platform.\n  flows:\n  - clientCredentials\n  - authorizationCode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipkart/refs/heads/main/scopes/flipkart-scopes.yml
summary_line: 2 scopes · clientCredentials/authorizationCode
tags:
- Company
- Consumer
- E-Commerce
- Marketplace
- Retail
- Sellers
- Orders
- Fulfillment
- India
- OAuth
token_urls:
- https://api.flipkart.net/oauth-service/oauth/token
---
