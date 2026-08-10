---
authorization_urls:
- https://shopify.com/authentication/54359195821/oauth/authorize
description: Fnatic has no OpenAPI to derive scopes from. These are the scopes the authorization server behind the Fnatic Shop's customer accounts actually advertises in its OIDC / RFC 8414 discovery documents (scopes_supported), fetched anonymously on 2026-08-04. Fnatic publishes no scope reference page of its own.
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Fnatic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fnatic publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fnatic API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/54359195821/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fnatic
provider_slug: fnatic
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/54359195821/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/54359195821/oauth/token
  issuer: https://shopify.com/authentication/54359195821
  name: shopify-customer-accounts
  source: well-known/fnatic-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope — issues an ID token identifying the shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the email and email_verified claims for the authenticated shopper.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in shopper — orders, addresses and profile for that customer of the Fnatic Shop.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the authenticated, per-shopper MCP surface. Distinct from the store-level UCP MCP endpoint at /api/ucp/mcp, which is gated on an agent profile rather than a shopper scope.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: fnatic-scopes
source_filename: fnatic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://shop.fnatic.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  Fnatic has no OpenAPI to derive scopes from. These are the scopes the authorization\n  server behind the Fnatic Shop's customer accounts actually advertises in its OIDC /\n  RFC 8414 discovery documents (scopes_supported), fetched anonymously on 2026-08-04.\n  Fnatic publishes no scope reference page of its own.\nschemes:\n  - name: shopify-customer-accounts\n    source: well-known/fnatic-openid-configuration.json\n    issuer: https://shopify.com/authentication/54359195821\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/54359195821/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/54359195821/oauth/token\n        pkce: S256\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope — issues an ID token identifying\
  \ the shopper.\n    flows: [authorizationCode]\n    sources: [well-known/fnatic-openid-configuration.json]\n  - scope: email\n    description: Releases the email and email_verified claims for the authenticated shopper.\n    flows: [authorizationCode]\n    sources: [well-known/fnatic-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: >-\n      Full access to the Shopify Customer Account API on behalf of the signed-in\n      shopper — orders, addresses and profile for that customer of the Fnatic Shop.\n    flows: [authorizationCode]\n    sources: [well-known/fnatic-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: >-\n      Full access to the Customer Account MCP API — the authenticated, per-shopper MCP\n      surface. Distinct from the store-level UCP MCP endpoint at /api/ucp/mcp, which is\n      gated on an agent profile rather than a shopper scope.\n    flows: [authorizationCode]\n    sources: [well-known/fnatic-openid-configuration.json]\n\
  notes:\n  - >-\n    These scopes govern the SHOPPER-delegated surface only. The anonymous Storefront\n    GraphQL endpoint requires no scope at all — full introspection and catalog reads\n    succeed unauthenticated.\n  - >-\n    Fnatic's own member accounts on fnatic.com (Fnatic ID) publish no scopes and no\n    OAuth/OIDC discovery document.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://shop.fnatic.com/.well-known/openid-configuration\n  http_status: 200\n  field: scopes_supported\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fnatic/refs/heads/main/scopes/fnatic-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Esports
- Gaming
- Entertainment
- Sports
- Consumer Electronics
- Gaming Hardware
- Apparel
- Ecommerce
- Direct to Consumer
- Agentic Commerce
- Shopify
- GraphQL
- Universal Commerce Protocol
- Model Context Protocol
- United Kingdom
token_urls:
- https://shopify.com/authentication/54359195821/oauth/token
---
