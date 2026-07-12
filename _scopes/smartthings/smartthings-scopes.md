---
authorization_urls:
- https://api.smartthings.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Smartthings Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Samsung SmartThings publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Samsung SmartThings API on a user''s behalf.


  Tokens are issued from https://api.smartthings.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Samsung SmartThings
provider_slug: smartthings
schemes:
- description: OAuth 2.0 authorization code flow for production integrations.
  flows:
  - authorizationUrl: https://api.smartthings.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.smartthings.com/oauth/token
  name: oauth2
  source: openapi/smartthings-openapi.yml
scope_count: 8
scope_names:
- r:devices:*
- r:locations:*
- r:rules:*
- r:scenes:*
- w:locations:*
- w:rules:*
- x:devices:*
- x:scenes:*
scopes:
- description: Read devices
  flows:
  - authorizationCode
  scope: r:devices:*
- description: Read locations
  flows:
  - authorizationCode
  scope: r:locations:*
- description: Read rules
  flows:
  - authorizationCode
  scope: r:rules:*
- description: Read scenes
  flows:
  - authorizationCode
  scope: r:scenes:*
- description: Manage locations
  flows:
  - authorizationCode
  scope: w:locations:*
- description: Manage rules
  flows:
  - authorizationCode
  scope: w:rules:*
- description: Control devices
  flows:
  - authorizationCode
  scope: x:devices:*
- description: Execute scenes
  flows:
  - authorizationCode
  scope: x:scenes:*
slug: smartthings-scopes
source_filename: smartthings-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartthings-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/smartthings-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.smartthings.com/oauth/authorize\n    tokenUrl: https://api.smartthings.com/oauth/token\n  description: OAuth 2.0 authorization code flow for production integrations.\nscopes:\n- scope: r:devices:*\n  description: Read devices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartthings-openapi.yml\n- scope: r:locations:*\n  description: Read locations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartthings-openapi.yml\n- scope: r:rules:*\n  description: Read rules\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartthings-openapi.yml\n- scope: r:scenes:*\n  description: Read scenes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartthings-openapi.yml\n- scope: w:locations:*\n  description: Manage locations\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartthings-openapi.yml\n- scope: w:rules:*\n  description: Manage rules\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartthings-openapi.yml\n- scope: x:devices:*\n  description: Control devices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartthings-openapi.yml\n- scope: x:scenes:*\n  description: Execute scenes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/smartthings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/scopes/smartthings-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Smart Home
- IoT
- Home Automation
- Devices
- Samsung
token_urls:
- https://api.smartthings.com/oauth/token
---
