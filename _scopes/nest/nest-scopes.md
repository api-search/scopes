---
authorization_urls:
- https://nestservices.google.com/partnerconnections/{project-id}/auth
description: ''
docs: https://developers.google.com/nest/device-access/authorize
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nest Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nest publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nest API on a user''s behalf.


  Tokens are issued from https://www.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nest
provider_slug: nest
schemes:
- flows:
  - authorizationUrl: https://nestservices.google.com/partnerconnections/{project-id}/auth
    flow: authorizationCode
    tokenUrl: https://www.googleapis.com/token
  name: GoogleOAuth2
  source: https://developers.google.com/nest/device-access/authorize
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/sdm.service
scopes:
- description: Single coarse-grained scope granting the Smart Device Management API access to view, control, and manage the Nest devices the user has authorized for the Device Access project. Per-device and per-trait consent is chosen by the end user in the Partner Connections Manager flow rather than through additional OAuth scopes.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/sdm.service
slug: nest-scopes
source_filename: nest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.google.com/nest/device-access/authorize\ndocs: https://developers.google.com/nest/device-access/authorize\nschemes:\n  - name: GoogleOAuth2\n    source: https://developers.google.com/nest/device-access/authorize\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://nestservices.google.com/partnerconnections/{project-id}/auth\n        tokenUrl: https://www.googleapis.com/token\nscopes:\n  - scope: https://www.googleapis.com/auth/sdm.service\n    description: >-\n      Single coarse-grained scope granting the Smart Device Management API access\n      to view, control, and manage the Nest devices the user has authorized for\n      the Device Access project. Per-device and per-trait consent is chosen by the\n      end user in the Partner Connections Manager flow rather than through\n      additional OAuth scopes.\n    flows: [authorizationCode]\n    sources: [https://developers.google.com/nest/device-access/authorize]\n\
  notes: >-\n  The SDM API exposes exactly one OAuth scope. Granular authorization is expressed\n  through the device/trait selections the user makes at consent time, not through\n  a scope hierarchy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nest/refs/heads/main/scopes/nest-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Hardware
- Smart Home
- IoT
- Home Automation
- Thermostat
- Google
- Device Access
token_urls:
- https://www.googleapis.com/token
---
