---
authorization_urls: []
description: ''
docs: https://developer.servicetitan.io/docs/oauth20/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Servicetitan Scopes
name_suffix: OAuth Scopes
note: ServiceTitan supports only the OAuth 2.0 client_credentials grant and publishes no OAuth scope strings — access is governed by per-app "API scopes" (View/Modify per API resource) selected in the developer portal and approved by the tenant admin (https://developer.servicetitan.io/docs/oauth20/, https://partnerapis.servicetitan.io/docs/create-and-manage-applications/).
overview: 'ServiceTitan uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.servicetitan.io/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ServiceTitan
provider_slug: servicetitan
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  source: openapi/servicetitan-accounting-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  source: openapi/servicetitan-crm-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  source: openapi/servicetitan-dispatch-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  source: openapi/servicetitan-equipment-systems-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  source: openapi/servicetitan-inventory-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  source: openapi/servicetitan-jpm-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  source: openapi/servicetitan-pricebook-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.servicetitan.io/connect/token
  name: OAuth2
  source: openapi/servicetitan-settings-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: servicetitan-scopes
source_filename: servicetitan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\ndocs: https://developer.servicetitan.io/docs/oauth20/\nnote: ServiceTitan supports only the OAuth 2.0 client_credentials grant and publishes\n  no OAuth scope strings — access is governed by per-app \"API scopes\" (View/Modify\n  per API resource) selected in the developer portal and approved by the tenant admin\n  (https://developer.servicetitan.io/docs/oauth20/, https://partnerapis.servicetitan.io/docs/create-and-manage-applications/).\nsource: openapi/servicetitan-accounting-api-openapi.yml, openapi/servicetitan-crm-api-openapi.yml,\n  openapi/servicetitan-dispatch-api-openapi.yml, openapi/servicetitan-equipment-systems-api-openapi.yml,\n  openapi/servicetitan-inventory-api-openapi.yml, openapi/servicetitan-jpm-api-openapi.yml,\n  openapi/servicetitan-pricebook-api-openapi.yml, openapi/servicetitan-settings-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/servicetitan-accounting-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://auth.servicetitan.io/connect/token\n- name: OAuth2\n  source: openapi/servicetitan-crm-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.servicetitan.io/connect/token\n- name: OAuth2\n  source: openapi/servicetitan-dispatch-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.servicetitan.io/connect/token\n- name: OAuth2\n  source: openapi/servicetitan-equipment-systems-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.servicetitan.io/connect/token\n- name: OAuth2\n  source: openapi/servicetitan-inventory-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.servicetitan.io/connect/token\n- name: OAuth2\n  source: openapi/servicetitan-jpm-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.servicetitan.io/connect/token\n- name: OAuth2\n  source: openapi/servicetitan-pricebook-api-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://auth.servicetitan.io/connect/token\n- name: OAuth2\n  source: openapi/servicetitan-settings-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.servicetitan.io/connect/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicetitan/refs/heads/main/scopes/servicetitan-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Field Service Management
- Trades
- HVAC
- Plumbing
- Electrical
- Construction
- CRM
- Dispatch
- Accounting
- Pricebook
- Marketing
- Memberships
- Webhooks
token_urls:
- https://auth.servicetitan.io/connect/token
---
