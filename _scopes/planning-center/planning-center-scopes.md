---
authorization_urls:
- https://api.planningcenteronline.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Planning Center Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Planning Center publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Planning Center API on a user''s behalf.


  Tokens are issued from https://api.planningcenteronline.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Planning Center
provider_slug: planning-center
schemes:
- flows:
  - authorizationUrl: https://api.planningcenteronline.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.planningcenteronline.com/oauth/token
  name: oauth2
  source: openapi/planning-center-openapi.yml
scope_count: 8
scope_names:
- calendar
- check_ins
- giving
- groups
- people
- publishing
- registrations
- services
scopes:
- description: Access the Calendar product
  flows:
  - authorizationCode
  scope: calendar
- description: Access the Check-Ins product
  flows:
  - authorizationCode
  scope: check_ins
- description: Access the Giving product
  flows:
  - authorizationCode
  scope: giving
- description: Access the Groups product
  flows:
  - authorizationCode
  scope: groups
- description: Access the People product
  flows:
  - authorizationCode
  scope: people
- description: Access the Publishing product
  flows:
  - authorizationCode
  scope: publishing
- description: Access the Registrations product
  flows:
  - authorizationCode
  scope: registrations
- description: Access the Services product
  flows:
  - authorizationCode
  scope: services
slug: planning-center-scopes
source_filename: planning-center-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/planning-center-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/planning-center-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.planningcenteronline.com/oauth/authorize\n    tokenUrl: https://api.planningcenteronline.com/oauth/token\nscopes:\n- scope: calendar\n  description: Access the Calendar product\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/planning-center-openapi.yml\n- scope: check_ins\n  description: Access the Check-Ins product\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/planning-center-openapi.yml\n- scope: giving\n  description: Access the Giving product\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/planning-center-openapi.yml\n- scope: groups\n  description: Access the Groups product\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/planning-center-openapi.yml\n- scope: people\n  description: Access the People\
  \ product\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/planning-center-openapi.yml\n- scope: publishing\n  description: Access the Publishing product\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/planning-center-openapi.yml\n- scope: registrations\n  description: Access the Registrations product\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/planning-center-openapi.yml\n- scope: services\n  description: Access the Services product\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/planning-center-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/scopes/planning-center-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Church Management
- ChMS
- Faith
- Giving
- Events
- Scheduling
- People
- Nonprofit
token_urls:
- https://api.planningcenteronline.com/oauth/token
---
