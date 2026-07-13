---
api_specs:
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Team Members
  slug: team-members
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Leave / Absences
  slug: leave-absences
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Leave Allowances
  slug: leave-allowances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
- filename: charliehr-openapi.yml
  format: yaml
  label: CharlieHR Company
  slug: company
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-openapi.yml
authorization_urls: []
description: ''
docs: https://www.charliehr.com/api_docs/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Charliehr Scopes
name_suffix: OAuth Scopes
note: CharlieHR does not publish OAuth scopes - the API docs (https://www.charliehr.com/api_docs/) show every endpoint authenticated with company-level client credentials sent as an Authorization header (Token token=client_id:client_secret), with no scope or permission-level system documented.
overview: 'CharlieHR uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://charliehr.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CharlieHR
provider_slug: charliehr
schemes:
- description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged for an access token, which is sent in the Authorization header of each request.
  flows:
  - flow: clientCredentials
    tokenUrl: https://charliehr.com/oauth/token
  name: oauth2
  source: openapi/charliehr-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: charliehr-scopes
source_filename: charliehr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/charliehr-openapi.yml\ndocs: https://www.charliehr.com/api_docs/\nnote: CharlieHR does not publish OAuth scopes - the API docs (https://www.charliehr.com/api_docs/)\n  show every endpoint authenticated with company-level client credentials sent as\n  an Authorization header (Token token=client_id:client_secret), with no scope or\n  permission-level system documented.\nschemes:\n- name: oauth2\n  source: openapi/charliehr-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://charliehr.com/oauth/token\n  description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged\n    for an access token, which is sent in the Authorization header of each request.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/scopes/charliehr-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- HR
- HRIS
- People
- Leave
- Time Off
token_urls:
- https://charliehr.com/oauth/token
---
