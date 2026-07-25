---
api_specs:
- filename: goto-webinar-attendees-api-openapi.yml
  format: yaml
  label: GoTo Webinar Attendees API
  slug: goto-webinar-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-attendees-api-openapi.yml
- filename: goto-webinar-panelists-api-openapi.yml
  format: yaml
  label: GoTo Webinar Panelists API
  slug: goto-webinar-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-panelists-api-openapi.yml
- filename: goto-webinar-polls-api-openapi.yml
  format: yaml
  label: GoTo Webinar Polls API
  slug: goto-webinar-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-polls-api-openapi.yml
- filename: goto-webinar-questions-api-openapi.yml
  format: yaml
  label: GoTo Webinar Questions API
  slug: goto-webinar-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-questions-api-openapi.yml
- filename: goto-webinar-registrants-api-openapi.yml
  format: yaml
  label: GoTo Webinar Registrants API
  slug: goto-webinar-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-registrants-api-openapi.yml
- filename: goto-webinar-sessions-api-openapi.yml
  format: yaml
  label: GoTo Webinar Sessions API
  slug: goto-webinar-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-sessions-api-openapi.yml
- filename: goto-webinar-webinars-api-openapi.yml
  format: yaml
  label: GoTo Webinar Webinars API
  slug: goto-webinar-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-webinars-api-openapi.yml
authorization_urls:
- https://authentication.logmeininc.com/oauth/authorize
description: ''
docs: https://developer.goto.com/GoToWebinarV2
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Goto Webinar Scopes
name_suffix: OAuth Scopes
note: GoTo Webinar does not publish a granular per-endpoint scope catalog; the v2 API reference documents a single product-level scope (`collab:`) required when requesting a token, with additional scopes selected per OAuth client in the GoTo developer portal (https://developer.goto.com/GoToWebinarV2).
overview: 'GoTo Webinar publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GoTo Webinar API on a user''s behalf.


  Tokens are issued from https://authentication.logmeininc.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GoTo Webinar
provider_slug: goto-webinar
schemes:
- flows:
  - authorizationUrl: https://authentication.logmeininc.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://authentication.logmeininc.com/oauth/token
  name: oauth2
  source: openapi/goto-webinar-openapi.yml
scope_count: 1
scope_names:
- 'collab:'
scopes:
- description: Grants access to the GoTo Webinar (collaboration) APIs. The GoTo Webinar v2 API reference states this scope must be used when a token is requested from the Authentication API.
  flows: []
  scope: 'collab:'
slug: goto-webinar-scopes
source_filename: goto-webinar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/goto-webinar-openapi.yml\ndocs: https://developer.goto.com/GoToWebinarV2\nschemes:\n- name: oauth2\n  source: openapi/goto-webinar-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authentication.logmeininc.com/oauth/authorize\n    tokenUrl: https://authentication.logmeininc.com/oauth/token\nscopes:\n- scope: 'collab:'\n  description: >-\n    Grants access to the GoTo Webinar (collaboration) APIs. The GoTo Webinar\n    v2 API reference states this scope must be used when a token is requested\n    from the Authentication API.\n  sources:\n  - https://developer.goto.com/GoToWebinarV2\nnote: >-\n  GoTo Webinar does not publish a granular per-endpoint scope catalog; the v2\n  API reference documents a single product-level scope (`collab:`) required\n  when requesting a token, with additional scopes selected per OAuth client in\n  the GoTo developer portal (https://developer.goto.com/GoToWebinarV2).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/scopes/goto-webinar-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Webinars
- Virtual Events
- Video Conferencing
- Marketing
- Lead Capture
- Registration
token_urls:
- https://authentication.logmeininc.com/oauth/token
---
