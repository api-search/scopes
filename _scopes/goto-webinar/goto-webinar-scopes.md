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
- filename: goto-webinar-co-organizers-api-openapi.yml
  format: yaml
  label: GoTo Webinar Co Organizers API
  slug: goto-webinar-co-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-co-organizers-api-openapi.yml
- filename: goto-webinar-recordingassets-api-openapi.yml
  format: yaml
  label: GoTo Webinar Recording Assets API
  slug: goto-webinar-recordingassets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-recordingassets-api-openapi.yml
- filename: goto-webinar-webhooks-api-openapi.yml
  format: yaml
  label: GoTo Webinar Webhooks API
  slug: goto-webinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-webhooks-api-openapi.yml
authorization_urls:
- https://identity.goto.com/oauth/authorize
description: ''
docs: https://developer.goto.com/GoToWebinarV2
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: searched
name: Goto Webinar Scopes
name_suffix: OAuth Scopes
note: GoTo Webinar has no granular scope surface. The OpenAPI declares an oauth2 scheme with an EMPTY scopes map on both flows, and no operation names a scope in its security requirement — the whole 53-operation API is guarded by one product-level scope. Additional product scopes are selected per OAuth client in the GoTo developer portal (https://developer.logmeininc.com/clients), not requested per token. The RFC 8414 authorization-server metadata at identity.goto.com does not advertise a scopes_supported array either.
overview: 'GoTo Webinar publishes 1 OAuth 2.0 scope via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the GoTo Webinar API on a user''s behalf.


  Tokens are issued from https://identity.goto.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GoTo Webinar
provider_slug: goto-webinar
schemes:
- flows:
  - authorizationUrl: https://identity.goto.com/oauth/authorize
    flow: authorizationCode
    spec_declares_host: https://authentication.logmeininc.com
    tokenUrl: https://identity.goto.com/oauth/token
  - deprecated: true
    flow: password
    tokenUrl: https://identity.goto.com/oauth/token
  name: OAuth2
  source: openapi/_original/goto-webinar-openapi.yml
scope_count: 1
scope_names:
- 'collab:'
scopes:
- description: Grants access to the GoTo Webinar (collaboration) APIs. The GoTo Webinar v2 API reference states under "Authentication Scopes" that "`collab:` must be used when a token is requested from the Authentication API."
  flows:
  - authorizationCode
  scope: 'collab:'
slug: goto-webinar-scopes
source_filename: goto-webinar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/goto-webinar-openapi.yml\ndocs: https://developer.goto.com/GoToWebinarV2\nmetadata_document: https://identity.goto.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: openapi/_original/goto-webinar-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.goto.com/oauth/authorize\n    tokenUrl: https://identity.goto.com/oauth/token\n    spec_declares_host: https://authentication.logmeininc.com\n  - flow: password\n    tokenUrl: https://identity.goto.com/oauth/token\n    deprecated: true\nscopes:\n- scope: 'collab:'\n  description: >-\n    Grants access to the GoTo Webinar (collaboration) APIs. The GoTo Webinar v2\n    API reference states under \"Authentication Scopes\" that \"`collab:` must be\n    used when a token is requested from the Authentication API.\"\n  flows: [authorizationCode]\n  sources:\n  - https://developer.goto.com/GoToWebinarV2\n\
  scope_count: 1\nscopes_declared_in_spec: 0\nnote: >-\n  GoTo Webinar has no granular scope surface. The OpenAPI declares an oauth2\n  scheme with an EMPTY scopes map on both flows, and no operation names a scope\n  in its security requirement — the whole 53-operation API is guarded by one\n  product-level scope. Additional product scopes are selected per OAuth client\n  in the GoTo developer portal (https://developer.logmeininc.com/clients), not\n  requested per token. The RFC 8414 authorization-server metadata at\n  identity.goto.com does not advertise a scopes_supported array either.\nconsequence: >-\n  A token that can read attendee reports can also cancel webinars, delete\n  registrants and rewrite webhook callbacks. There is no read-only token and no\n  way to least-privilege an agent — the only privilege boundary available is\n  the organizer seat the token authenticates as. This is the single largest\n  authorization gap in GoTo Webinar's agent surface, and closing it would need\n\
  \  a per-resource scope catalogue GoTo does not currently publish.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/scopes/goto-webinar-scopes.yml
summary_line: 1 scope · authorizationCode/password
tags:
- Webinars
- Virtual Events
- Video Conferencing
- Marketing
- Lead Capture
- Registration
- Webhook
- Event Management
- Collaboration
- Analytics
token_urls:
- https://identity.goto.com/oauth/token
---
