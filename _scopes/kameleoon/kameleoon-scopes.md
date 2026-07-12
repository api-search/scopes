---
authorization_urls:
- https://api.kameleoon.com/oauth/authorize
description: ''
docs: https://docs.kameleoon.com/developer-docs/apis/automation-api-rest/get-started/get-started
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Kameleoon Scopes
name_suffix: OAuth Scopes
note: Kameleoon's Automation API uses OAuth 2.0 client credentials and authorization code flows but does not document any OAuth scopes; access is tied to the Kameleoon user account behind the API credentials (https://docs.kameleoon.com/developer-docs/apis/automation-api-rest/get-started/get-started).
overview: 'Kameleoon uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.kameleoon.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kameleoon
provider_slug: kameleoon
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.kameleoon.com/oauth/token
  - authorizationUrl: https://api.kameleoon.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kameleoon.com/oauth/token
  name: oauth2
  source: openapi/kameleoon-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: kameleoon-scopes
source_filename: kameleoon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kameleoon-openapi.yml\ndocs: https://docs.kameleoon.com/developer-docs/apis/automation-api-rest/get-started/get-started\nnote: >-\n  Kameleoon's Automation API uses OAuth 2.0 client credentials and authorization\n  code flows but does not document any OAuth scopes; access is tied to the\n  Kameleoon user account behind the API credentials\n  (https://docs.kameleoon.com/developer-docs/apis/automation-api-rest/get-started/get-started).\nschemes:\n- name: oauth2\n  source: openapi/kameleoon-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.kameleoon.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.kameleoon.com/oauth/authorize\n    tokenUrl: https://api.kameleoon.com/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/scopes/kameleoon-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Experimentation
- AB Testing
- Personalization
- Feature Flags
- AI
token_urls:
- https://api.kameleoon.com/oauth/token
---
