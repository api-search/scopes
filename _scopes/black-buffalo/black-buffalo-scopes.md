---
authorization_urls:
- https://shopify.com/authentication/22588521/oauth/authorize
description: Black Buffalo has no OpenAPI to derive scopes from. These are the scopes the authorization server behind Black Buffalo's customer accounts actually advertises in its OIDC / RFC 8414 discovery document (scopes_supported), fetched anonymously on 2026-08-07.
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Black Buffalo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Black Buffalo publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Black Buffalo API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/22588521/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Black Buffalo
provider_slug: black-buffalo
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/22588521/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/22588521/oauth/token
  issuer: https://shopify.com/authentication/22588521
  name: shopify-customer-accounts
  source: well-known/black-buffalo-openid-configuration.json
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
- description: Full access to the Shopify Customer Account API on behalf of the signed-in shopper — orders, addresses and profile for that customer. This is the scope that governs the order history the anonymous Storefront GraphQL schema deliberately does not expose.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the authenticated, per-shopper MCP surface, distinct from the two anonymous MCP servers at /api/mcp and /api/ucp/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: black-buffalo-scopes
source_filename: black-buffalo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://blackbuffalo.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  Black Buffalo has no OpenAPI to derive scopes from. These are the scopes the\n  authorization server behind Black Buffalo's customer accounts actually advertises in\n  its OIDC / RFC 8414 discovery document (scopes_supported), fetched anonymously on\n  2026-08-07.\nschemes:\n- name: shopify-customer-accounts\n  source: well-known/black-buffalo-openid-configuration.json\n  issuer: https://shopify.com/authentication/22588521\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/22588521/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/22588521/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope — issues an ID token identifying the shopper.\n  flows: [authorizationCode]\n  sources: [well-known/black-buffalo-openid-configuration.json]\n\
  - scope: email\n  description: Releases the email and email_verified claims for the authenticated shopper.\n  flows: [authorizationCode]\n  sources: [well-known/black-buffalo-openid-configuration.json]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API on behalf of the signed-in shopper —\n    orders, addresses and profile for that customer. This is the scope that governs the\n    order history the anonymous Storefront GraphQL schema deliberately does not expose.\n  flows: [authorizationCode]\n  sources: [well-known/black-buffalo-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API — the authenticated, per-shopper MCP\n    surface, distinct from the two anonymous MCP servers at /api/mcp and /api/ucp/mcp.\n  flows: [authorizationCode]\n  sources: [well-known/black-buffalo-openid-configuration.json]\nnotes:\n- >-\n  These scopes govern the SHOPPER-delegated\
  \ surface only. The anonymous storefront\n  GraphQL server and BOTH MCP servers require no scope at all — see\n  authentication/black-buffalo-authentication.yml.\n- >-\n  The UCP MCP server's access control is not scope-based: it requires a resolvable agent\n  profile URI in meta[\"ucp-agent\"].profile, which is an identity assertion rather than a\n  delegated permission.\n- >-\n  Black Buffalo publishes no scope reference page of its own; the governing documentation\n  is Shopify's customer-accounts documentation.\nx-evidence:\n  fetched: '2026-08-07'\n  url: https://blackbuffalo.com/.well-known/openid-configuration\n  http_status: 200\n  field: scopes_supported\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-buffalo/refs/heads/main/scopes/black-buffalo-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Packaged Goods
- Nicotine Pouches
- Smokeless Tobacco Alternative
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
token_urls:
- https://shopify.com/authentication/22588521/oauth/token
---
