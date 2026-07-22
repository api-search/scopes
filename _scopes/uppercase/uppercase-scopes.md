---
authorization_urls:
- https://shopify.com/authentication/67539140858/oauth/authorize
description: OAuth scopes advertised by the storefront's authorization server (Shopify customer accounts on uppercase.co.in). Captured verbatim from the scopes_supported claim of the OIDC discovery document; there is no provider-authored scopes reference page beyond this machine-readable surface.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Uppercase Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Uppercase publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Uppercase API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/67539140858/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Uppercase
provider_slug: uppercase
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/67539140858/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/67539140858/oauth/token
  name: shopify-customer-accounts-oauth2
  source: well-known/uppercase-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (id_token issuance).
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API surface for agent-driven commerce.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: uppercase-scopes
source_filename: uppercase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://uppercase.co.in/.well-known/openid-configuration\ndescription: >-\n  OAuth scopes advertised by the storefront's authorization server (Shopify\n  customer accounts on uppercase.co.in). Captured verbatim from the\n  scopes_supported claim of the OIDC discovery document; there is no\n  provider-authored scopes reference page beyond this machine-readable\n  surface.\nschemes:\n  - name: shopify-customer-accounts-oauth2\n    source: well-known/uppercase-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/67539140858/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/67539140858/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (id_token issuance).\n    flows: [authorizationCode]\n    sources: [well-known/uppercase-openid-configuration.json]\n  - scope: email\n    description: Access to\
  \ the customer's email and email_verified claims.\n    flows: [authorizationCode]\n    sources: [well-known/uppercase-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API for the authenticated customer.\n    flows: [authorizationCode]\n    sources: [well-known/uppercase-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the customer-account MCP API surface for agent-driven commerce.\n    flows: [authorizationCode]\n    sources: [well-known/uppercase-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uppercase/refs/heads/main/scopes/uppercase-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Travel
- Luggage
- Backpacks
- Ecommerce
- Retail
- Sustainability
- Agentic Commerce
token_urls:
- https://shopify.com/authentication/67539140858/oauth/token
---
