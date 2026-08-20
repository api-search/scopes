---
authorization_urls:
- https://shopify.com/authentication/3205202020/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- refreshToken
- jwtBearer
kind: oauth-scopes
layout: scope
method: probed
name: Lemon Perfect Scopes
name_suffix: OAuth Scopes
note: Scopes are taken verbatim from the `scopes_supported` array of the OIDC discovery / RFC 8414 metadata that lemonperfect.com serves for its Shopify Customer Accounts authorization server. No OpenAPI oauth2 securityScheme exists for this provider; nothing here is inferred.
overview: 'Lemon Perfect publishes 4 OAuth 2.0 scopes via the authorizationCode, refreshToken, and jwtBearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lemon Perfect API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/3205202020/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lemon Perfect
provider_slug: lemon-perfect
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/3205202020/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/3205202020/oauth/token
  - flow: refreshToken
    tokenUrl: https://shopify.com/authentication/3205202020/oauth/token
  - flow: jwtBearer
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://shopify.com/authentication/3205202020/oauth/token
  issuer: https://shopify.com/authentication/3205202020
  name: CustomerAccountsOIDC
  source: well-known/lemon-perfect-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect — request an ID token identifying the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Customer Account API on behalf of the signed-in customer (orders, addresses, profile, subscriptions).
  flows:
  - authorizationCode
  - refreshToken
  scope: customer-account-api:full
- description: Full access to the customer account MCP API — the authenticated, customer-scoped counterpart to the store's anonymous UCP/MCP commerce endpoint.
  flows:
  - authorizationCode
  - refreshToken
  scope: customer-account-mcp-api:full
slug: lemon-perfect-scopes
source_filename: lemon-perfect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://lemonperfect.com/.well-known/openid-configuration\nnote: >-\n  Scopes are taken verbatim from the `scopes_supported` array of the OIDC\n  discovery / RFC 8414 metadata that lemonperfect.com serves for its Shopify\n  Customer Accounts authorization server. No OpenAPI oauth2 securityScheme\n  exists for this provider; nothing here is inferred.\nschemes:\n- name: CustomerAccountsOIDC\n  type: openIdConnect\n  source: well-known/lemon-perfect-openid-configuration.json\n  issuer: https://shopify.com/authentication/3205202020\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/3205202020/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/3205202020/oauth/token\n    pkce: S256\n  - flow: refreshToken\n    tokenUrl: https://shopify.com/authentication/3205202020/oauth/token\n  - flow: jwtBearer\n    grant_type: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    tokenUrl:\
  \ https://shopify.com/authentication/3205202020/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect — request an ID token identifying the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/lemon-perfect-openid-configuration.json]\n- scope: email\n  description: Release the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/lemon-perfect-openid-configuration.json]\n- scope: 'customer-account-api:full'\n  description: >-\n    Full access to the Customer Account API on behalf of the signed-in customer\n    (orders, addresses, profile, subscriptions).\n  flows: [authorizationCode, refreshToken]\n  sources: [well-known/lemon-perfect-openid-configuration.json]\n- scope: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the customer account MCP API — the authenticated,\n    customer-scoped counterpart to the store's anonymous UCP/MCP commerce\n    endpoint.\n  flows: [authorizationCode,\
  \ refreshToken]\n  sources: [well-known/lemon-perfect-openid-configuration.json]\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://lemonperfect.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemon-perfect/refs/heads/main/scopes/lemon-perfect-scopes.yml
summary_line: 4 scopes · authorizationCode/refreshToken/jwtBearer
tags:
- Company
- Beverages
- Consumer Packaged Goods
- E-Commerce
- Retail
- Direct to Consumer
- Agentic Commerce
- MCP
- GraphQL
- Universal Commerce Protocol
- Shopify
token_urls:
- https://shopify.com/authentication/3205202020/oauth/token
---
