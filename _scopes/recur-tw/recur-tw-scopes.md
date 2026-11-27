---
api_specs:
- filename: recur-tw-checkout-sessions-api-openapi.yml
  format: yaml
  label: Recur Checkout Sessions API
  slug: recur-tw-checkout-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-checkout-sessions-api-openapi.yml
- filename: recur-tw-products-api-openapi.yml
  format: yaml
  label: Recur Products API
  slug: recur-tw-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-products-api-openapi.yml
- filename: recur-tw-subscription-schedules-api-openapi.yml
  format: yaml
  label: Recur Subscription Schedules API
  slug: recur-tw-subscription-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscription-schedules-api-openapi.yml
- filename: recur-tw-subscription-switching-api-openapi.yml
  format: yaml
  label: Recur Subscription Switching API
  slug: recur-tw-subscription-switching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscription-switching-api-openapi.yml
- filename: recur-tw-subscriptions-api-openapi.yml
  format: yaml
  label: Recur Subscriptions API
  slug: recur-tw-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscriptions-api-openapi.yml
authorization_urls:
- https://app.recur.tw/api/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Recur Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Recur publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Recur API on a user''s behalf.


  Tokens are issued from https://app.recur.tw/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Recur
provider_slug: recur-tw
schemes:
- description: 'OAuth 2.1 (Authorization Code + PKCE) for AI agents and MCP clients.

    Used by the Recur MCP server (https://mcp.recur.tw) so agents can request

    least-privilege, scoped access on behalf of a user. Human-facing API

    integrations should use `SecretKey`/`PublishableKey` instead.


    Discovery: https://app.recur.tw/.well-known/openid-configuration'
  flows:
  - authorizationUrl: https://app.recur.tw/api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.recur.tw/api/auth/oauth2/token
  name: OAuth2
  source: openapi/recur-tw-openapi.json
scope_count: 13
scope_names:
- analytics:read
- api-keys:read
- api-keys:write
- customers:read
- email
- integration:verify
- openid
- orders:read
- org:read
- products:read
- products:write
- profile
- subscriptions:read
scopes:
- description: Read revenue analytics (MRR, ARR, churn, LTV).
  flows:
  - authorizationCode
  scope: analytics:read
- description: List and read API keys.
  flows:
  - authorizationCode
  scope: api-keys:read
- description: Create and revoke API keys.
  flows:
  - authorizationCode
  scope: api-keys:write
- description: Read customer records.
  flows:
  - authorizationCode
  scope: customers:read
- description: Read the user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Verify integration and connection status.
  flows:
  - authorizationCode
  scope: integration:verify
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Read orders and payment history.
  flows:
  - authorizationCode
  scope: orders:read
- description: Read organization details.
  flows:
  - authorizationCode
  scope: org:read
- description: Read products and pricing.
  flows:
  - authorizationCode
  scope: products:read
- description: Create and update products.
  flows:
  - authorizationCode
  scope: products:write
- description: Read the user's basic profile.
  flows:
  - authorizationCode
  scope: profile
- description: Read subscriptions and their schedules.
  flows:
  - authorizationCode
  scope: subscriptions:read
slug: recur-tw-scopes
source_filename: recur-tw-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: derived\nsource: openapi/recur-tw-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/recur-tw-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.recur.tw/api/auth/oauth2/authorize\n    tokenUrl: https://app.recur.tw/api/auth/oauth2/token\n  description: |-\n    OAuth 2.1 (Authorization Code + PKCE) for AI agents and MCP clients.\n    Used by the Recur MCP server (https://mcp.recur.tw) so agents can request\n    least-privilege, scoped access on behalf of a user. Human-facing API\n    integrations should use `SecretKey`/`PublishableKey` instead.\n\n    Discovery: https://app.recur.tw/.well-known/openid-configuration\nscopes:\n- scope: analytics:read\n  description: Read revenue analytics (MRR, ARR, churn, LTV).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: api-keys:read\n  description: List and read API keys.\n  flows:\n  - authorizationCode\n  sources:\n \
  \ - openapi/recur-tw-openapi.json\n- scope: api-keys:write\n  description: Create and revoke API keys.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: customers:read\n  description: Read customer records.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: email\n  description: Read the user's email address.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: integration:verify\n  description: Verify integration and connection status.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: openid\n  description: OpenID Connect authentication.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: orders:read\n  description: Read orders and payment history.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: org:read\n  description: Read organization details.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: products:read\n  description: Read products and pricing.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: products:write\n  description: Create and update products.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: profile\n  description: Read the user's basic profile.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n- scope: subscriptions:read\n  description: Read subscriptions and their schedules.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recur-tw-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/recur-tw/scopes/recur-tw-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Subscription
- Payments
- CreatorEconomy
- Taiwan
- SaaS
token_bound: false
token_urls:
- https://app.recur.tw/api/auth/oauth2/token
---
