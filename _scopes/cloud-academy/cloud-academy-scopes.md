---
api_specs:
- filename: cloud-academy-openapi-original.json
  format: json
  label: QA API (Cloud Academy)
  slug: qa-api-cloud-academy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-academy/refs/heads/main/openapi/cloud-academy-openapi-original.json
authorization_urls:
- https://platform.qa.com/oauth2/authorize/
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cloud Academy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cloud Academy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://platform.qa.com/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cloud Academy
provider_slug: cloud-academy
schemes:
- description: Insert your API key pair.<br/><br/>Enterprise members with Admin permissions can generate and view their own API keys on the settings area of their Company Account [here](https://platform.qa.com/organizations/settings/api/).
  flows:
  - authorizationUrl: https://platform.qa.com/oauth2/authorize/
    flow: clientCredentials
    tokenUrl: https://platform.qa.com/oauth2/token/
  name: oauth2
  source: openapi/cloud-academy-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: cloud-academy-scopes
source_filename: cloud-academy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cloud-academy-openapi-original.json\nschemes:\n- name: oauth2\n  source: openapi/cloud-academy-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    authorizationUrl: https://platform.qa.com/oauth2/authorize/\n    tokenUrl: https://platform.qa.com/oauth2/token/\n  description: Insert your API key pair.<br/><br/>Enterprise members with Admin permissions\n    can generate and view their own API keys on the settings area of their Company Account [here](https://platform.qa.com/organizations/settings/api/).\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-academy/refs/heads/main/scopes/cloud-academy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Training
- Education
- Learning Management
- Cloud Computing
- Skills
- Reporting
- eLearning
token_urls:
- https://platform.qa.com/oauth2/token/
---
