---
authorization_urls:
- https://shopify.com/authentication/86227812661/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Arlettie Scopes
name_suffix: OAuth Scopes
note: 'There is no OpenAPI to derive scopes from and Arlettie publishes no scopes reference page. This is the verbatim scopes_supported array from the live RFC 8414 authorization-server metadata served by the Les échappées storefront. Descriptions below are labelled by origin: two are OIDC-registered and carry their standard meaning; two are Shopify customer-account scopes whose meaning is inferred from their name and the resource they guard, and are marked as such rather than asserted.'
overview: 'Arlettie publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arlettie API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/86227812661/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arlettie
provider_slug: arlettie
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/86227812661/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/86227812661/oauth/token
  issuer: https://shopify.com/authentication/86227812661
  name: shopify-customer-account-oauth
  source: well-known/arlettie-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Request an OIDC ID token identifying the authenticated customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the authenticated customer's account API surface (orders, addresses, profile) for this shop.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the authenticated customer's account surface through the MCP transport — the customer-scoped counterpart to the anonymous UCP/MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: arlettie-scopes
source_filename: arlettie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://lesechappees.arlettie.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  There is no OpenAPI to derive scopes from and Arlettie publishes no scopes reference page. This is\n  the verbatim scopes_supported array from the live RFC 8414 authorization-server metadata served by\n  the Les échappées storefront. Descriptions below are labelled by origin: two are OIDC-registered\n  and carry their standard meaning; two are Shopify customer-account scopes whose meaning is inferred\n  from their name and the resource they guard, and are marked as such rather than asserted.\n\nschemes:\n- name: shopify-customer-account-oauth\n  issuer: https://shopify.com/authentication/86227812661\n  source: well-known/arlettie-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/86227812661/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/86227812661/oauth/token\n\
  \    code_challenge_methods_supported: [S256]\n\nscopes:\n- scope: openid\n  description: Request an OIDC ID token identifying the authenticated customer.\n  description_origin: oidc-core-registered\n  flows: [authorizationCode]\n  sources: [well-known/arlettie-oauth-authorization-server.json]\n- scope: email\n  description: Release the customer's email and email_verified claims.\n  description_origin: oidc-core-registered\n  flows: [authorizationCode]\n  sources: [well-known/arlettie-oauth-authorization-server.json]\n- scope: customer-account-api:full\n  description: Full access to the authenticated customer's account API surface (orders, addresses,\n    profile) for this shop.\n  description_origin: inferred-from-scope-name\n  flows: [authorizationCode]\n  sources: [well-known/arlettie-oauth-authorization-server.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the authenticated customer's account surface through the MCP transport\n    — the customer-scoped\
  \ counterpart to the anonymous UCP/MCP endpoint.\n  description_origin: inferred-from-scope-name\n  flows: [authorizationCode]\n  sources: [well-known/arlettie-oauth-authorization-server.json]\n  note: >-\n    Notable: this shop advertises an MCP-specific OAuth scope, which is what distinguishes the\n    anonymous agent surface (catalog, cart, checkout) from a customer-authorized one (orders,\n    saved addresses, account history).\n\nsummary:\n  scope_count: 4\n  granularity: coarse\n  note: >-\n    Both non-OIDC scopes are \":full\" — there is no read/write or per-resource split, so a customer\n    authorizing an agent grants the whole account surface or nothing.\n\nx-evidence:\n  fetched: '2026-08-17'\n  url: https://lesechappees.arlettie.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arlettie/refs/heads/main/scopes/arlettie-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Fashion
- Luxury
- Private Sales
- Marketplace
- Shopify
- Agent Commerce
- MCP
- UCP
token_urls:
- https://shopify.com/authentication/86227812661/oauth/token
---
