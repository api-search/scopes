---
authorization_urls:
- https://account.daily-harvest.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Daily Harvest Scopes
name_suffix: OAuth Scopes
note: scopes_supported taken verbatim from the live OIDC discovery document served on the provider host. These are Shopify Customer Account API scopes for account.daily-harvest.com (issuer https://shopify.com/authentication/73275670826).
overview: 'Daily Harvest publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Daily Harvest API on a user''s behalf.


  Tokens are issued from https://account.daily-harvest.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Daily Harvest
provider_slug: daily-harvest
schemes:
- flows:
  - authorizationUrl: https://account.daily-harvest.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.daily-harvest.com/authentication/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/daily-harvest-openid-configuration.json
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
- description: Full access to the Shopify Customer Account API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: daily-harvest-scopes
source_filename: daily-harvest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://daily-harvest.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  scopes_supported taken verbatim from the live OIDC discovery document served\n  on the provider host. These are Shopify Customer Account API scopes for\n  account.daily-harvest.com (issuer https://shopify.com/authentication/73275670826).\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/daily-harvest-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.daily-harvest.com/authentication/oauth/authorize\n    tokenUrl: https://account.daily-harvest.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/daily-harvest-openid-configuration.json]\n- scope: email\n  description: Access the customer's email address\
  \ and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/daily-harvest-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/daily-harvest-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the authenticated customer.\n  flows: [authorizationCode]\n  sources: [well-known/daily-harvest-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daily-harvest/refs/heads/main/scopes/daily-harvest-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Food & Beverage
- Direct-to-Consumer
- E-commerce
- Food Delivery
- Health & Wellness
- Subscription
- Shopify
token_urls:
- https://account.daily-harvest.com/authentication/oauth/token
---
