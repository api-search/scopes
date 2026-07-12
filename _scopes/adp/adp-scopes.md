---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Adp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ADP publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ADP API on a user''s behalf.


  Tokens are issued from https://accounts.adp.com/auth/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ADP
provider_slug: adp
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.adp.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  source: openapi/adp-payroll-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.adp.com/auth/oauth/v2/token
  name: oauth2ClientCredentials
  source: openapi/adp-workers-openapi.yml
scope_count: 3
scope_names:
- api__payroll-output-v1__read
- api__workers-v2__read
- api__workers-v2__write
scopes:
- description: Read payroll output data
  flows:
  - clientCredentials
  scope: api__payroll-output-v1__read
- description: Read worker data
  flows:
  - clientCredentials
  scope: api__workers-v2__read
- description: Write worker data
  flows:
  - clientCredentials
  scope: api__workers-v2__write
slug: adp-scopes
source_filename: adp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adp-payroll-openapi.yml, openapi/adp-workers-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/adp-payroll-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.adp.com/auth/oauth/v2/token\n- name: oauth2ClientCredentials\n  source: openapi/adp-workers-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.adp.com/auth/oauth/v2/token\nscopes:\n- scope: api__payroll-output-v1__read\n  description: Read payroll output data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/adp-payroll-openapi.yml\n- scope: api__workers-v2__read\n  description: Read worker data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/adp-workers-openapi.yml\n- scope: api__workers-v2__write\n  description: Write worker data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/adp-workers-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/scopes/adp-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
token_urls:
- https://accounts.adp.com/auth/oauth/v2/token
---
