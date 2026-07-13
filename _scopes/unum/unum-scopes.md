---
api_specs:
- filename: unum-hr-connect-openapi.yml
  format: yaml
  label: Unum HR Connect API
  slug: hr-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-hr-connect-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Unum Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Unum publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unum API on a user''s behalf.


  Tokens are issued from https://api.unum.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unum
provider_slug: unum
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.unum.com/v1/oauth/token
  name: OAuth2
  source: openapi/unum-hr-connect-openapi.yml
scope_count: 9
scope_names:
- billing:read
- eligibility:read
- eligibility:write
- enrollment:read
- enrollment:write
- eoi:read
- eoi:write
- leave:read
- leave:write
scopes:
- description: Read billing invoices
  flows:
  - clientCredentials
  scope: billing:read
- description: Read member eligibility
  flows:
  - clientCredentials
  scope: eligibility:read
- description: Write member eligibility
  flows:
  - clientCredentials
  scope: eligibility:write
- description: Read enrollment elections
  flows:
  - clientCredentials
  scope: enrollment:read
- description: Write enrollment elections
  flows:
  - clientCredentials
  scope: enrollment:write
- description: Read EOI submissions
  flows:
  - clientCredentials
  scope: eoi:read
- description: Write EOI submissions
  flows:
  - clientCredentials
  scope: eoi:write
- description: Read leave requests
  flows:
  - clientCredentials
  scope: leave:read
- description: Write leave requests
  flows:
  - clientCredentials
  scope: leave:write
slug: unum-scopes
source_filename: unum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unum-hr-connect-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/unum-hr-connect-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.unum.com/v1/oauth/token\nscopes:\n- scope: billing:read\n  description: Read billing invoices\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n- scope: eligibility:read\n  description: Read member eligibility\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n- scope: eligibility:write\n  description: Write member eligibility\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n- scope: enrollment:read\n  description: Read enrollment elections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n- scope: enrollment:write\n  description: Write enrollment elections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n\
  - scope: eoi:read\n  description: Read EOI submissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n- scope: eoi:write\n  description: Write EOI submissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n- scope: leave:read\n  description: Read leave requests\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n- scope: leave:write\n  description: Write leave requests\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/scopes/unum-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Insurance
- Benefits Administration
- HR Integration
- Disability Insurance
- Life Insurance
- Fortune 500
token_urls:
- https://api.unum.com/v1/oauth/token
---
