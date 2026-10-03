---
api_specs:
- filename: aspiresingapore-public-api-openapi.yml
  format: yaml
  label: Aspiresingapore Public API
  slug: aspiresingapore-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspiresingapore/refs/heads/main/openapi/aspiresingapore-public-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Aspiresingapore Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aspiresingapore uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.aspireapp.com/public/v1/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aspiresingapore
provider_slug: aspiresingapore
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.aspireapp.com/public/v1/login
  name: API_Key_client_credentials
  source: openapi/aspiresingapore-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: aspiresingapore-scopes
source_filename: aspiresingapore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: derived\nsource: openapi/aspiresingapore-openapi-generated.yml\nschemes:\n- name: API_Key_client_credentials\n  source: openapi/aspiresingapore-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.aspireapp.com/public/v1/login\nscopes:\n  - name: none\n    description: No scopes defined\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspiresingapore/refs/heads/main/scopes/aspiresingapore-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Finance
- Banking
- Singapore
- Software-as-a-Service
token_urls:
- https://api.aspireapp.com/public/v1/login
---
