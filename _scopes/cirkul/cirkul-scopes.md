---
authorization_urls:
- https://shopify.com/authentication/5052170330/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cirkul Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cirkul publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cirkul API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/5052170330/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cirkul
provider_slug: cirkul
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/5052170330/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/5052170330/oauth/token
  issuer: https://shopify.com/authentication/5052170330
  name: shopify-customer-account-oauth2
  source: well-known/cirkul-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the signed-in Cirkul customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the email and email_verified claims for the signed-in customer.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for this shop — the signed-in customer's profile, addresses, orders and subscription plans.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API — the authenticated, customer-scoped counterpart to the anonymous storefront MCP server at /api/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: cirkul-scopes
source_filename: cirkul-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://drinkcirkul.com/.well-known/openid-configuration\nnotes: >-\n  Cirkul publishes no OpenAPI, so these scopes were not derived from a spec. They\n  are the scopes_supported list served verbatim by the OAuth 2.0 / OpenID Connect\n  discovery documents on Cirkul's own host, for the Shopify Customer Account API\n  authorization server bound to Cirkul's shop (5052170330). Descriptions are\n  written from the scope names and the standard OIDC meanings; Cirkul publishes no\n  scope reference page of its own.\nschemes:\n- name: shopify-customer-account-oauth2\n  source: well-known/cirkul-oauth-authorization-server.json\n  issuer: https://shopify.com/authentication/5052170330\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/5052170330/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/5052170330/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard\
  \ OpenID Connect scope; requests an ID token identifying the\n    signed-in Cirkul customer.\n  flows: [authorizationCode]\n  sources: [well-known/cirkul-openid-configuration.json]\n- scope: email\n  description: Releases the email and email_verified claims for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/cirkul-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for this shop — the\n    signed-in customer's profile, addresses, orders and subscription plans.\n  flows: [authorizationCode]\n  sources: [well-known/cirkul-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API — the authenticated,\n    customer-scoped counterpart to the anonymous storefront MCP server at /api/mcp.\n  flows: [authorizationCode]\n  sources: [well-known/cirkul-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://drinkcirkul.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cirkul/refs/heads/main/scopes/cirkul-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Direct to Consumer
- Ecommerce
- Retail
- Subscription Commerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Hydration
token_urls:
- https://shopify.com/authentication/5052170330/oauth/token
---
