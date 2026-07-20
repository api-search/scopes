---
api_specs:
- filename: automile-openapi-original.json
  format: json
  label: Automile API
  slug: automile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automile/refs/heads/main/openapi/automile-openapi-original.json
authorization_urls:
- https://api.automile.com/login/
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Automile Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Automile publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Automile API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Automile
provider_slug: automile
schemes:
- description: OAuth2 Implicit Grant
  flows:
  - authorizationUrl: https://api.automile.com/login/
    flow: implicit
  name: oauth2
  source: openapi/automile-openapi-original.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to protected resources
  flows:
  - implicit
  scope: read
- description: Write access to protected resources
  flows:
  - implicit
  scope: write
slug: automile-scopes
source_filename: automile-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/automile-openapi-original.json\nschemes:\n- name: oauth2\n  source: openapi/automile-openapi-original.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.automile.com/login/\n  description: OAuth2 Implicit Grant\nscopes:\n- scope: read\n  description: Read access to protected resources\n  flows:\n  - implicit\n  sources:\n  - openapi/automile-openapi-original.json\n- scope: write\n  description: Write access to protected resources\n  flows:\n  - implicit\n  sources:\n  - openapi/automile-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automile/refs/heads/main/scopes/automile-scopes.yml
summary_line: 2 scopes · implicit
tags:
- Fleet Management
- Telematics
- GPS Tracking
- Vehicles
- Transportation
- Mileage
- IoT
- Logistics
- Company
token_urls: []
---
