---
authorization_urls:
- https://www.smartrecruiters.com/identity/oauth/allow
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Smartrecruiters Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SmartRecruiters publishes 4 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the SmartRecruiters API on a user''s behalf.


  Tokens are issued from https://www.smartrecruiters.com/identity/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SmartRecruiters
provider_slug: smartrecruiters
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token
  name: OAuth2
  source: openapi/smartrecruiters-candidates-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token
  name: OAuth2
  source: openapi/smartrecruiters-jobs-openapi.yml
- flows:
  - authorizationUrl: https://www.smartrecruiters.com/identity/oauth/allow
    flow: authorizationCode
    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token
  name: OAuth2
  source: openapi/smartrecruiters-posting-openapi.yml
scope_count: 4
scope_names:
- candidates.read
- candidates.write
- jobs.read
- jobs.write
scopes:
- description: Read candidate data
  flows:
  - authorizationCode
  - clientCredentials
  scope: candidates.read
- description: Write candidate data
  flows:
  - authorizationCode
  - clientCredentials
  scope: candidates.write
- description: Read job data
  flows:
  - authorizationCode
  - clientCredentials
  scope: jobs.read
- description: Write job data
  flows:
  - authorizationCode
  - clientCredentials
  scope: jobs.write
slug: smartrecruiters-scopes
source_filename: smartrecruiters-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartrecruiters-candidates-openapi.yml, openapi/smartrecruiters-jobs-openapi.yml,\n  openapi/smartrecruiters-posting-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/smartrecruiters-candidates-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token\n- name: OAuth2\n  source: openapi/smartrecruiters-jobs-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token\n- name: OAuth2\n  source: openapi/smartrecruiters-posting-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.smartrecruiters.com/identity/oauth/allow\n    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token\nscopes:\n- scope: candidates.read\n  description: Read candidate data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/smartrecruiters-candidates-openapi.yml\n\
  \  - openapi/smartrecruiters-posting-openapi.yml\n- scope: candidates.write\n  description: Write candidate data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/smartrecruiters-candidates-openapi.yml\n  - openapi/smartrecruiters-posting-openapi.yml\n- scope: jobs.read\n  description: Read job data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/smartrecruiters-jobs-openapi.yml\n  - openapi/smartrecruiters-posting-openapi.yml\n- scope: jobs.write\n  description: Write job data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/smartrecruiters-jobs-openapi.yml\n  - openapi/smartrecruiters-posting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/scopes/smartrecruiters-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode
tags:
- Human Resources
- Recruiting
- Talent Acquisition
- Applicant Tracking
- HR Technology
token_urls:
- https://www.smartrecruiters.com/identity/oauth/token
---
