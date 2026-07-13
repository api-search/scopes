---
api_specs:
- filename: dexcom-dexcom-api.yml
  format: yaml
  label: Dexcom Developer API
  slug: dexcom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-dexcom-api.yml
authorization_urls:
- https://api.dexcom.com/v2/oauth2/login
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Dexcom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dexcom publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dexcom API on a user''s behalf.


  Tokens are issued from https://api.dexcom.com/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dexcom
provider_slug: dexcom
schemes:
- description: Dexcom uses OAuth 2.0 authorization code flow. The only acceptable scope value is `offline_access`.
  flows:
  - authorizationUrl: https://api.dexcom.com/v2/oauth2/login
    flow: authorizationCode
    tokenUrl: https://api.dexcom.com/v2/oauth2/token
  name: OAuth2
  source: openapi/dexcom-dexcom-api.yml
scope_count: 1
scope_names:
- offline_access
scopes:
- description: Long-lived access to the user's CGM data via refresh tokens.
  flows:
  - authorizationCode
  scope: offline_access
slug: dexcom-scopes
source_filename: dexcom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dexcom-dexcom-api.yml\nschemes:\n- name: OAuth2\n  source: openapi/dexcom-dexcom-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.dexcom.com/v2/oauth2/login\n    tokenUrl: https://api.dexcom.com/v2/oauth2/token\n  description: Dexcom uses OAuth 2.0 authorization code flow. The only acceptable scope value\n    is `offline_access`.\nscopes:\n- scope: offline_access\n  description: Long-lived access to the user's CGM data via refresh tokens.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dexcom-dexcom-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/scopes/dexcom-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Continuous Glucose Monitoring
- Diabetes
- Digital Health
- Glucose
- Healthcare
- Medical Devices
- Wearables
token_urls:
- https://api.dexcom.com/v2/oauth2/token
---
