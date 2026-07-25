---
api_specs:
- filename: zubale-api-documentation-for-external-notification-handler-api-openapi.yml
  format: yaml
  label: Zubale API Documentation for External Notification Handler API
  slug: zubale-api-documentation-for-external-notification-handler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-api-documentation-for-external-notification-handler-api-openapi.yml
- filename: zubale-cancel-tasks-api-openapi.yml
  format: yaml
  label: Zubale Cancel tasks API
  slug: zubale-cancel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-cancel-tasks-api-openapi.yml
- filename: zubale-delivery-api-api-openapi.yml
  format: yaml
  label: Zubale Delivery API API
  slug: zubale-delivery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-delivery-api-api-openapi.yml
- filename: zubale-external-outbound-api-openapi.yml
  format: yaml
  label: Zubale External outbound API
  slug: zubale-external-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-external-outbound-api-openapi.yml
- filename: zubale-live-tracking-for-cencosud-api-openapi.yml
  format: yaml
  label: Zubale Live Tracking For Cencosud API
  slug: zubale-live-tracking-for-cencosud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-live-tracking-for-cencosud-api-openapi.yml
- filename: zubale-picking-delivery-api-api-openapi.yml
  format: yaml
  label: Zubale Picking & Delivery API API
  slug: zubale-picking-delivery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-picking-delivery-api-api-openapi.yml
- filename: zubale-product-catalog-api-openapi.yml
  format: yaml
  label: Zubale Product catalog API
  slug: zubale-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-product-catalog-api-openapi.yml
- filename: zubale-webhook-payload-structure-for-order-notification-api-openapi.yml
  format: yaml
  label: 'Zubale Webhook: Payload Structure for Order Notification API'
  slug: zubale-webhook-payload-structure-for-order-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-webhook-payload-structure-for-order-notification-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Zubale Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zubale uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.zubale.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zubale
provider_slug: zubale
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.zubale.com/oauth2/token
  name: oauth2
  source: openapi/zubale-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: zubale-scopes
source_filename: zubale-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zubale-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/zubale-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.zubale.com/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/scopes/zubale-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Ecommerce
token_urls:
- https://api.zubale.com/oauth2/token
---
