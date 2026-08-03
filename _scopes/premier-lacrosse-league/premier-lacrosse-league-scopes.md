---
authorization_urls:
- https://account.premierlacrosseleague.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- refreshToken
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: probed
name: Premier Lacrosse League Scopes
name_suffix: OAuth Scopes
note: The Premier Lacrosse League publishes no OAuth documentation. These scopes were read directly from the OAuth 2.0 Authorization Server Metadata (RFC 8414) / OpenID Connect Discovery document served by the league's Shopify-hosted store. They govern customer-account access to the shop, not access to league statistics — the PLL web GraphQL API has no OAuth surface at all.
overview: 'Premier Lacrosse League publishes 4 OAuth 2.0 scopes via the authorizationCode, refreshToken, and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Premier Lacrosse League API on a user''s behalf.


  Tokens are issued from https://account.premierlacrosseleague.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Premier Lacrosse League
provider_slug: premier-lacrosse-league
schemes:
- flows:
  - authorizationUrl: https://account.premierlacrosseleague.com/authentication/oauth/authorize
    endSessionUrl: https://account.premierlacrosseleague.com/authentication/logout
    flow: authorizationCode
    jwksUri: https://account.premierlacrosseleague.com/authentication/.well-known/jwks.json
    pkce:
    - S256
    tokenUrl: https://account.premierlacrosseleague.com/authentication/oauth/token
  - flow: refreshToken
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/8037761076
  name: shop-customer-accounts
  source: well-known/premier-lacrosse-league-shop-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  type: oauth2
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token for the shop customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the authenticated customer's Shopify Customer Account API surface.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API — the authenticated agent-commerce surface behind the store's UCP MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: premier-lacrosse-league-scopes
source_filename: premier-lacrosse-league-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://shop.premierlacrosseleague.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  The Premier Lacrosse League publishes no OAuth documentation. These scopes were read directly\n  from the OAuth 2.0 Authorization Server Metadata (RFC 8414) / OpenID Connect Discovery document\n  served by the league's Shopify-hosted store. They govern customer-account access to the shop,\n  not access to league statistics — the PLL web GraphQL API has no OAuth surface at all.\nschemes:\n- name: shop-customer-accounts\n  type: oauth2\n  issuer: https://shopify.com/authentication/8037761076\n  source: well-known/premier-lacrosse-league-shop-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.premierlacrosseleague.com/authentication/oauth/authorize\n    tokenUrl: https://account.premierlacrosseleague.com/authentication/oauth/token\n    endSessionUrl: https://account.premierlacrosseleague.com/authentication/logout\n\
  \    jwksUri: https://account.premierlacrosseleague.com/authentication/.well-known/jwks.json\n    pkce: [S256]\n  - flow: refreshToken\n  - flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token for the shop customer.\n  flows: [authorizationCode]\n  sources: [well-known/premier-lacrosse-league-shop-oauth-authorization-server.json]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/premier-lacrosse-league-shop-oauth-authorization-server.json]\n- scope: customer-account-api:full\n  description: Full access to the authenticated customer's Shopify Customer Account API surface.\n  flows: [authorizationCode]\n  sources: [well-known/premier-lacrosse-league-shop-oauth-authorization-server.json]\n- scope: customer-account-mcp-api:full\n\
  \  description: >-\n    Full access to the customer-account MCP API — the authenticated agent-commerce surface behind\n    the store's UCP MCP endpoint.\n  flows: [authorizationCode]\n  sources: [well-known/premier-lacrosse-league-shop-oauth-authorization-server.json]\nprotected_resource:\n  resource: https://shop.premierlacrosseleague.com\n  authorization_servers:\n  - https://account.premierlacrosseleague.com\n  - https://shopify.com/authentication/8037761076\n  bearer_methods_supported: [header]\n  source: well-known/premier-lacrosse-league-shop-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://shop.premierlacrosseleague.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/premier-lacrosse-league/refs/heads/main/scopes/premier-lacrosse-league-scopes.yml
summary_line: 4 scopes · authorizationCode/refreshToken/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Company
- Sports
- Lacrosse
- Professional Sports League
- Sports Statistics
- Media and Entertainment
- Ecommerce
- Agent Commerce
- GraphQL
- Fantasy Sports
token_urls:
- https://account.premierlacrosseleague.com/authentication/oauth/token
---
