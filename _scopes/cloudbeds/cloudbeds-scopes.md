---
authorization_urls:
- https://hotels.cloudbeds.com/api/v1.2/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cloudbeds Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cloudbeds publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cloudbeds API on a user''s behalf.


  Tokens are issued from https://hotels.cloudbeds.com/api/v1.2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cloudbeds
provider_slug: cloudbeds
schemes:
- flows:
  - authorizationUrl: https://hotels.cloudbeds.com/api/v1.2/oauth
    flow: authorizationCode
    tokenUrl: https://hotels.cloudbeds.com/api/v1.2/access_token
  name: oauth2
  source: openapi/cloudbeds-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access
  flows:
  - authorizationCode
  scope: read
- description: Write access
  flows:
  - authorizationCode
  scope: write
slug: cloudbeds-scopes
source_filename: cloudbeds-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudbeds-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cloudbeds-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hotels.cloudbeds.com/api/v1.2/oauth\n    tokenUrl: https://hotels.cloudbeds.com/api/v1.2/access_token\nscopes:\n- scope: read\n  description: Read access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloudbeds-openapi.yml\n- scope: write\n  description: Write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cloudbeds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudbeds/refs/heads/main/scopes/cloudbeds-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Hospitality
- Hotels
- PMS
- Property Management
- Channel Manager
- Booking Engine
- Payments
token_urls:
- https://hotels.cloudbeds.com/api/v1.2/access_token
---
