---
api_specs:
- filename: paychex-payroll-companies-openapi.yml
  format: yaml
  label: Paychex Payroll Companies API
  slug: paychex-payroll-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-payroll-companies-openapi.yml
- filename: paychex-workers-openapi.yml
  format: yaml
  label: Paychex Workers API
  slug: paychex-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-workers-openapi.yml
- filename: paychex-time-openapi.yml
  format: yaml
  label: Paychex Time API
  slug: paychex-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-time-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.paychex.com/getting-started/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Paychex Developer Scopes
name_suffix: OAuth Scopes
note: Paychex uses an OAuth 2.0 client_credentials flow with access granted per registered partner application and company rather than requestable scopes; the public docs (https://developer.paychex.com/getting-started/authentication) publish no scopes reference, showing scope values (read:company_people write:company_people read:workers) only inside a sample token response with no descriptions.
overview: 'Paychex uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.paychex.com/auth/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paychex
provider_slug: paychex-developer
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.paychex.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  source: openapi/paychex-payroll-companies-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.paychex.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  source: openapi/paychex-time-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.paychex.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  source: openapi/paychex-workers-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: paychex-developer-scopes
source_filename: paychex-developer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paychex-payroll-companies-openapi.yml, openapi/paychex-time-openapi.yml, openapi/paychex-workers-openapi.yml\ndocs: https://developer.paychex.com/getting-started/authentication\nnote: >-\n  Paychex uses an OAuth 2.0 client_credentials flow with access granted per registered\n  partner application and company rather than requestable scopes; the public docs\n  (https://developer.paychex.com/getting-started/authentication) publish no scopes\n  reference, showing scope values (read:company_people write:company_people read:workers)\n  only inside a sample token response with no descriptions.\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/paychex-payroll-companies-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paychex.com/auth/oauth/v2/token\n- name: oauth2ClientCredentials\n  source: openapi/paychex-time-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paychex.com/auth/oauth/v2/token\n\
  - name: oauth2ClientCredentials\n  source: openapi/paychex-workers-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paychex.com/auth/oauth/v2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/scopes/paychex-developer-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Benefits
- HCM
- HR
- Paychex Flex
- Payroll
- Time and Attendance
- Workforce
- Fortune 1000
token_urls:
- https://api.paychex.com/auth/oauth/v2/token
---
