---
authorization_urls:
- https://api.surveymonkey.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Surveymonkey Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SurveyMonkey publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SurveyMonkey API on a user''s behalf.


  Tokens are issued from https://api.surveymonkey.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SurveyMonkey
provider_slug: surveymonkey
schemes:
- flows:
  - authorizationUrl: https://api.surveymonkey.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.surveymonkey.com/oauth/token
  name: oauth2
  source: openapi/surveymonkey-openapi.yml
scope_count: 7
scope_names:
- contacts_read
- contacts_write
- responses_read
- responses_write
- surveys_read
- surveys_write
- users_read
scopes:
- description: Read contacts
  flows:
  - authorizationCode
  scope: contacts_read
- description: Modify contacts
  flows:
  - authorizationCode
  scope: contacts_write
- description: Read responses
  flows:
  - authorizationCode
  scope: responses_read
- description: Create and modify responses
  flows:
  - authorizationCode
  scope: responses_write
- description: Read surveys
  flows:
  - authorizationCode
  scope: surveys_read
- description: Create and modify surveys
  flows:
  - authorizationCode
  scope: surveys_write
- description: Read user data
  flows:
  - authorizationCode
  scope: users_read
slug: surveymonkey-scopes
source_filename: surveymonkey-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/surveymonkey-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/surveymonkey-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.surveymonkey.com/oauth/authorize\n    tokenUrl: https://api.surveymonkey.com/oauth/token\nscopes:\n- scope: contacts_read\n  description: Read contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/surveymonkey-openapi.yml\n- scope: contacts_write\n  description: Modify contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/surveymonkey-openapi.yml\n- scope: responses_read\n  description: Read responses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/surveymonkey-openapi.yml\n- scope: responses_write\n  description: Create and modify responses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/surveymonkey-openapi.yml\n- scope: surveys_read\n  description: Read surveys\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/surveymonkey-openapi.yml\n- scope: surveys_write\n  description: Create and modify surveys\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/surveymonkey-openapi.yml\n- scope: users_read\n  description: Read user data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/surveymonkey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surveymonkey/refs/heads/main/scopes/surveymonkey-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Surveys
- Market Research
- Feedback
- NPS
- Forms
- OAuth
token_urls:
- https://api.surveymonkey.com/oauth/token
---
