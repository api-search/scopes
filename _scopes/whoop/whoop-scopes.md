---
authorization_urls:
- https://api.prod.whoop.com/oauth/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Whoop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WHOOP publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the WHOOP API on a user''s behalf.


  Tokens are issued from https://api.prod.whoop.com/oauth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WHOOP
provider_slug: whoop
schemes:
- flows:
  - authorizationUrl: https://api.prod.whoop.com/oauth/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://api.prod.whoop.com/oauth/oauth2/token
  name: OAuth
  source: openapi/whoop-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prod.whoop.com/developer/v2/partner/token
  name: Trusted Partner
  source: openapi/whoop-openapi.yml
scope_count: 7
scope_names:
- read:body_measurement
- read:cycles
- read:profile
- read:recovery
- read:sleep
- read:workout
- whoop-partner/token
scopes:
- description: Read body measurements data, including height, weight, and max heart rate.
  flows:
  - authorizationCode
  scope: read:body_measurement
- description: Read cycles data, including day Strain and average heart rate during a physiological cycle.
  flows:
  - authorizationCode
  scope: read:cycles
- description: Read profile data, including name and email.
  flows:
  - authorizationCode
  scope: read:profile
- description: Read Recovery data, including score, heart rate variability, and resting heart rate.
  flows:
  - authorizationCode
  scope: read:recovery
- description: Read sleep data, including performance % and duration per sleep stage.
  flows:
  - authorizationCode
  scope: read:sleep
- description: Read workout data, including activity Strain and average heart rate.
  flows:
  - authorizationCode
  scope: read:workout
- description: Read service requests and upload results.
  flows:
  - clientCredentials
  scope: whoop-partner/token
slug: whoop-scopes
source_filename: whoop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whoop-openapi.yml\nschemes:\n- name: OAuth\n  source: openapi/whoop-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.prod.whoop.com/oauth/oauth2/auth\n    tokenUrl: https://api.prod.whoop.com/oauth/oauth2/token\n- name: Trusted Partner\n  source: openapi/whoop-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prod.whoop.com/developer/v2/partner/token\nscopes:\n- scope: read:body_measurement\n  description: Read body measurements data, including height, weight, and max heart rate.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/whoop-openapi.yml\n- scope: read:cycles\n  description: Read cycles data, including day Strain and average heart rate during a physiological\n    cycle.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/whoop-openapi.yml\n- scope: read:profile\n  description: Read profile data, including name and email.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/whoop-openapi.yml\n- scope: read:recovery\n  description: Read Recovery data, including score, heart rate variability, and resting heart\n    rate.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/whoop-openapi.yml\n- scope: read:sleep\n  description: Read sleep data, including performance % and duration per sleep stage.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/whoop-openapi.yml\n- scope: read:workout\n  description: Read workout data, including activity Strain and average heart rate.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/whoop-openapi.yml\n- scope: whoop-partner/token\n  description: Read service requests and upload results.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/whoop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whoop/refs/heads/main/scopes/whoop-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- Fitness
- Wearables
- Health
- Recovery
- Sleep
- Workout
- Strain
- Heart Rate
- Performance
token_urls:
- https://api.prod.whoop.com/oauth/oauth2/token
- https://api.prod.whoop.com/developer/v2/partner/token
---
