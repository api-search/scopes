---
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
- Open Source
token_urls:
- https://api.example.com/oauth2/authorize
---
