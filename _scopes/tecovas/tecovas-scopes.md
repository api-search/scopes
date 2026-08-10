---
authorization_urls:
- https://accounts.tecovas.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tecovas Scopes
name_suffix: OAuth Scopes
note: Scopes come from the RFC 8414 authorization-server metadata Tecovas serves from its checkout host for Shopify customer accounts. Tecovas publishes no scope reference page of its own; these are the scopes the issuer advertises as supported. The public read APIs use no scopes.
overview: 'Tecovas publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tecovas API on a user''s behalf.


  Tokens are issued from https://accounts.tecovas.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tecovas
provider_slug: tecovas
schemes:
- flows:
  - authorizationUrl: https://accounts.tecovas.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://accounts.tecovas.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/9910824
  name: shopify-customer-accounts
  source: well-known/tecovas-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect — request an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API — the authenticated agent surface for a signed-in customer (orders, profile, addresses).
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: tecovas-scopes
source_filename: tecovas-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://checkout.tecovas.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes come from the RFC 8414 authorization-server metadata Tecovas serves from its checkout\n  host for Shopify customer accounts. Tecovas publishes no scope reference page of its own;\n  these are the scopes the issuer advertises as supported. The public read APIs use no scopes.\nschemes:\n- name: shopify-customer-accounts\n  issuer: https://shopify.com/authentication/9910824\n  source: well-known/tecovas-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.tecovas.com/authentication/oauth/authorize\n    tokenUrl: https://accounts.tecovas.com/authentication/oauth/token\n    pkce: [S256]\nscopes:\n- scope: openid\n  description: OpenID Connect — request an ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/tecovas-oauth-authorization-server.json]\n\
  - scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/tecovas-oauth-authorization-server.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/tecovas-oauth-authorization-server.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Shopify Customer Account MCP API — the authenticated agent surface for\n    a signed-in customer (orders, profile, addresses).\n  flows: [authorizationCode]\n  sources: [well-known/tecovas-oauth-authorization-server.json]\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://checkout.tecovas.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tecovas/refs/heads/main/scopes/tecovas-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Footwear
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Product Catalog
token_urls:
- https://accounts.tecovas.com/authentication/oauth/token
---
