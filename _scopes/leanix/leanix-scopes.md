---
api_specs:
- filename: leanix-configurations-api-openapi.yml
  format: yaml
  label: LeanIX Configurations API
  slug: leanix-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/openapi/leanix-configurations-api-openapi.yml
- filename: leanix-examples-api-openapi.yml
  format: yaml
  label: LeanIX Examples API
  slug: leanix-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/openapi/leanix-examples-api-openapi.yml
- filename: leanix-fastsynchronizationruns-api-openapi.yml
  format: yaml
  label: LeanIX Fast Synchronization Runs API
  slug: leanix-fastsynchronizationruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/openapi/leanix-fastsynchronizationruns-api-openapi.yml
- filename: leanix-storages-api-openapi.yml
  format: yaml
  label: LeanIX Storages API
  slug: leanix-storages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/openapi/leanix-storages-api-openapi.yml
- filename: leanix-synchronizationruns-api-openapi.yml
  format: yaml
  label: LeanIX Synchronization Runs API
  slug: leanix-synchronizationruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/openapi/leanix-synchronizationruns-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Leanix Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'LeanIX uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /services/mtm/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LeanIX
provider_slug: leanix
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /services/mtm/v1/oauth2/token
  name: token
  source: openapi/leanix-configurations-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /services/mtm/v1/oauth2/token
  name: token
  source: openapi/leanix-examples-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /services/mtm/v1/oauth2/token
  name: token
  source: openapi/leanix-fastsynchronizationruns-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /services/mtm/v1/oauth2/token
  name: token
  source: openapi/leanix-storages-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /services/mtm/v1/oauth2/token
  name: token
  source: openapi/leanix-synchronizationruns-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: leanix-scopes
source_filename: leanix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/leanix-configurations-api-openapi.yml, openapi/leanix-examples-api-openapi.yml,\n  openapi/leanix-fastsynchronizationruns-api-openapi.yml, openapi/leanix-storages-api-openapi.yml,\n  openapi/leanix-synchronizationruns-api-openapi.yml\nschemes:\n- name: token\n  source: openapi/leanix-configurations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /services/mtm/v1/oauth2/token\n- name: token\n  source: openapi/leanix-examples-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /services/mtm/v1/oauth2/token\n- name: token\n  source: openapi/leanix-fastsynchronizationruns-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /services/mtm/v1/oauth2/token\n- name: token\n  source: openapi/leanix-storages-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /services/mtm/v1/oauth2/token\n- name: token\n  source: openapi/leanix-synchronizationruns-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /services/mtm/v1/oauth2/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/scopes/leanix-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Enterprise Architecture
- SaaS Management
- IT Portfolio Management
- Application Portfolio
- Technology Risk
token_bound: false
token_urls:
- /services/mtm/v1/oauth2/token
---
