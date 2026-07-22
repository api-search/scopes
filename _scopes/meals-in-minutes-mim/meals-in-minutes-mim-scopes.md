---
authorization_urls:
- https://account.mealsinminutes.co/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Meals In Minutes Mim Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Meals In Minutes, MIM publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Meals In Minutes, MIM API on a user''s behalf.


  Tokens are issued from https://account.mealsinminutes.co/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meals In Minutes, MIM
provider_slug: meals-in-minutes-mim
schemes:
- flows:
  - authorizationUrl: https://account.mealsinminutes.co/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.mealsinminutes.co/authentication/oauth/token
  name: shopify-customer-accounts-oidc
  source: well-known/meals-in-minutes-mim-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — enables agent-driven commerce (UCP MCP) actions on behalf of the authenticated buyer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: meals-in-minutes-mim-scopes
source_filename: meals-in-minutes-mim-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mealsinminutes.co/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: shopify-customer-accounts-oidc\n  source: well-known/meals-in-minutes-mim-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.mealsinminutes.co/authentication/oauth/authorize\n    tokenUrl: https://account.mealsinminutes.co/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the customer's email address claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in buyer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API\
  \ — enables agent-driven commerce\n    (UCP MCP) actions on behalf of the authenticated buyer.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meals-in-minutes-mim/refs/heads/main/scopes/meals-in-minutes-mim-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Food and Beverage
- Meal Delivery
- E-Commerce
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
token_urls:
- https://account.mealsinminutes.co/authentication/oauth/token
---
