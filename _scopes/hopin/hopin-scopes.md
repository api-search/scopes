---
api_specs:
- filename: openapi.json
  format: json
  label: RingCentral Events API
  slug: ringcentral-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hopin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RingCentral Events publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RingCentral Events API on a user''s behalf.


  Tokens are issued from https://api.events.ringcentral.com/v1/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RingCentral Events
provider_slug: hopin
schemes:
- description: OAuth 2.0 Client Credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.events.ringcentral.com/v1/auth/token
  name: oauth2
  source: openapi/openapi.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to resources
  flows:
  - clientCredentials
  scope: read
- description: Write access to resources
  flows:
  - clientCredentials
  scope: write
slug: hopin-scopes
source_filename: hopin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nschemes:\n- name: oauth2\n  source: openapi/openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.events.ringcentral.com/v1/auth/token\n  description: OAuth 2.0 Client Credentials flow\nscopes:\n- scope: read\n  description: Read access to resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openapi.json\n- scope: write\n  description: Write access to resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/scopes/hopin-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Events
- Virtual Events
- Hybrid Events
- Webinars
- Event Management
- Registration
- Sessions
- Networking
token_urls:
- https://api.events.ringcentral.com/v1/auth/token
---
