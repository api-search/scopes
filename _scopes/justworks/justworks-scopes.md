---
api_specs:
- filename: justworks-members-api-openapi.yml
  format: yaml
  label: Justworks Members API
  slug: justworks-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-members-api-openapi.yml
- filename: justworks-company-api-openapi.yml
  format: yaml
  label: Justworks Company API
  slug: justworks-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-company-api-openapi.yml
- filename: justworks-payroll-api-openapi.yml
  format: yaml
  label: Justworks Payroll API
  slug: justworks-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-payroll-api-openapi.yml
- filename: justworks-deductions-api-openapi.yml
  format: yaml
  label: Justworks Deductions API
  slug: justworks-deductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-deductions-api-openapi.yml
- filename: justworks-time-off-api-openapi.yml
  format: yaml
  label: Justworks Time Off API
  slug: justworks-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-time-off-api-openapi.yml
- filename: justworks-webhooks-api-openapi.yml
  format: yaml
  label: Justworks Webhooks API
  slug: justworks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-webhooks-api-openapi.yml
- filename: justworks-oauth-api-openapi.yml
  format: yaml
  label: Justworks OAuth API
  slug: justworks-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-oauth-api-openapi.yml
authorization_urls:
- https://secure.justworks.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Justworks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Justworks publishes 15 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Justworks API on a user''s behalf.


  Tokens are issued from https://public-api.justworks.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Justworks
provider_slug: justworks
schemes:
- flows:
  - authorizationUrl: https://secure.justworks.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://public-api.justworks.com/oauth/token
  name: OAuth2
  source: openapi/justworks-company-api-openapi.yml
- flows:
  - authorizationUrl: https://secure.justworks.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://public-api.justworks.com/oauth/token
  name: OAuth2
  source: openapi/justworks-deductions-api-openapi.yml
- flows:
  - authorizationUrl: https://secure.justworks.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://public-api.justworks.com/oauth/token
  name: OAuth2
  source: openapi/justworks-members-api-openapi.yml
- flows:
  - authorizationUrl: https://secure.justworks.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://public-api.justworks.com/oauth/token
  name: OAuth2
  source: openapi/justworks-payroll-api-openapi.yml
- flows:
  - authorizationUrl: https://secure.justworks.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://public-api.justworks.com/oauth/token
  name: OAuth2
  source: openapi/justworks-time-off-api-openapi.yml
- flows:
  - authorizationUrl: https://secure.justworks.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://public-api.justworks.com/oauth/token
  name: OAuth2
  source: openapi/justworks-webhooks-api-openapi.yml
scope_count: 15
scope_names:
- company.bank_account:read
- company.basic:read
- company.detail:read
- deductions:read
- deductions:write
- member.basic:read
- member.detail:read
- member.dob:read
- member.employment:read
- member.pay:read
- member.sex:read
- member.tax_id:read
- payroll:read
- paystub:read
- time_off:read
scopes:
- description: Read company bank account on file
  flows:
  - authorizationCode
  scope: company.bank_account:read
- description: Read basic company data
  flows:
  - authorizationCode
  scope: company.basic:read
- description: Read detailed company data
  flows:
  - authorizationCode
  scope: company.detail:read
- description: Read deductions
  flows:
  - authorizationCode
  scope: deductions:read
- description: Create, update, and cancel deductions
  flows:
  - authorizationCode
  scope: deductions:write
- description: Read basic member profile fields
  flows:
  - authorizationCode
  scope: member.basic:read
- description: Read detailed member profile including history
  flows:
  - authorizationCode
  scope: member.detail:read
- description: Read date of birth
  flows:
  - authorizationCode
  scope: member.dob:read
- description: Read employment records
  flows:
  - authorizationCode
  scope: member.employment:read
- description: Read pay history
  flows:
  - authorizationCode
  scope: member.pay:read
- description: Read sex assigned at birth
  flows:
  - authorizationCode
  scope: member.sex:read
- description: Read U.S. tax identifier (SSN)
  flows:
  - authorizationCode
  scope: member.tax_id:read
- description: Read payroll runs and fees
  flows:
  - authorizationCode
  scope: payroll:read
- description: Read paystub detail
  flows:
  - authorizationCode
  scope: paystub:read
- description: Read time-off policies, balances, and requests
  flows:
  - authorizationCode
  scope: time_off:read
slug: justworks-scopes
source_filename: justworks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/justworks-company-api-openapi.yml, openapi/justworks-deductions-api-openapi.yml,\n  openapi/justworks-members-api-openapi.yml, openapi/justworks-payroll-api-openapi.yml, openapi/justworks-time-off-api-openapi.yml,\n  openapi/justworks-webhooks-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/justworks-company-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.justworks.com/oauth/authorize\n    tokenUrl: https://public-api.justworks.com/oauth/token\n- name: OAuth2\n  source: openapi/justworks-deductions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.justworks.com/oauth/authorize\n    tokenUrl: https://public-api.justworks.com/oauth/token\n- name: OAuth2\n  source: openapi/justworks-members-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.justworks.com/oauth/authorize\n    tokenUrl:\
  \ https://public-api.justworks.com/oauth/token\n- name: OAuth2\n  source: openapi/justworks-payroll-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.justworks.com/oauth/authorize\n    tokenUrl: https://public-api.justworks.com/oauth/token\n- name: OAuth2\n  source: openapi/justworks-time-off-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.justworks.com/oauth/authorize\n    tokenUrl: https://public-api.justworks.com/oauth/token\n- name: OAuth2\n  source: openapi/justworks-webhooks-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.justworks.com/oauth/authorize\n    tokenUrl: https://public-api.justworks.com/oauth/token\nscopes:\n- scope: company.bank_account:read\n  description: Read company bank account on file\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-company-api-openapi.yml\n- scope: company.basic:read\n  description: Read basic\
  \ company data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-company-api-openapi.yml\n- scope: company.detail:read\n  description: Read detailed company data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-company-api-openapi.yml\n- scope: deductions:read\n  description: Read deductions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-deductions-api-openapi.yml\n- scope: deductions:write\n  description: Create, update, and cancel deductions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-deductions-api-openapi.yml\n- scope: member.basic:read\n  description: Read basic member profile fields\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-members-api-openapi.yml\n- scope: member.detail:read\n  description: Read detailed member profile including history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-members-api-openapi.yml\n- scope: member.dob:read\n  description: Read\
  \ date of birth\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-members-api-openapi.yml\n- scope: member.employment:read\n  description: Read employment records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-members-api-openapi.yml\n- scope: member.pay:read\n  description: Read pay history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-members-api-openapi.yml\n- scope: member.sex:read\n  description: Read sex assigned at birth\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-members-api-openapi.yml\n- scope: member.tax_id:read\n  description: Read U.S. tax identifier (SSN)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-members-api-openapi.yml\n- scope: payroll:read\n  description: Read payroll runs and fees\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-payroll-api-openapi.yml\n- scope: paystub:read\n  description: Read paystub detail\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/justworks-payroll-api-openapi.yml\n- scope: time_off:read\n  description: Read time-off policies, balances, and requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justworks-time-off-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/scopes/justworks-scopes.yml
summary_line: 15 scopes · authorizationCode
tags:
- PEO
- Payroll
- HR
- Human Resources
- Benefits
- Health Insurance
- 401(k)
- Time Off
- Compliance
- Small Business
- Employer of Record
- HRIS
token_urls:
- https://public-api.justworks.com/oauth/token
---
