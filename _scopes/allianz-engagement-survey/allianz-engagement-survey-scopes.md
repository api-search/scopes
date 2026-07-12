---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Allianz Engagement Survey Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allianz Engagement Survey publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allianz Engagement Survey API on a user''s behalf.


  Tokens are issued from https://api.allianz.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schemes:
- description: OAuth2 client credentials for Allianz internal API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.allianz.com/oauth2/token
  name: OAuth2
  source: openapi/allianz-engagement-survey.yaml
scope_count: 5
scope_names:
- action_plans:write
- analytics:read
- responses:read
- surveys:read
- surveys:write
scopes:
- description: Create and manage action plans
  flows:
  - clientCredentials
  scope: action_plans:write
- description: Access survey analytics and reporting
  flows:
  - clientCredentials
  scope: analytics:read
- description: Read anonymized survey responses
  flows:
  - clientCredentials
  scope: responses:read
- description: Read survey definitions and configurations
  flows:
  - clientCredentials
  scope: surveys:read
- description: Create and manage surveys
  flows:
  - clientCredentials
  scope: surveys:write
slug: allianz-engagement-survey-scopes
source_filename: allianz-engagement-survey-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-engagement-survey.yaml\nschemes:\n- name: OAuth2\n  source: openapi/allianz-engagement-survey.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.allianz.com/oauth2/token\n  description: OAuth2 client credentials for Allianz internal API access\nscopes:\n- scope: action_plans:write\n  description: Create and manage action plans\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-engagement-survey.yaml\n- scope: analytics:read\n  description: Access survey analytics and reporting\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-engagement-survey.yaml\n- scope: responses:read\n  description: Read anonymized survey responses\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-engagement-survey.yaml\n- scope: surveys:read\n  description: Read survey definitions and configurations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-engagement-survey.yaml\n\
  - scope: surveys:write\n  description: Create and manage surveys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-engagement-survey.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/scopes/allianz-engagement-survey-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
token_urls:
- https://api.allianz.com/oauth2/token
---
