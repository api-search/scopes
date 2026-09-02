---
api_specs:
- filename: brooklinen-cart-api-openapi.yml
  format: yaml
  label: Brooklinen Cart API
  slug: brooklinen-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-cart-api-openapi.yml
- filename: brooklinen-collections-api-openapi.yml
  format: yaml
  label: Brooklinen Collections API
  slug: brooklinen-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-collections-api-openapi.yml
- filename: brooklinen-discovery-api-openapi.yml
  format: yaml
  label: Brooklinen Discovery API
  slug: brooklinen-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-discovery-api-openapi.yml
- filename: brooklinen-products-api-openapi.yml
  format: yaml
  label: Brooklinen Products API
  slug: brooklinen-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-products-api-openapi.yml
- filename: brooklinen-search-api-openapi.yml
  format: yaml
  label: Brooklinen Search API
  slug: brooklinen-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/openapi/brooklinen-search-api-openapi.yml
authorization_urls:
- https://account.brooklinen.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Brooklinen Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Brooklinen publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brooklinen API on a user''s behalf.


  Tokens are issued from https://account.brooklinen.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brooklinen
provider_slug: brooklinen
schemes:
- flows:
  - authorizationUrl: https://account.brooklinen.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.brooklinen.com/authentication/oauth/token
  name: shopify-customer-account-oauth2
  source: https://www.brooklinen.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Request an OpenID Connect ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and its verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for this shop — the authenticated customer's profile, addresses, orders, subscriptions and payment methods.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for this shop — the authenticated, customer-scoped agent surface, distinct from the anonymous storefront UCP/MCP endpoint at /api/ucp/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: brooklinen-scopes
source_filename: brooklinen-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://www.brooklinen.com/.well-known/oauth-authorization-server\ndocs: https://shopify.dev/docs/api/customer\nsummary: >-\n  Brooklinen serves RFC 8414 OAuth 2.0 authorization server metadata at its store origin, pointing at the\n  Shopify customer account issuer for shop 9517126 and fronted on account.brooklinen.com. Four scopes are\n  advertised. These govern customer account access — including the Customer Account MCP API — not a developer\n  API program; Brooklinen operates no partner/developer OAuth application surface of its own.\nissuer: https://shopify.com/authentication/9517126\nschemes:\n- name: shopify-customer-account-oauth2\n  source: https://www.brooklinen.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.brooklinen.com/authentication/oauth/authorize\n    tokenUrl: https://account.brooklinen.com/authentication/oauth/token\n    pkce: S256\n\
  scopes:\n- scope: openid\n  description: Request an OpenID Connect ID token identifying the customer.\n  flows: [authorizationCode]\n  sources: [https://www.brooklinen.com/.well-known/oauth-authorization-server]\n- scope: email\n  description: Access the customer's email address and its verification status.\n  flows: [authorizationCode]\n  sources: [https://www.brooklinen.com/.well-known/oauth-authorization-server]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for this shop — the authenticated customer's profile,\n    addresses, orders, subscriptions and payment methods.\n  flows: [authorizationCode]\n  sources: [https://www.brooklinen.com/.well-known/oauth-authorization-server]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API for this shop — the authenticated, customer-scoped agent\n    surface, distinct from the anonymous storefront UCP/MCP endpoint at /api/ucp/mcp.\n\
  \  flows: [authorizationCode]\n  sources: [https://www.brooklinen.com/.well-known/oauth-authorization-server]\nnotes:\n- No scope-by-scope reference page is published by Brooklinen; scope semantics follow Shopify's Customer\n  Account API documentation.\n- The storefront UCP/MCP endpoint at /api/ucp/mcp is gated by agent identity (UCP agent profile), not by\n  OAuth scope. See authentication/brooklinen-authentication.yml.\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://www.brooklinen.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brooklinen/refs/heads/main/scopes/brooklinen-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- E-Commerce
- Retail
- Direct to Consumer
- Home Goods
- Bedding
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- agent-native
- Catalog
- Checkout
token_urls:
- https://account.brooklinen.com/authentication/oauth/token
---
