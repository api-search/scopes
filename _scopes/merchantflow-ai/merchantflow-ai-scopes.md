---
api_specs:
- filename: merchantflow-ai-metrics-api-openapi.yml
  format: yaml
  label: MerchantFlow Metrics API
  slug: merchantflow-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-metrics-api-openapi.yml
- filename: merchantflow-ai-orders-api-openapi.yml
  format: yaml
  label: MerchantFlow Orders API
  slug: merchantflow-ai-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-orders-api-openapi.yml
- filename: merchantflow-ai-products-api-openapi.yml
  format: yaml
  label: MerchantFlow Products API
  slug: merchantflow-ai-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-products-api-openapi.yml
- filename: merchantflow-ai-profitability-api-openapi.yml
  format: yaml
  label: MerchantFlow Profitability API
  slug: merchantflow-ai-profitability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-profitability-api-openapi.yml
- filename: merchantflow-ai-store-api-openapi.yml
  format: yaml
  label: MerchantFlow Store API
  slug: merchantflow-ai-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merchantflow-ai/openapi/merchantflow-ai-store-api-openapi.yml
authorization_urls:
- https://merchantflow.ai/api/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: MerchantFlow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MerchantFlow publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MerchantFlow API on a user''s behalf.


  Tokens are issued from https://merchantflow.ai/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MerchantFlow
provider_slug: merchantflow-ai
schemes:
- description: 'OAuth 2.1 authorization code flow with PKCE (S256 required).


    Send the RFC 8707 resource indicator `resource=https://merchantflow.ai/api/v1` at both

    the authorize and token endpoints. If you omit it, MerchantFlow infers it from

    your requested scopes, but sending it explicitly is strongly preferred.


    Request `offline_access` alongside your data scopes to receive a refresh token;

    without it your access token expires after one hour and the merchant has to

    repeat the browser consent flow.'
  flows:
  - authorizationUrl: https://merchantflow.ai/api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://merchantflow.ai/api/auth/oauth2/token
  name: oauth2
  source: openapi/merchantflow-ai-openapi.json
scope_count: 9
scope_names:
- metrics:ad_spend:read
- metrics:contribution_profit:read
- metrics:mer:read
- metrics:revenue:read
- offline_access
- orders:read
- products:read
- profitability:read
- store:read
scopes:
- description: Read the advertising spend total used to calculate MER for a date range
  flows:
  - authorizationCode
  scope: metrics:ad_spend:read
- description: Read your contribution profit total for a date range - the single figure, not the cost breakdown behind it
  flows:
  - authorizationCode
  scope: metrics:contribution_profit:read
- description: Read your Marketing Efficiency Ratio (MER) for a date range - the ratio only, not the underlying figures
  flows:
  - authorizationCode
  scope: metrics:mer:read
- description: Read the revenue total used to calculate MER (D2C gross revenue) for a date range
  flows:
  - authorizationCode
  scope: metrics:revenue:read
- description: Receive a refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: Read your orders and their economics (revenue, COGS, fees, profit). Includes a pseudonymous customer reference so the app can tell repeat buyers from new ones - never names, email addresses, phone numbers, or shipping addresses
  flows:
  - authorizationCode
  scope: orders:read
- description: Read your products, variants, and cost of goods sold
  flows:
  - authorizationCode
  scope: products:read
- description: Read your full profit & loss summary and daily profit history, including COGS, expenses and net profit
  flows:
  - authorizationCode
  scope: profitability:read
- description: Read your store name, currency, timezone, and data freshness
  flows:
  - authorizationCode
  scope: store:read
slug: merchantflow-ai-scopes
source_filename: merchantflow-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/merchantflow-ai-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/merchantflow-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://merchantflow.ai/api/auth/oauth2/authorize\n    tokenUrl: https://merchantflow.ai/api/auth/oauth2/token\n  description: |-\n    OAuth 2.1 authorization code flow with PKCE (S256 required).\n\n    Send the RFC 8707 resource indicator `resource=https://merchantflow.ai/api/v1` at both\n    the authorize and token endpoints. If you omit it, MerchantFlow infers it from\n    your requested scopes, but sending it explicitly is strongly preferred.\n\n    Request `offline_access` alongside your data scopes to receive a refresh token;\n    without it your access token expires after one hour and the merchant has to\n    repeat the browser consent flow.\nscopes:\n- scope: metrics:ad_spend:read\n  description: Read the advertising spend total used to calculate\
  \ MER for a date range\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n- scope: metrics:contribution_profit:read\n  description: Read your contribution profit total for a date range - the single figure, not\n    the cost breakdown behind it\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n- scope: metrics:mer:read\n  description: Read your Marketing Efficiency Ratio (MER) for a date range - the ratio only,\n    not the underlying figures\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n- scope: metrics:revenue:read\n  description: Read the revenue total used to calculate MER (D2C gross revenue) for a date range\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n- scope: offline_access\n  description: Receive a refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n- scope: orders:read\n\
  \  description: Read your orders and their economics (revenue, COGS, fees, profit). Includes\n    a pseudonymous customer reference so the app can tell repeat buyers from new ones - never\n    names, email addresses, phone numbers, or shipping addresses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n- scope: products:read\n  description: Read your products, variants, and cost of goods sold\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n- scope: profitability:read\n  description: Read your full profit & loss summary and daily profit history, including COGS,\n    expenses and net profit\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n- scope: store:read\n  description: Read your store name, currency, timezone, and data freshness\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/merchantflow-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/merchantflow-ai/scopes/merchantflow-ai-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- E-Commerce
- Analytics
- Software-as-a-Service
- Profitability
- Shopify
- WooCommerce
token_bound: false
token_urls:
- https://merchantflow.ai/api/auth/oauth2/token
---
