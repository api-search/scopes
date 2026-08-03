---
authorization_urls:
- https://shopify.com/authentication/85136474359/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Aptera Motors Scopes
name_suffix: OAuth Scopes
note: Aptera Motors publishes no OpenAPI with oauth2 securitySchemes and no scopes reference page. These scopes are the scopes_supported list advertised by the Shopify customer-account authorization server backing https://shop.aptera.us. Descriptions are the standard meanings of these OIDC/Shopify scopes; no scope descriptions are published by the provider.
overview: 'Aptera Motors publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aptera Motors API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/85136474359/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aptera Motors
provider_slug: aptera-motors
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/85136474359/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/85136474359/oauth/token
  issuer: https://shopify.com/authentication/85136474359
  name: shopify-customer-account-oidc
  source: well-known/aptera-motors-shop-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the authenticated customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer of this store.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in customer — the authenticated counterpart of the anonymous storefront MCP server.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: aptera-motors-scopes
source_filename: aptera-motors-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: well-known/aptera-motors-shop-openid-configuration.json\nnote: >-\n  Aptera Motors publishes no OpenAPI with oauth2 securitySchemes and no scopes\n  reference page. These scopes are the scopes_supported list advertised by the\n  Shopify customer-account authorization server backing https://shop.aptera.us.\n  Descriptions are the standard meanings of these OIDC/Shopify scopes; no scope\n  descriptions are published by the provider.\ndocs: null\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/aptera-motors-shop-openid-configuration.json\n  issuer: https://shopify.com/authentication/85136474359\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/85136474359/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/85136474359/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token for the\
  \ authenticated\n    customer.\n  flows: [authorizationCode]\n  sources: [well-known/aptera-motors-shop-openid-configuration.json]\n- scope: email\n  description: Releases the customer's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/aptera-motors-shop-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in\n    customer of this store.\n  flows: [authorizationCode]\n  sources: [well-known/aptera-motors-shop-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the signed-in\n    customer — the authenticated counterpart of the anonymous storefront MCP server.\n  flows: [authorizationCode]\n  sources: [well-known/aptera-motors-shop-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-02'\n  http_status: 200\n  url: https://shop.aptera.us/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptera-motors/refs/heads/main/scopes/aptera-motors-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Automotive
- Electric Vehicles
- Solar
- Manufacturing
- Clean Energy
- Transportation
- Consumer Products
- Mobility
token_urls:
- https://shopify.com/authentication/85136474359/oauth/token
---
