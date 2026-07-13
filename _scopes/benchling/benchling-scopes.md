---
api_specs:
- filename: llms.txt
  format: yaml
  label: Benchling REST API
  slug: benchling-rest-api
  spec_type: OpenAPI
  url: https://docs.benchling.com/llms.txt
authorization_urls: []
description: ''
docs: https://docs.benchling.com/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Benchling Scopes
name_suffix: OAuth Scopes
note: Benchling's OAuth 2.0 client credentials flow does not use scopes; API access is governed by the app's or user's permissions (organization, team, and project membership), per https://docs.benchling.com/docs/authentication.
overview: 'Benchling uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Benchling
provider_slug: benchling
schemes:
- description: OAuth2 Client Credentials flow intended for service access
  flows:
  - flow: clientCredentials
    tokenUrl: /api/v2/token
  name: oAuth
  source: openapi/benchling-openapi.yaml
scope_count: 0
scope_names: []
scopes: []
slug: benchling-scopes
source_filename: benchling-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/benchling-openapi.yaml\ndocs: https://docs.benchling.com/docs/authentication\nnote: Benchling's OAuth 2.0 client credentials flow does not use scopes; API access\n  is governed by the app's or user's permissions (organization, team, and project\n  membership), per https://docs.benchling.com/docs/authentication.\nschemes:\n- name: oAuth\n  source: openapi/benchling-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/v2/token\n  description: OAuth2 Client Credentials flow intended for service access\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchling/refs/heads/main/scopes/benchling-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Life Sciences
- Biotech
- R&D
- Molecular Biology
- Laboratory Information Management
- Electronic Lab Notebook
- Assay Management
- Inventory Management
- Sequence Management
- Experiment Workflows
- REST
- Webhooks
token_urls:
- /api/v2/token
---
