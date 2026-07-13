---
api_specs:
- filename: leanix-openapi.json
  format: json
  label: LeanIX Integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/openapi/leanix-openapi.json
authorization_urls: []
description: ''
docs: https://help.sap.com/docs/leanix/ea/authentication-to-sap-leanix-services
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Leanix Scopes
name_suffix: OAuth Scopes
note: SAP LeanIX OAuth 2.0 does not use published scopes; the client_credentials token response returns an empty scope value and access is governed by the permission role (Admin, Member, Viewer) of the technical user or API token encoded in the JWT (https://help.sap.com/docs/leanix/ea/authentication-to-sap-leanix-services).
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
  source: openapi/leanix-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: leanix-scopes
source_filename: leanix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leanix-openapi.json\ndocs: https://help.sap.com/docs/leanix/ea/authentication-to-sap-leanix-services\nnote: >-\n  SAP LeanIX OAuth 2.0 does not use published scopes; the client_credentials\n  token response returns an empty scope value and access is governed by the\n  permission role (Admin, Member, Viewer) of the technical user or API token\n  encoded in the JWT\n  (https://help.sap.com/docs/leanix/ea/authentication-to-sap-leanix-services).\nschemes:\n- name: token\n  source: openapi/leanix-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /services/mtm/v1/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanix/refs/heads/main/scopes/leanix-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Enterprise Architecture
- SaaS Management
- IT Portfolio Management
- Application Portfolio
- Technology Risk
token_urls:
- /services/mtm/v1/oauth2/token
---
