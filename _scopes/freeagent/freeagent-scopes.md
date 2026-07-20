---
api_specs:
- filename: postman-freeagent-api-collection
  format: yaml
  label: FreeAgent REST API
  slug: rest-api
  spec_type: Postman
  url: https://github.com/fac/postman-freeagent-api-collection
authorization_urls:
- https://api.freeagent.com/v2/approve_app
description: ''
docs: https://dev.freeagent.com/docs/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Freeagent Scopes
name_suffix: OAuth Scopes
note: FreeAgent's OAuth 2.0 authorization code flow does not use or document OAuth scopes; API access is instead limited by the authorizing FreeAgent user's numeric permission level (0 No Access through 8 Full), with a minimum required access level specified per resource (https://dev.freeagent.com/docs/introduction).
overview: 'FreeAgent uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.freeagent.com/v2/token_endpoint.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FreeAgent
provider_slug: freeagent
schemes:
- description: 'OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;

    refresh tokens used to obtain new access tokens.'
  flows:
  - authorizationUrl: https://api.freeagent.com/v2/approve_app
    flow: authorizationCode
    tokenUrl: https://api.freeagent.com/v2/token_endpoint
  name: oauth2
  source: openapi/freeagent-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: freeagent-scopes
source_filename: freeagent-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freeagent-openapi.yml\ndocs: https://dev.freeagent.com/docs/oauth\nnote: >-\n  FreeAgent's OAuth 2.0 authorization code flow does not use or document OAuth\n  scopes; API access is instead limited by the authorizing FreeAgent user's\n  numeric permission level (0 No Access through 8 Full), with a minimum\n  required access level specified per resource\n  (https://dev.freeagent.com/docs/introduction).\nschemes:\n- name: oauth2\n  source: openapi/freeagent-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.freeagent.com/v2/approve_app\n    tokenUrl: https://api.freeagent.com/v2/token_endpoint\n  description: |-\n    OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;\n    refresh tokens used to obtain new access tokens.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeagent/refs/heads/main/scopes/freeagent-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Accounting
- Small Business
- Invoicing
- Bookkeeping
- Expenses
- Payroll
- VAT
- HMRC
- Making Tax Digital
token_urls:
- https://api.freeagent.com/v2/token_endpoint
---
