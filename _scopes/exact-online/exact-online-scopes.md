---
api_specs:
- filename: exact-online-crm-api-openapi.yml
  format: yaml
  label: Exact Online CRM API
  slug: exact-online-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/openapi/exact-online-crm-api-openapi.yml
- filename: exact-online-financial-api-openapi.yml
  format: yaml
  label: Exact Online Financial API
  slug: exact-online-financial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/openapi/exact-online-financial-api-openapi.yml
- filename: exact-online-logistics-api-openapi.yml
  format: yaml
  label: Exact Online Logistics API
  slug: exact-online-logistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/openapi/exact-online-logistics-api-openapi.yml
- filename: exact-online-purchase-api-openapi.yml
  format: yaml
  label: Exact Online Purchase API
  slug: exact-online-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/openapi/exact-online-purchase-api-openapi.yml
- filename: exact-online-sales-api-openapi.yml
  format: yaml
  label: Exact Online Sales API
  slug: exact-online-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/openapi/exact-online-sales-api-openapi.yml
- filename: exact-online-system-api-openapi.yml
  format: yaml
  label: Exact Online System API
  slug: exact-online-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/openapi/exact-online-system-api-openapi.yml
authorization_urls:
- https://start.exactonline.nl/api/oauth2/auth
description: ''
docs: https://support.exactonline.com/community/s/article/All-All-DNO-Content-oauth-eol-oauth-devstep2?language=en_GB
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Exact Online Scopes
name_suffix: OAuth Scopes
note: Exact Online's OAuth 2.0 authorization code flow does not use a scope parameter (documented request parameters are client_id, redirect_uri, response_type, and force_login); access levels are instead configured per resource (None/Read/Manage) in the Exact App Center Data & Security Review and consented per division by the user (https://support.exactonline.com/community/s/article/All-All-DNO-Content-oauth-eol-oauth-devstep2?language=en_GB).
overview: 'Exact Online uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://start.exactonline.nl/api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Exact Online
provider_slug: exact-online
schemes:
- flows:
  - authorizationUrl: https://start.exactonline.nl/api/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://start.exactonline.nl/api/oauth2/token
  name: oauth2
  source: openapi/exact-online-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: exact-online-scopes
source_filename: exact-online-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/exact-online-openapi.yml\ndocs: https://support.exactonline.com/community/s/article/All-All-DNO-Content-oauth-eol-oauth-devstep2?language=en_GB\nnote: >-\n  Exact Online's OAuth 2.0 authorization code flow does not use a scope\n  parameter (documented request parameters are client_id, redirect_uri,\n  response_type, and force_login); access levels are instead configured per\n  resource (None/Read/Manage) in the Exact App Center Data & Security Review\n  and consented per division by the user\n  (https://support.exactonline.com/community/s/article/All-All-DNO-Content-oauth-eol-oauth-devstep2?language=en_GB).\nschemes:\n- name: oauth2\n  source: openapi/exact-online-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://start.exactonline.nl/api/oauth2/auth\n    tokenUrl: https://start.exactonline.nl/api/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/scopes/exact-online-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Accounting
- ERP
- Invoicing
- Business Software
- CRM
- Financial Software
- SME
token_urls:
- https://start.exactonline.nl/api/oauth2/token
---
