---
authorization_urls:
- https://shopify.com/authentication/3092321/oauth/authorize
description: ''
docs: https://www.ministryofsupply.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Ministry Of Supply Scopes
name_suffix: OAuth Scopes
note: Scopes are read from the merchant's own OpenID Connect discovery document, served from www.ministryofsupply.com. They govern Shopify Customer Accounts (a shopper's own orders and profile), not the anonymous UCP/MCP commerce endpoint — that endpoint has no scope surface and requires no token.
overview: 'Ministry of Supply publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ministry of Supply API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/3092321/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ministry of Supply
provider_slug: ministry-of-supply
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/3092321/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/3092321/oauth/token
  issuer: https://shopify.com/authentication/3092321
  name: shopify-customer-accounts-oidc
  source: well-known/ministry-of-supply-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; issues an ID token for the authenticated shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the shopper's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated shopper.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the authenticated shopper — the account-scoped agent surface, distinct from the anonymous storefront UCP/MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: ministry-of-supply-scopes
source_filename: ministry-of-supply-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://www.ministryofsupply.com/.well-known/openid-configuration\ndocs: https://www.ministryofsupply.com/.well-known/openid-configuration\nnote: >-\n  Scopes are read from the merchant's own OpenID Connect discovery document, served from\n  www.ministryofsupply.com. They govern Shopify Customer Accounts (a shopper's own orders and profile),\n  not the anonymous UCP/MCP commerce endpoint — that endpoint has no scope surface and requires no token.\nschemes:\n- name: shopify-customer-accounts-oidc\n  source: well-known/ministry-of-supply-openid-configuration.json\n  issuer: https://shopify.com/authentication/3092321\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/3092321/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/3092321/oauth/token\nscope_count: 4\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; issues an ID token for the authenticated\
  \ shopper.\n  flows: [authorizationCode]\n  sources: [well-known/ministry-of-supply-openid-configuration.json]\n- scope: email\n  description: Releases the shopper's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/ministry-of-supply-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the authenticated shopper.\n  flows: [authorizationCode]\n  sources: [well-known/ministry-of-supply-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Shopify Customer Account MCP API for the authenticated shopper — the\n    account-scoped agent surface, distinct from the anonymous storefront UCP/MCP endpoint.\n  flows: [authorizationCode]\n  sources: [well-known/ministry-of-supply-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ministry-of-supply/refs/heads/main/scopes/ministry-of-supply-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Apparel
- Retail
- E-Commerce
- Direct To Consumer
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Manufacturing
token_urls:
- https://shopify.com/authentication/3092321/oauth/token
---
