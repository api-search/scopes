---
api_specs:
- filename: llms.txt
  format: yaml
  label: Acuity Scheduling API
  slug: acuity-scheduling-api
  spec_type: OpenAPI
  url: https://developers.acuityscheduling.com/llms.txt
authorization_urls:
- https://acuityscheduling.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Acuity Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Acuity Scheduling publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Acuity Scheduling API on a user''s behalf.


  Tokens are issued from https://acuityscheduling.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Acuity Scheduling
provider_slug: acuity
schemes:
- description: OAuth2 for multi-account integrations
  flows:
  - authorizationUrl: https://acuityscheduling.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://acuityscheduling.com/oauth2/token
  name: oauth2
  source: openapi/acuity-scheduling-api-openapi.yml
scope_count: 1
scope_names:
- api
scopes:
- description: Full API access
  flows:
  - authorizationCode
  scope: api
slug: acuity-scopes
source_filename: acuity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acuity-scheduling-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/acuity-scheduling-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://acuityscheduling.com/oauth2/authorize\n    tokenUrl: https://acuityscheduling.com/oauth2/token\n  description: OAuth2 for multi-account integrations\nscopes:\n- scope: api\n  description: Full API access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/acuity-scheduling-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acuity/refs/heads/main/scopes/acuity-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Scheduling
- Appointments
- Calendar
- Booking
- HIPAA
- Webhooks
token_urls:
- https://acuityscheduling.com/oauth2/token
---
