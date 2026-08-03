---
authorization_urls:
- https://account.beekeepersnaturals.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Beekeepers Naturals Scopes
name_suffix: OAuth Scopes
note: Derived from the live OIDC/OAuth discovery documents served on the store's own host (there is no OpenAPI for this provider). Scope descriptions are the Shopify customer-account meanings of the advertised scope strings; only the four scopes the store actually advertises are listed.
overview: 'Beekeeper''s Naturals publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beekeeper''s Naturals API on a user''s behalf.


  Tokens are issued from https://account.beekeepersnaturals.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beekeeper's Naturals
provider_slug: beekeepers-naturals
schemes:
- flows:
  - authorizationUrl: https://account.beekeepersnaturals.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.beekeepersnaturals.com/authentication/oauth/token
  name: shopify-customer-accounts
  source: well-known/beekeepers-naturals-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Issue an OpenID Connect ID token identifying the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the authenticated customer's account data — profile, addresses, orders and subscriptions — through the Shopify Customer Account API.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the authenticated customer's account through the MCP-shaped customer account surface, for agents acting on the buyer's behalf.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: beekeepers-naturals-scopes
source_filename: beekeepers-naturals-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://www.beekeepersnaturals.com/.well-known/openid-configuration\nnote: 'Derived from the live OIDC/OAuth discovery documents served on the store''s own host (there is no\n  OpenAPI for this provider). Scope descriptions are the Shopify customer-account meanings of the advertised\n  scope strings; only the four scopes the store actually advertises are listed.'\nschemes:\n- name: shopify-customer-accounts\n  source: well-known/beekeepers-naturals-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.beekeepersnaturals.com/authentication/oauth/authorize\n    tokenUrl: https://account.beekeepersnaturals.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Issue an OpenID Connect ID token identifying the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/beekeepers-naturals-openid-configuration.json]\n- scope: email\n\
  \  description: Release the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/beekeepers-naturals-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the authenticated customer's account data — profile, addresses, orders and\n    subscriptions — through the Shopify Customer Account API.\n  flows: [authorizationCode]\n  sources: [well-known/beekeepers-naturals-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the authenticated customer's account through the MCP-shaped customer account\n    surface, for agents acting on the buyer's behalf.\n  flows: [authorizationCode]\n  sources: [well-known/beekeepers-naturals-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://www.beekeepersnaturals.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beekeepers-naturals/refs/heads/main/scopes/beekeepers-naturals-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Consumer Packaged Goods
- Health and Wellness
- Supplements
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
token_urls:
- https://account.beekeepersnaturals.com/authentication/oauth/token
---
