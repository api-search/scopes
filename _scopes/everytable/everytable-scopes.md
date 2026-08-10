---
authorization_urls:
- https://account.everytable.com/authentication/oauth/authorize
description: ''
docs: https://everytable.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Everytable Scopes
name_suffix: OAuth Scopes
note: Derived from the live authorization-server metadata Everytable's storefront serves anonymously (scopes_supported), not from an OpenAPI securityScheme — Everytable publishes no OpenAPI. Scope descriptions are the standard OIDC meanings; Everytable publishes no scope reference page of its own.
overview: 'Everytable publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Everytable API on a user''s behalf.


  Tokens are issued from https://account.everytable.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Everytable
provider_slug: everytable
schemes:
- flows:
  - authorizationUrl: https://account.everytable.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.everytable.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/69951324217
  name: ShopifyCustomerAccountOIDC
  source: well-known/everytable-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Request an OpenID Connect ID token identifying the signed-in Everytable customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in Everytable customer — orders, addresses, subscriptions and profile.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-scoped MCP API on behalf of the signed-in customer — the buyer-authenticated counterpart to the anonymous UCP/MCP commerce endpoint at /api/ucp/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: everytable-scopes
source_filename: everytable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://everytable.com/.well-known/oauth-authorization-server\ndocs: https://everytable.com/.well-known/openid-configuration\nnote: Derived from the live authorization-server metadata Everytable's storefront serves\n  anonymously (scopes_supported), not from an OpenAPI securityScheme — Everytable publishes\n  no OpenAPI. Scope descriptions are the standard OIDC meanings; Everytable publishes\n  no scope reference page of its own.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/everytable-oauth-authorization-server.json\n  issuer: https://shopify.com/authentication/69951324217\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.everytable.com/authentication/oauth/authorize\n    tokenUrl: https://account.everytable.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token identifying the signed-in Everytable\n    customer.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - well-known/everytable-oauth-authorization-server.json\n- scope: email\n  description: Release the customer's email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/everytable-oauth-authorization-server.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in\n    Everytable customer — orders, addresses, subscriptions and profile.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/everytable-oauth-authorization-server.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-scoped MCP API on behalf of the signed-in\n    customer — the buyer-authenticated counterpart to the anonymous UCP/MCP commerce\n    endpoint at /api/ucp/mcp.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/everytable-oauth-authorization-server.json\nx-evidence:\n  fetched: '2026-08-04'\n  url:\
  \ https://everytable.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everytable/refs/heads/main/scopes/everytable-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Food
- Restaurants
- Meal Delivery
- Ecommerce
- Agentic Commerce
- Shopify
- Social Enterprise
- Nutrition
- Subscriptions
token_urls:
- https://account.everytable.com/authentication/oauth/token
---
