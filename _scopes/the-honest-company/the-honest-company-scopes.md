---
authorization_urls:
- https://shopify.com/authentication/64768475320/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: The Honest Company Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'The Honest Company publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Honest Company API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/64768475320/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Honest Company
provider_slug: the-honest-company
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/64768475320/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/64768475320/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/the-honest-company-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: the-honest-company-scopes
source_filename: the-honest-company-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.honest.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  scopes_supported captured verbatim from the live OIDC discovery document at\n  www.honest.com/.well-known/openid-configuration. These are Shopify Customer\n  Account API scopes for the honest.com storefront, not first-party Honest\n  Company API scopes.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/the-honest-company-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/64768475320/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/64768475320/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token identifying the customer.\n  flows: [authorizationCode]\n  sources: [well-known/the-honest-company-openid-configuration.json]\n- scope: email\n  description: Access\
  \ the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/the-honest-company-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/the-honest-company-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/the-honest-company-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-honest-company/refs/heads/main/scopes/the-honest-company-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Consumer Goods
- Ecommerce
- Retail
- Baby
- Personal Care
- Shopify
token_urls:
- https://shopify.com/authentication/64768475320/oauth/token
---
