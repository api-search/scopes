---
authorization_urls: []
description: ''
docs: https://docs.benchling.com/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Benchling Lims Scopes
name_suffix: OAuth Scopes
note: Benchling's OAuth2 client-credentials flow does not use scopes - app permissions are granted by adding the app as a collaborator to organizations, teams, and projects, so a Bearer token can do anything the app has been granted in the UI (https://docs.benchling.com/docs/authentication).
overview: 'Benchling uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{tenant}.benchling.com/api/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Benchling
provider_slug: benchling-lims
schemes:
- description: Benchling Apps authenticate with OAuth2 client credentials. Exchange client_id/client_secret at POST /api/v2/token for a Bearer access_token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.benchling.com/api/v2/token
  name: appBearerAuth
  source: openapi/benchling-lims-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: benchling-lims-scopes
source_filename: benchling-lims-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/benchling-lims-openapi.yml\ndocs: https://docs.benchling.com/docs/authentication\nnote: Benchling's OAuth2 client-credentials flow does not use scopes - app permissions\n  are granted by adding the app as a collaborator to organizations, teams, and projects,\n  so a Bearer token can do anything the app has been granted in the UI\n  (https://docs.benchling.com/docs/authentication).\nschemes:\n- name: appBearerAuth\n  source: openapi/benchling-lims-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.benchling.com/api/v2/token\n  description: Benchling Apps authenticate with OAuth2 client credentials. Exchange client_id/client_secret\n    at POST /api/v2/token for a Bearer access_token.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchling-lims/refs/heads/main/scopes/benchling-lims-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Life Sciences
- Biotech
- LIMS
- Electronic Lab Notebook
- Registry
- Molecular Biology
- Inventory Management
- Assay Management
- Workflows
- Webhooks
- REST
token_urls:
- https://{tenant}.benchling.com/api/v2/token
---
