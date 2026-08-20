---
api_specs:
- filename: fossology-admin-api-openapi.yml
  format: yaml
  label: FOSSology Admin API
  slug: fossology-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-admin-api-openapi.yml
- filename: fossology-auth-api-openapi.yml
  format: yaml
  label: FOSSology auth API
  slug: fossology-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-auth-api-openapi.yml
- filename: fossology-copyrights-api-openapi.yml
  format: yaml
  label: FOSSology Copyrights API
  slug: fossology-copyrights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-copyrights-api-openapi.yml
- filename: fossology-folders-api-openapi.yml
  format: yaml
  label: FOSSology Folders API
  slug: fossology-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-folders-api-openapi.yml
- filename: fossology-groups-api-openapi.yml
  format: yaml
  label: FOSSology Groups API
  slug: fossology-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-groups-api-openapi.yml
- filename: fossology-info-api-openapi.yml
  format: yaml
  label: FOSSology info API
  slug: fossology-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-info-api-openapi.yml
- filename: fossology-job-api-openapi.yml
  format: yaml
  label: FOSSology Job API
  slug: fossology-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-job-api-openapi.yml
- filename: fossology-license-api-openapi.yml
  format: yaml
  label: FOSSology License API
  slug: fossology-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-license-api-openapi.yml
- filename: fossology-maintenance-api-openapi.yml
  format: yaml
  label: FOSSology Maintenance API
  slug: fossology-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-maintenance-api-openapi.yml
- filename: fossology-organize-api-openapi.yml
  format: yaml
  label: FOSSology Organize API
  slug: fossology-organize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-organize-api-openapi.yml
- filename: fossology-overview-api-openapi.yml
  format: yaml
  label: FOSSology Overview API
  slug: fossology-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-overview-api-openapi.yml
- filename: fossology-report-api-openapi.yml
  format: yaml
  label: FOSSology Report API
  slug: fossology-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-report-api-openapi.yml
- filename: fossology-search-api-openapi.yml
  format: yaml
  label: FOSSology Search API
  slug: fossology-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-search-api-openapi.yml
- filename: fossology-upload-api-openapi.yml
  format: yaml
  label: FOSSology Upload API
  slug: fossology-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-upload-api-openapi.yml
- filename: fossology-user-api-openapi.yml
  format: yaml
  label: FOSSology User API
  slug: fossology-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-user-api-openapi.yml
authorization_urls: []
description: ''
docs: https://github.com/fossology/fossology/wiki/FOSSology-REST-API
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Fossology Scopes
name_suffix: OAuth Scopes
note: FOSSology authenticates with JWT bearer tokens (or OIDC machine-to-machine tokens) whose scope is limited to read or write; it does not publish a finer-grained OAuth scope catalog (https://github.com/fossology/fossology/wiki/FOSSology-REST-API).
overview: 'FOSSology publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FOSSology API on a user''s behalf.


  Tokens are issued from https://api.example.com/oauth2/authorize.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FOSSology
provider_slug: fossology
schemes:
- description: Machine-2-Machine communication from oauth
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.example.com/oauth2/authorize
  name: oauth
  source: openapi/fossology-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read-only access to the FOSSology REST API, allowing retrieval of information without creating or modifying data. Requested as token_scope when generating a token via POST /tokens and carried in the JWT scope claim.
  flows: []
  scope: read
- description: Read-write access to the FOSSology REST API, allowing creation and modification of data such as uploads, jobs, and clearing decisions. Requested as token_scope when generating a token via POST /tokens and carried in the JWT scope claim.
  flows: []
  scope: write
slug: fossology-scopes
source_filename: fossology-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/fossology-openapi.yml\ndocs: https://github.com/fossology/fossology/wiki/FOSSology-REST-API\nschemes:\n- name: oauth\n  source: openapi/fossology-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.example.com/oauth2/authorize\n  description: Machine-2-Machine communication from oauth\nscopes:\n- scope: read\n  description: Read-only access to the FOSSology REST API, allowing retrieval of\n    information without creating or modifying data. Requested as token_scope when\n    generating a token via POST /tokens and carried in the JWT scope claim.\n  sources:\n  - https://github.com/fossology/fossology/wiki/FOSSology-REST-API\n- scope: write\n  description: Read-write access to the FOSSology REST API, allowing creation and\n    modification of data such as uploads, jobs, and clearing decisions. Requested\n    as token_scope when generating a token via POST /tokens and carried in the JWT\n   \
  \ scope claim.\n  sources:\n  - https://github.com/fossology/fossology/wiki/FOSSology-REST-API\nnote: FOSSology authenticates with JWT bearer tokens (or OIDC machine-to-machine\n  tokens) whose scope is limited to read or write; it does not publish a finer-grained\n  OAuth scope catalog (https://github.com/fossology/fossology/wiki/FOSSology-REST-API).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/scopes/fossology-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Compliance
- Licensing
- Linux Foundation
- Scanning
- SPDX
- Open-Source
token_urls:
- https://api.example.com/oauth2/authorize
---
