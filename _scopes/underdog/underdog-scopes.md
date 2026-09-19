---
authorization_urls:
- https://account.underdog.shop/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Underdog Scopes
name_suffix: OAuth Scopes
note: Scopes advertised in scopes_supported by the authorization server Underdog's storefront names for shopper accounts (Shopify customer accounts, issuer https://shopify.com/authentication/69142905142, endpoints on account.underdog.shop). They govern a signed-in shopper's own account, not a developer programme — Underdog publishes none. Only the four strings the document returns are recorded; descriptions state the scope semantics conservatively.
overview: 'Underdog publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Underdog API on a user''s behalf.


  Tokens are issued from https://account.underdog.shop/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Underdog
provider_slug: underdog
schemes:
- flows:
  - authorizationUrl: https://account.underdog.shop/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.underdog.shop/authentication/oauth/token
  name: shopify-customer-account-oauth2
  source: well-known/underdog-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the shopper's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the signed-in shopper's own customer account data (orders, addresses, profile) through the customer account API.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the signed-in shopper's own customer account data through the customer account MCP transport.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: underdog-scopes
source_filename: underdog-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: https://underdog.shop/.well-known/openid-configuration\nnote: >-\n  Scopes advertised in scopes_supported by the authorization server Underdog's storefront\n  names for shopper accounts (Shopify customer accounts, issuer\n  https://shopify.com/authentication/69142905142, endpoints on account.underdog.shop). They\n  govern a signed-in shopper's own account, not a developer programme — Underdog publishes\n  none. Only the four strings the document returns are recorded; descriptions state the\n  scope semantics conservatively.\nschemes:\n- name: shopify-customer-account-oauth2\n  source: well-known/underdog-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.underdog.shop/authentication/oauth/authorize\n    tokenUrl: https://account.underdog.shop/authentication/oauth/token\nscope_count: 4\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token\
  \ identifying the shopper.\n  flows: [authorizationCode]\n  sources: [well-known/underdog-openid-configuration.json]\n- scope: email\n  description: Releases the shopper's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/underdog-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the signed-in shopper's own customer account data (orders, addresses, profile) through the customer account API.\n  flows: [authorizationCode]\n  sources: [well-known/underdog-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the signed-in shopper's own customer account data through the customer account MCP transport.\n  flows: [authorizationCode]\n  sources: [well-known/underdog-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/underdog/refs/heads/main/scopes/underdog-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Climate Tech
- Circular Economy
- Refurbished Electronics
- Home Appliances
- Retail
- E-Commerce
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- France
token_urls:
- https://account.underdog.shop/authentication/oauth/token
---
