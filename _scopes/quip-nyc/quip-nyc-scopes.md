---
authorization_urls:
- https://shopify.com/authentication/57677807690/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Quip Nyc Scopes
name_suffix: OAuth Scopes
note: No OpenAPI exists, so derive-oauth-scopes.py has nothing to read. These scopes are taken verbatim from the scopes_supported array of the live OIDC / RFC 8414 discovery documents served on quip's own host by Shopify Customer Accounts. The scope strings are the provider's; the descriptions are ours.
overview: 'Quip NYC publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Quip NYC API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/57677807690/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Quip NYC
provider_slug: quip-nyc
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/57677807690/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/57677807690/oauth/token
  issuer: https://shopify.com/authentication/57677807690
  name: shopify-customer-accounts
  source: https://www.getquip.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope — requests an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer — orders, addresses, profile, and for quip specifically the refill subscription record.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-scoped MCP API on behalf of the signed-in customer. Distinct from the anonymous UCP shopping MCP endpoint at /api/ucp/mcp, which needs no token.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: quip-nyc-scopes
source_filename: quip-nyc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.getquip.com/.well-known/openid-configuration\nnote: >-\n  No OpenAPI exists, so derive-oauth-scopes.py has nothing to read. These scopes are taken\n  verbatim from the scopes_supported array of the live OIDC / RFC 8414 discovery documents\n  served on quip's own host by Shopify Customer Accounts. The scope strings are the\n  provider's; the descriptions are ours.\nschemes:\n- name: shopify-customer-accounts\n  source: https://www.getquip.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/57677807690\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/57677807690/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/57677807690/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope — requests an ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/quip-nyc-openid-configuration.json]\n\
  - scope: email\n  description: Releases the customer's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/quip-nyc-openid-configuration.json]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API on behalf of the signed-in customer —\n    orders, addresses, profile, and for quip specifically the refill subscription record.\n  flows: [authorizationCode]\n  sources: [well-known/quip-nyc-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-scoped MCP API on behalf of the signed-in customer. Distinct\n    from the anonymous UCP shopping MCP endpoint at /api/ucp/mcp, which needs no token.\n  flows: [authorizationCode]\n  sources: [well-known/quip-nyc-openid-configuration.json]\ncoverage:\n  scopes_total: 4\n  documented_by_provider: false\n  note: >-\n    quip publishes no scopes reference page of its own; the scope list is machine-readable\n\
  \    only, via the discovery document.\nx-evidence:\n- url: https://www.getquip.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quip-nyc/refs/heads/main/scopes/quip-nyc-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Oral Care
- Consumer Health
- Personal Care
- Retail
- E-Commerce
- Direct to Consumer
- Subscription
- Agentic Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/57677807690/oauth/token
---
