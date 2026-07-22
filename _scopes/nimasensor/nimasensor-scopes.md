---
authorization_urls:
- https://account.nimanow.com/authentication/oauth/authorize
description: ''
docs: https://nimanow.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nimasensor Scopes
name_suffix: OAuth Scopes
note: OAuth2/OIDC scopes advertised by Shopify's Customer Account API for the NIMA storefront (scopes_supported in the store's OIDC discovery document). Platform-level, not a first-party NIMA developer API.
overview: 'NimaSensor publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the NimaSensor API on a user''s behalf.


  Tokens are issued from https://account.nimanow.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NimaSensor
provider_slug: nimasensor
schemes:
- flows:
  - authorizationUrl: https://account.nimanow.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.nimanow.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/nimasensor-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication of the storefront customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: nimasensor-scopes
source_filename: nimasensor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nimanow.com/.well-known/openid-configuration\ndocs: https://nimanow.com/.well-known/openid-configuration\nnote: >-\n  OAuth2/OIDC scopes advertised by Shopify's Customer Account API for the NIMA storefront\n  (scopes_supported in the store's OIDC discovery document). Platform-level, not a first-party\n  NIMA developer API.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/nimasensor-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.nimanow.com/authentication/oauth/authorize\n    tokenUrl: https://account.nimanow.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the storefront customer.\n  flows:\n  - authorizationCode\n- scope: email\n  description: Access to the authenticated customer's email address.\n  flows:\n  - authorizationCode\n- scope: customer-account-api:full\n  description: Full\
  \ access to the Shopify Customer Account API for the signed-in customer.\n  flows:\n  - authorizationCode\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the signed-in customer.\n  flows:\n  - authorizationCode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimasensor/refs/heads/main/scopes/nimasensor-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Health
- Consumer Hardware
- Food Safety
- Gluten
- Celiac
- E-Commerce
- IoT
token_urls:
- https://account.nimanow.com/authentication/oauth/token
---
