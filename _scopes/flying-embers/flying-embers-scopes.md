---
authorization_urls:
- https://shopify.com/authentication/35263676475/oauth/authorize
description: ''
docs: https://www.flyingembers.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Flying Embers Scopes
name_suffix: OAuth Scopes
note: Derived from the store-scoped OIDC/OAuth 2.0 discovery documents served at the merchant's own domain. The UCP/MCP commerce endpoint itself is anonymous and declares no scopes; these scopes govern customer-account access only.
overview: 'Flying Embers publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flying Embers API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/35263676475/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flying Embers
provider_slug: flying-embers
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/35263676475/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/35263676475/oauth/token
  issuer: https://shopify.com/authentication/35263676475
  name: shopify-customer-accounts-oidc
  source: well-known/flying-embers-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OIDC authentication; issues an ID token identifying the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the signed-in customer's account API (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API — the authenticated agent surface that sits alongside the anonymous UCP shopping MCP endpoint.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: flying-embers-scopes
source_filename: flying-embers-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: https://www.flyingembers.com/.well-known/openid-configuration\ndocs: https://www.flyingembers.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived from the store-scoped OIDC/OAuth 2.0 discovery documents served at the\n  merchant's own domain. The UCP/MCP commerce endpoint itself is anonymous and declares\n  no scopes; these scopes govern customer-account access only.\nschemes:\n  - name: shopify-customer-accounts-oidc\n    source: well-known/flying-embers-openid-configuration.json\n    issuer: https://shopify.com/authentication/35263676475\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/35263676475/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/35263676475/oauth/token\n        pkce: S256\nscopes:\n  - scope: openid\n    description: OIDC authentication; issues an ID token identifying the signed-in customer.\n    flows: [authorizationCode]\n\
  \    sources: [well-known/flying-embers-openid-configuration.json]\n  - scope: email\n    description: Release the customer's email address and email_verified claim.\n    flows: [authorizationCode]\n    sources: [well-known/flying-embers-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the signed-in customer's account API (orders, addresses, profile).\n    flows: [authorizationCode]\n    sources: [well-known/flying-embers-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: >-\n      Full access to the customer-account MCP API — the authenticated agent surface that\n      sits alongside the anonymous UCP shopping MCP endpoint.\n    flows: [authorizationCode]\n    sources: [well-known/flying-embers-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flying-embers/refs/heads/main/scopes/flying-embers-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Beverages
- Consumer Packaged Goods
- Agentic Commerce
- MCP
- Shopify
- Direct to Consumer
token_urls:
- https://shopify.com/authentication/35263676475/oauth/token
---
