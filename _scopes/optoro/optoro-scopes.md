---
api_specs:
- filename: optoro-auth-openapi.yml
  format: yaml
  label: Optoro Auth API
  slug: optoro-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-auth-openapi.yml
- filename: optoro-catalogs-openapi.yml
  format: yaml
  label: Optoro Catalogs API
  slug: optoro-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-catalogs-openapi.yml
- filename: optoro-facilities-openapi.yml
  format: yaml
  label: Optoro Facilities API
  slug: optoro-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-facilities-openapi.yml
- filename: optoro-rtv-openapi.yml
  format: yaml
  label: Optoro RTV Vendor API
  slug: optoro-rtv-vendor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-rtv-openapi.yml
- filename: optoro-asn-openapi.yml
  format: yaml
  label: Optoro Inbound ASN API
  slug: optoro-inbound-asn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-asn-openapi.yml
- filename: optoro-external-bin-changes-openapi.yml
  format: yaml
  label: Optoro External Bin Changes API
  slug: optoro-external-bin-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-external-bin-changes-openapi.yml
- filename: optoro-drop-ship-openapi.yml
  format: yaml
  label: Optoro Drop Ship API
  slug: optoro-drop-ship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-drop-ship-openapi.yml
- filename: optoro-returns-portal-orders-openapi.yml
  format: yaml
  label: Optoro Returns Portal Orders API
  slug: optoro-returns-portal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-returns-portal-orders-openapi.yml
- filename: optoro-rmas-openapi.yml
  format: yaml
  label: Optoro Event Webhooks and Customer Endpoints
  slug: optoro-event-webhooks-and-customer-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-rmas-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Optoro Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Optoro uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.optiturn.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Optoro
provider_slug: optoro
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.optiturn.com/oauth/token
  name: oAuth2
  source: openapi/optoro-catalogs-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.optiturn.com/oauth/token
  name: oAuth2
  source: openapi/optoro-drop-ship-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.optiturn.com/oauth/token
  name: oAuth2
  source: openapi/optoro-facilities-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.optiturn.com/oauth/token
  name: oAuth2
  source: openapi/optoro-rtv-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: optoro-scopes
source_filename: optoro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/optoro-catalogs-openapi.yml, openapi/optoro-drop-ship-openapi.yml, openapi/optoro-facilities-openapi.yml,\n  openapi/optoro-rtv-openapi.yml\nschemes:\n- name: oAuth2\n  source: openapi/optoro-catalogs-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.optiturn.com/oauth/token\n- name: oAuth2\n  source: openapi/optoro-drop-ship-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.optiturn.com/oauth/token\n- name: oAuth2\n  source: openapi/optoro-facilities-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.optiturn.com/oauth/token\n- name: oAuth2\n  source: openapi/optoro-rtv-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.optiturn.com/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/scopes/optoro-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Returns Management
- Reverse Logistics
- Retail
- Supply Chain
- eCommerce
- Fulfillment
- Drop Ship
- Inventory
- Webhooks
- Order Management
token_urls:
- https://auth.optiturn.com/oauth/token
---
