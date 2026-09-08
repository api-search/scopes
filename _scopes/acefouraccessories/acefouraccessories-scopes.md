---
authorization_urls:
- https://shopify.com/authentication/67539140858/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Acefouraccessories Scopes
name_suffix: OAuth Scopes
note: There is no OpenAPI in this repo, so derive-oauth-scopes.py has nothing to read. These scopes were read directly from the OIDC discovery document served by the company's own host. They govern the buyer/customer-account plane; the UCP shopping MCP surface is anonymous and consumes no scope.
overview: 'Acefour Accessories publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Acefour Accessories API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/67539140858/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Acefour Accessories
provider_slug: acefouraccessories
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/67539140858/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/67539140858/oauth/token
  issuer: https://shopify.com/authentication/67539140858
  name: shopify-customer-account-oidc
  source: https://uppercase.co.in/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OIDC scope requesting an ID token for the authenticated buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the buyer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Customer Account API for the authenticated buyer of this shop - orders, addresses and profile.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface for the authenticated buyer, the authenticated counterpart to the anonymous UCP shopping MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: acefouraccessories-scopes
source_filename: acefouraccessories-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://uppercase.co.in/.well-known/openid-configuration\nnote: >-\n  There is no OpenAPI in this repo, so derive-oauth-scopes.py has nothing to read. These scopes were\n  read directly from the OIDC discovery document served by the company's own host. They govern the\n  buyer/customer-account plane; the UCP shopping MCP surface is anonymous and consumes no scope.\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: shopify-customer-account-oidc\n  source: https://uppercase.co.in/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/67539140858\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/67539140858/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/67539140858/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated buyer.\n  flows: [authorizationCode]\n\
  \  sources: [https://uppercase.co.in/.well-known/openid-configuration]\n- scope: email\n  description: Releases the buyer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [https://uppercase.co.in/.well-known/openid-configuration]\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Customer Account API for the authenticated buyer of this shop - orders,\n    addresses and profile.\n  flows: [authorizationCode]\n  sources: [https://uppercase.co.in/.well-known/openid-configuration]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP surface for the authenticated buyer, the authenticated\n    counterpart to the anonymous UCP shopping MCP endpoint.\n  flows: [authorizationCode]\n  sources: [https://uppercase.co.in/.well-known/openid-configuration]\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acefouraccessories/refs/heads/main/scopes/acefouraccessories-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Consumer Goods
- Travel
- Luggage
- Direct to Consumer
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- India
token_urls:
- https://shopify.com/authentication/67539140858/oauth/token
---
