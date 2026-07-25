---
api_specs:
- filename: airship-push-api-openapi.yml
  format: yaml
  label: Airship Push API
  slug: airship-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-push-api-openapi.yml
- filename: airship-segments-api-openapi.yml
  format: yaml
  label: Airship Segments API
  slug: airship-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-segments-api-openapi.yml
- filename: airship-reports-api-openapi.yml
  format: yaml
  label: Airship Reports API
  slug: airship-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-reports-api-openapi.yml
- filename: airship-channels-api-openapi.yml
  format: yaml
  label: Airship Channels API
  slug: airship-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-channels-api-openapi.yml
- filename: airship-custom-events-api-openapi.yml
  format: yaml
  label: Airship Custom Events API
  slug: airship-custom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-custom-events-api-openapi.yml
- filename: airship-lists-api-openapi.yml
  format: yaml
  label: Airship Lists API
  slug: airship-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-lists-api-openapi.yml
- filename: airship-message-center-api-openapi.yml
  format: yaml
  label: Airship Message Center API
  slug: airship-message-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-message-center-api-openapi.yml
- filename: airship-named-users-api-openapi.yml
  format: yaml
  label: Airship Named Users API
  slug: airship-named-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-named-users-api-openapi.yml
- filename: airship-push-api-openapi.yml
  format: yaml
  label: Airship Push API
  slug: airship-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-push-api-openapi.yml
- filename: airship-reports-api-openapi.yml
  format: yaml
  label: Airship Reports API
  slug: airship-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-reports-api-openapi.yml
- filename: airship-schedules-api-openapi.yml
  format: yaml
  label: Airship Schedules API
  slug: airship-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-schedules-api-openapi.yml
- filename: airship-segments-api-openapi.yml
  format: yaml
  label: Airship Segments API
  slug: airship-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-segments-api-openapi.yml
- filename: airship-templates-api-openapi.yml
  format: yaml
  label: Airship Templates API
  slug: airship-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/openapi/airship-templates-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Airship Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Airship publishes 11 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Airship API on a user''s behalf.


  Tokens are issued from https://oauth2.asnapieu.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Airship
provider_slug: airship
schemes:
- description: 'OAuth 2.0 scoped tokens. Scopes include att (attachments), chn (channels),

    cnt (contacts), evt (events), lst (lists), nu (named users), pln (pipelines),

    psh (push), rpt (reports), sch (schedules), tpl (content templates).'
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth2.asnapieu.com/token
  name: OAuth2
  source: openapi/airship-openapi.yml
scope_count: 11
scope_names:
- att
- chn
- cnt
- evt
- lst
- nu
- pln
- psh
- rpt
- sch
- tpl
scopes:
- description: Attachments
  flows:
  - clientCredentials
  scope: att
- description: Channels
  flows:
  - clientCredentials
  scope: chn
- description: Contacts
  flows:
  - clientCredentials
  scope: cnt
- description: Events
  flows:
  - clientCredentials
  scope: evt
- description: Lists
  flows:
  - clientCredentials
  scope: lst
- description: Named Users
  flows:
  - clientCredentials
  scope: nu
- description: Pipelines
  flows:
  - clientCredentials
  scope: pln
- description: Push
  flows:
  - clientCredentials
  scope: psh
- description: Reports
  flows:
  - clientCredentials
  scope: rpt
- description: Schedules
  flows:
  - clientCredentials
  scope: sch
- description: Content Templates
  flows:
  - clientCredentials
  scope: tpl
slug: airship-scopes
source_filename: airship-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airship-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/airship-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth2.asnapieu.com/token\n  description: |-\n    OAuth 2.0 scoped tokens. Scopes include att (attachments), chn (channels),\n    cnt (contacts), evt (events), lst (lists), nu (named users), pln (pipelines),\n    psh (push), rpt (reports), sch (schedules), tpl (content templates).\nscopes:\n- scope: att\n  description: Attachments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: chn\n  description: Channels\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: cnt\n  description: Contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: evt\n  description: Events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: lst\n  description:\
  \ Lists\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: nu\n  description: Named Users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: pln\n  description: Pipelines\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: psh\n  description: Push\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: rpt\n  description: Reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: sch\n  description: Schedules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n- scope: tpl\n  description: Content Templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/airship-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airship/refs/heads/main/scopes/airship-scopes.yml
summary_line: 11 scopes · clientCredentials
tags:
- Notifications
- Push
- Email
- Mobile
- CDP
token_urls:
- https://oauth2.asnapieu.com/token
---
