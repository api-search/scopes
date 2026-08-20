---
authorization_urls:
- https://shopify.com/authentication/97378959650/oauth/authorize
description: ''
docs: https://coldsnap.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coldsnap Scopes
name_suffix: OAuth Scopes
note: Scopes were read from the live OpenID Connect / RFC 8414 discovery documents served at the ColdSnap origin, not from an OpenAPI oauth2 securityScheme - ColdSnap publishes no OpenAPI.
overview: 'ColdSnap publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ColdSnap API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/97378959650/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ColdSnap
provider_slug: coldsnap
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/97378959650/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/97378959650/oauth/token
  issuer: https://shopify.com/authentication/97378959650
  name: shopify-customer-accounts
  source: https://coldsnap.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Request an OpenID Connect id_token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer - orders, addresses, profile and subscription state for this store.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface on behalf of the signed-in customer. This is the authenticated agent scope; the anonymous storefront MCP server at /api/mcp requires no scope at all.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: coldsnap-scopes
source_filename: coldsnap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://coldsnap.com/.well-known/openid-configuration\ndocs: https://coldsnap.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes were read from the live OpenID Connect / RFC 8414 discovery documents served\n  at the ColdSnap origin, not from an OpenAPI oauth2 securityScheme - ColdSnap publishes\n  no OpenAPI.\nschemes:\n- name: shopify-customer-accounts\n  issuer: https://shopify.com/authentication/97378959650\n  source: https://coldsnap.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/97378959650/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/97378959650/oauth/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: openid\n  description: Request an OpenID Connect id_token identifying the customer.\n  flows: [authorizationCode]\n  sources: ['https://coldsnap.com/.well-known/openid-configuration']\n- scope:\
  \ email\n  description: Release the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: ['https://coldsnap.com/.well-known/openid-configuration']\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API on behalf of the signed-in customer -\n    orders, addresses, profile and subscription state for this store.\n  flows: [authorizationCode]\n  sources: ['https://coldsnap.com/.well-known/openid-configuration']\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP surface on behalf of the signed-in customer.\n    This is the authenticated agent scope; the anonymous storefront MCP server at\n    /api/mcp requires no scope at all.\n  flows: [authorizationCode]\n  sources: ['https://coldsnap.com/.well-known/openid-configuration']\nobserved_in_the_wild:\n- scope_set: 'openid email customer-account-api'\n  where: >-\n    the authorize redirect emitted by\
  \ https://coldsnap.com/customer_authentication/login\n  note: the storefront's own login flow requests the narrower customer-account scope,\n    not the :full variant advertised in discovery.\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://coldsnap.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coldsnap/refs/heads/main/scopes/coldsnap-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Food and Beverage
- Consumer Products
- Hardware
- Appliances
- Food Service
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
token_urls:
- https://shopify.com/authentication/97378959650/oauth/token
---
