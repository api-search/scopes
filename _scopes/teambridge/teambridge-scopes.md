---
api_specs:
- filename: teambridge-openapi-original.json
  format: json
  label: Teambridge External API
  slug: teambridge-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teambridge/refs/heads/main/openapi/teambridge-openapi-original.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Teambridge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Teambridge publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Teambridge API on a user''s behalf.


  Tokens are issued from https://teambridge.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Teambridge
provider_slug: teambridge
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://teambridge.us.auth0.com/oauth/token
  name: OAuth2
  source: openapi/teambridge-openapi-original.json
scope_count: 1
scope_names:
- write
scopes:
- description: Full access
  flows:
  - clientCredentials
  scope: write
slug: teambridge-scopes
source_filename: teambridge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/teambridge-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/teambridge-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://teambridge.us.auth0.com/oauth/token\nscopes:\n- scope: write\n  description: Full access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/teambridge-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teambridge/refs/heads/main/scopes/teambridge-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Workforce Management
- Scheduling
- Time Tracking
- Payroll
- HR
- Frontline
- Webhooks
token_urls:
- https://teambridge.us.auth0.com/oauth/token
---
