---
api_specs:
- filename: arcnm-io-calculations-api-openapi.yml
  format: yaml
  label: ARCNM Calculations API
  slug: arcnm-io-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-calculations-api-openapi.yml
- filename: arcnm-io-calibration-api-openapi.yml
  format: yaml
  label: ARCNM Calibration API
  slug: arcnm-io-calibration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-calibration-api-openapi.yml
- filename: arcnm-io-datasets-api-openapi.yml
  format: yaml
  label: ARCNM Datasets API
  slug: arcnm-io-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-datasets-api-openapi.yml
- filename: arcnm-io-environments-api-openapi.yml
  format: yaml
  label: ARCNM Environments API
  slug: arcnm-io-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-environments-api-openapi.yml
- filename: arcnm-io-folders-api-openapi.yml
  format: yaml
  label: ARCNM Folders API
  slug: arcnm-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-folders-api-openapi.yml
- filename: arcnm-io-geometry-api-openapi.yml
  format: yaml
  label: ARCNM Geometry API
  slug: arcnm-io-geometry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-geometry-api-openapi.yml
- filename: arcnm-io-import-api-openapi.yml
  format: yaml
  label: ARCNM Import API
  slug: arcnm-io-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-import-api-openapi.yml
- filename: arcnm-io-machine-library-api-openapi.yml
  format: yaml
  label: ARCNM Machine Library API
  slug: arcnm-io-machine-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-machine-library-api-openapi.yml
- filename: arcnm-io-machines-api-openapi.yml
  format: yaml
  label: ARCNM Machines API
  slug: arcnm-io-machines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-machines-api-openapi.yml
- filename: arcnm-io-materials-api-openapi.yml
  format: yaml
  label: ARCNM Materials API
  slug: arcnm-io-materials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-materials-api-openapi.yml
- filename: arcnm-io-nesting-api-openapi.yml
  format: yaml
  label: ARCNM Nesting API
  slug: arcnm-io-nesting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-nesting-api-openapi.yml
- filename: arcnm-io-parts-api-openapi.yml
  format: yaml
  label: ARCNM Parts API
  slug: arcnm-io-parts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-parts-api-openapi.yml
- filename: arcnm-io-remnants-api-openapi.yml
  format: yaml
  label: ARCNM Remnants API
  slug: arcnm-io-remnants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-remnants-api-openapi.yml
- filename: arcnm-io-subcontractors-api-openapi.yml
  format: yaml
  label: ARCNM Subcontractors API
  slug: arcnm-io-subcontractors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-subcontractors-api-openapi.yml
- filename: arcnm-io-tools-api-openapi.yml
  format: yaml
  label: ARCNM Tools API
  slug: arcnm-io-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-tools-api-openapi.yml
- filename: arcnm-io-upload-links-api-openapi.yml
  format: yaml
  label: ARCNM Upload Links API
  slug: arcnm-io-upload-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-upload-links-api-openapi.yml
- filename: arcnm-io-uploads-api-openapi.yml
  format: yaml
  label: ARCNM Uploads API
  slug: arcnm-io-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-uploads-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Arcnm Io Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'ARCNM uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/v1/sessions/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ARCNM
provider_slug: arcnm-io
schemes:
- flows:
  - flow: password
    tokenUrl: /api/v1/sessions/login
  name: OAuth2PasswordBearer
  source: openapi/arcnm-io-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: arcnm-io-scopes
source_filename: arcnm-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: none\nsource: openapi/arcnm-io-openapi.yml\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/arcnm-io-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/v1/sessions/login\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/arcnm-io/scopes/arcnm-io-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Manufacturing
- Costing
- CAD
- Engineering
token_bound: false
token_urls:
- /api/v1/sessions/login
---
