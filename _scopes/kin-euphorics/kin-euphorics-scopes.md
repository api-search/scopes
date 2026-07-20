---
authorization_urls:
- https://account.kineuphorics.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kin Euphorics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kin Euphorics publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kin Euphorics API on a user''s behalf.


  Tokens are issued from https://account.kineuphorics.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kin Euphorics
provider_slug: kin-euphorics
schemes:
- flows:
  - authorizationUrl: https://account.kineuphorics.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.kineuphorics.com/authentication/oauth/token
  name: shopifyCustomerAccountsOIDC
  source: well-known/kin-euphorics-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated shopper.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven account operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: kin-euphorics-scopes
source_filename: kin-euphorics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.kineuphorics.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: shopifyCustomerAccountsOIDC\n  source: well-known/kin-euphorics-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.kineuphorics.com/authentication/oauth/authorize\n    tokenUrl: https://account.kineuphorics.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/kin-euphorics-openid-configuration.json]\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/kin-euphorics-openid-configuration.json]\n- scope: 'customer-account-api:full'\n  description: Full access to the Shopify Customer Account API for the authenticated shopper.\n\
  \  flows: [authorizationCode]\n  sources: [well-known/kin-euphorics-openid-configuration.json]\n- scope: 'customer-account-mcp-api:full'\n  description: Full access to the Shopify Customer Account MCP API for agent-driven account operations.\n  flows: [authorizationCode]\n  sources: [well-known/kin-euphorics-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kin-euphorics/refs/heads/main/scopes/kin-euphorics-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Beverages
- Non-Alcoholic
- Functional Beverage
- Adaptogens
- Nootropics
- Consumer Packaged Goods
- Ecommerce
- Shopify
- Direct to Consumer
- Agentic Commerce
- UCP
- MCP
token_urls:
- https://account.kineuphorics.com/authentication/oauth/token
---
