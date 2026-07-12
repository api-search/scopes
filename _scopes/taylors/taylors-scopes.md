---
authorization_urls: []
description: ''
docs: https://librarycatalogue.taylors.edu.my/api/v1/.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Taylors Scopes
name_suffix: OAuth Scopes
note: The Koha REST API behind the Taylor's Library catalog supports OAuth2 client credentials only and does not use OAuth scopes — API clients inherit the permissions of the patron they are tied to, and the API documentation states "We do not yet support OAuth Scopes or the Authorization Code grant flow" (https://librarycatalogue.taylors.edu.my/api/v1/.html).
overview: 'Taylor''s University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://librarycatalogue.taylors.edu.my/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Taylor's University
provider_slug: taylors
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/taylors-library-rest.yaml
scope_count: 0
scope_names: []
scopes: []
slug: taylors-scopes
source_filename: taylors-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taylors-library-rest.yaml\ndocs: https://librarycatalogue.taylors.edu.my/api/v1/.html\nnote: >-\n  The Koha REST API behind the Taylor's Library catalog supports OAuth2 client\n  credentials only and does not use OAuth scopes — API clients inherit the\n  permissions of the patron they are tied to, and the API documentation states\n  \"We do not yet support OAuth Scopes or the Authorization Code grant flow\"\n  (https://librarycatalogue.taylors.edu.my/api/v1/.html).\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/taylors-library-rest.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/scopes/taylors-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Library
- Institutional Repository
- Open Data
- Malaysia
- Asia
token_urls:
- https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
---
