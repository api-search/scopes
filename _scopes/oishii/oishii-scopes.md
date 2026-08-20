---
authorization_urls:
- https://shopify.com/authentication/26346881082/oauth/authorize
description: ''
docs: https://oishii.com/.well-known/openid-configuration
flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: Oishii Scopes
name_suffix: OAuth Scopes
note: Scopes are declared by the Shopify customer-account authorization server that oishii.com delegates identity to. Oishii publishes no OpenAPI, so these are read verbatim from the RFC 8414 / OIDC discovery documents served on the oishii.com host — not derived from a spec. The two customer-account scopes are coarse-grained (":full"); there is no per-resource scope surface.
overview: 'Oishii publishes 4 OAuth 2.0 scopes via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Oishii API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/26346881082/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oishii
provider_slug: oishii
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/26346881082/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/26346881082/oauth/token
  - flow: refreshToken
    tokenUrl: https://shopify.com/authentication/26346881082/oauth/token
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://shopify.com/authentication/26346881082/oauth/token
  issuer: https://shopify.com/authentication/26346881082
  name: shopify-customer-account
  source: well-known/oishii-oauth-authorization-server.json
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
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API on behalf of the signed-in customer — the authenticated agent surface complementing the anonymous storefront MCP server.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: oishii-scopes
source_filename: oishii-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://oishii.com/.well-known/oauth-authorization-server\ndocs: https://oishii.com/.well-known/openid-configuration\nnote: >-\n  Scopes are declared by the Shopify customer-account authorization server that oishii.com delegates\n  identity to. Oishii publishes no OpenAPI, so these are read verbatim from the RFC 8414 / OIDC discovery\n  documents served on the oishii.com host — not derived from a spec. The two customer-account scopes are\n  coarse-grained (\":full\"); there is no per-resource scope surface.\nschemes:\n- name: shopify-customer-account\n  source: well-known/oishii-oauth-authorization-server.json\n  issuer: https://shopify.com/authentication/26346881082\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/26346881082/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/26346881082/oauth/token\n    pkce: S256\n  - flow: refreshToken\n    tokenUrl: https://shopify.com/authentication/26346881082/oauth/token\n\
  \  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer\n    tokenUrl: https://shopify.com/authentication/26346881082/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/oishii-openid-configuration.json]\n- scope: email\n  description: Release the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/oishii-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile).\n  flows: [authorizationCode]\n  sources: [well-known/oishii-oauth-authorization-server.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API on behalf of the signed-in customer — the authenticated agent surface complementing the anonymous storefront MCP server.\n\
  \  flows: [authorizationCode]\n  sources: [well-known/oishii-oauth-authorization-server.json]\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://oishii.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oishii/refs/heads/main/scopes/oishii-scopes.yml
summary_line: 4 scopes · authorizationCode/refreshToken/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Company
- Agriculture
- Vertical Farming
- Food and Beverage
- Consumer Products
- E-Commerce
- Retail
- Agent Commerce
- Shopify
- MCP
- Universal Commerce Protocol
token_urls:
- https://shopify.com/authentication/26346881082/oauth/token
---
