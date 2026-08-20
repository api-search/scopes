---
authorization_urls:
- https://shopify.com/authentication/31052262/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 100 Thieves Scopes
name_suffix: OAuth Scopes
note: No OpenAPI exists, so derive-oauth-scopes.py found nothing. These scopes are read verbatim from the scopes_supported array of the live OIDC/OAuth discovery documents served on the 100 Thieves host by Shopify Customer Accounts. Descriptions are ours; the scope strings are the provider's.
overview: '100 Thieves publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 100 Thieves API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/31052262/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 100 Thieves
provider_slug: 100-thieves
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/31052262/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/31052262/oauth/token
  issuer: https://shopify.com/authentication/31052262
  name: shopify-customer-accounts
  source: https://100thieves.com/.well-known/openid-configuration
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
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer — orders, addresses, profile.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-scoped MCP API on behalf of the signed-in customer. Distinct from the anonymous UCP shopping MCP endpoint at /api/ucp/mcp, which needs no token.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: 100-thieves-scopes
source_filename: 100-thieves-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://100thieves.com/.well-known/openid-configuration\nnote: >-\n  No OpenAPI exists, so derive-oauth-scopes.py found nothing. These scopes are read\n  verbatim from the scopes_supported array of the live OIDC/OAuth discovery documents\n  served on the 100 Thieves host by Shopify Customer Accounts. Descriptions are ours;\n  the scope strings are the provider's.\nschemes:\n- name: shopify-customer-accounts\n  source: https://100thieves.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/31052262\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/31052262/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/31052262/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope — requests an ID token for the signed-in\n    customer.\n  flows: [authorizationCode]\n  sources: [well-known/100-thieves-openid-configuration.json]\n\
  - scope: email\n  description: Releases the customer's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/100-thieves-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in\n    customer — orders, addresses, profile.\n  flows: [authorizationCode]\n  sources: [well-known/100-thieves-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-scoped MCP API on behalf of the signed-in\n    customer. Distinct from the anonymous UCP shopping MCP endpoint at /api/ucp/mcp,\n    which needs no token.\n  flows: [authorizationCode]\n  sources: [well-known/100-thieves-openid-configuration.json]\ncoverage:\n  scopes_total: 4\n  documented_by_provider: false\n  note: 100 Thieves publishes no scopes reference page of its own; the scope list is\n    machine-readable only, via the discovery document.\nx-evidence:\n- url:\
  \ https://100thieves.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/100-thieves/refs/heads/main/scopes/100-thieves-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Esports
- Gaming
- Apparel
- Retail
- E-Commerce
- Entertainment
- Media
- Direct to Consumer
- Agentic Commerce
token_urls:
- https://shopify.com/authentication/31052262/oauth/token
---
