---
authorization_urls:
- https://shopify.com/authentication/14905858/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Super Coffee Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from the storefront's live OIDC/OAuth discovery documents (scopes_supported). No OpenAPI exists for this provider, so nothing here is derived from a spec. The authorization server is Shopify's customer account service for shop id 14905858.
overview: 'Super Coffee publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Super Coffee API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/14905858/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Super Coffee
provider_slug: super-coffee
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/14905858/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/14905858/oauth/token
  issuer: https://shopify.com/authentication/14905858
  name: shopify-customer-account-oauth2
  source: https://www.drinksupercoffee.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer - the authenticated, customer-scoped counterpart to the anonymous UCP commerce MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: super-coffee-scopes
source_filename: super-coffee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://www.drinksupercoffee.com/.well-known/openid-configuration\nnote: >-\n  Scopes are read verbatim from the storefront's live OIDC/OAuth discovery\n  documents (scopes_supported). No OpenAPI exists for this provider, so nothing\n  here is derived from a spec. The authorization server is Shopify's customer\n  account service for shop id 14905858.\nschemes:\n- name: shopify-customer-account-oauth2\n  source: https://www.drinksupercoffee.com/.well-known/oauth-authorization-server\n  issuer: https://shopify.com/authentication/14905858\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/14905858/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/14905858/oauth/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the\n    customer.\n  flows: [authorizationCode]\n  sources: [https://www.drinksupercoffee.com/.well-known/openid-configuration]\n\
  - scope: email\n  description: Releases the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [https://www.drinksupercoffee.com/.well-known/openid-configuration]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in\n    customer (orders, addresses, profile).\n  flows: [authorizationCode]\n  sources: [https://www.drinksupercoffee.com/.well-known/openid-configuration]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API on behalf of the\n    signed-in customer - the authenticated, customer-scoped counterpart to the anonymous\n    UCP commerce MCP endpoint.\n  flows: [authorizationCode]\n  sources: [https://www.drinksupercoffee.com/.well-known/openid-configuration]\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://www.drinksupercoffee.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-coffee/refs/heads/main/scopes/super-coffee-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
token_urls:
- https://shopify.com/authentication/14905858/oauth/token
---
