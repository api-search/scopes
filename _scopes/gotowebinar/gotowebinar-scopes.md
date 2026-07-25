---
api_specs:
- filename: gotowebinar-attendees-api-openapi.yml
  format: yaml
  label: GoToWebinar Attendees API
  slug: gotowebinar-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-attendees-api-openapi.yml
- filename: gotowebinar-co-organizers-api-openapi.yml
  format: yaml
  label: GoToWebinar Co-Organizers API
  slug: gotowebinar-co-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-co-organizers-api-openapi.yml
- filename: gotowebinar-panelists-api-openapi.yml
  format: yaml
  label: GoToWebinar Panelists API
  slug: gotowebinar-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-panelists-api-openapi.yml
- filename: gotowebinar-polls-api-openapi.yml
  format: yaml
  label: GoToWebinar Polls API
  slug: gotowebinar-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-polls-api-openapi.yml
- filename: gotowebinar-questions-api-openapi.yml
  format: yaml
  label: GoToWebinar Questions API
  slug: gotowebinar-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-questions-api-openapi.yml
- filename: gotowebinar-recordings-api-openapi.yml
  format: yaml
  label: GoToWebinar Recordings API
  slug: gotowebinar-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-recordings-api-openapi.yml
- filename: gotowebinar-registrants-api-openapi.yml
  format: yaml
  label: GoToWebinar Registrants API
  slug: gotowebinar-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-registrants-api-openapi.yml
- filename: gotowebinar-sessions-api-openapi.yml
  format: yaml
  label: GoToWebinar Sessions API
  slug: gotowebinar-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-sessions-api-openapi.yml
- filename: gotowebinar-surveys-api-openapi.yml
  format: yaml
  label: GoToWebinar Surveys API
  slug: gotowebinar-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-surveys-api-openapi.yml
- filename: gotowebinar-user-subscriptions-api-openapi.yml
  format: yaml
  label: GoToWebinar User Subscriptions API
  slug: gotowebinar-user-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-user-subscriptions-api-openapi.yml
- filename: gotowebinar-webhooks-api-openapi.yml
  format: yaml
  label: GoToWebinar Webhooks API
  slug: gotowebinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webhooks-api-openapi.yml
- filename: gotowebinar-webinars-api-openapi.yml
  format: yaml
  label: GoToWebinar Webinars API
  slug: gotowebinar-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webinars-api-openapi.yml
authorization_urls:
- https://authentication.logmeininc.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Gotowebinar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GoToWebinar publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GoToWebinar API on a user''s behalf.


  Tokens are issued from https://authentication.logmeininc.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GoToWebinar
provider_slug: gotowebinar
schemes:
- description: OAuth 2.0 via the GoTo authentication service.
  flows:
  - authorizationUrl: https://authentication.logmeininc.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://authentication.logmeininc.com/oauth/token
  name: oauth2
  source: openapi/gotowebinar-rest-openapi.yml
- flows:
  - authorizationUrl: https://authentication.logmeininc.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://authentication.logmeininc.com/oauth/token
  name: oauth2
  source: openapi/gotowebinar-webhooks-openapi.yml
scope_count: 2
scope_names:
- collab
- identity:scim.me
scopes:
- description: Collaboration / GoToWebinar scope.
  flows:
  - authorizationCode
  scope: collab
- description: Read the authenticated user's identity (SCIM /me).
  flows:
  - authorizationCode
  scope: identity:scim.me
slug: gotowebinar-scopes
source_filename: gotowebinar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gotowebinar-rest-openapi.yml, openapi/gotowebinar-webhooks-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/gotowebinar-rest-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authentication.logmeininc.com/oauth/authorize\n    tokenUrl: https://authentication.logmeininc.com/oauth/token\n  description: OAuth 2.0 via the GoTo authentication service.\n- name: oauth2\n  source: openapi/gotowebinar-webhooks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authentication.logmeininc.com/oauth/authorize\n    tokenUrl: https://authentication.logmeininc.com/oauth/token\nscopes:\n- scope: collab\n  description: Collaboration / GoToWebinar scope.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gotowebinar-rest-openapi.yml\n  - openapi/gotowebinar-webhooks-openapi.yml\n- scope: identity:scim.me\n  description: Read the authenticated user's identity\
  \ (SCIM /me).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gotowebinar-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/scopes/gotowebinar-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Attendees
- Collaboration
- Communications
- Events
- Meetings
- Registrants
- Sessions
- Surveys
- Video Conferencing
- Virtual Events
- Webhooks
- Webinars
token_urls:
- https://authentication.logmeininc.com/oauth/token
---
