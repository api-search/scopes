---
authorization_urls:
- https://developer.api.autodesk.com/authentication/v2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Autodesk Construction Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Autodesk Construction Cloud publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Autodesk Construction Cloud API on a user''s behalf.


  Tokens are issued from https://developer.api.autodesk.com/authentication/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Autodesk Construction Cloud
provider_slug: autodesk-construction-cloud
schemes:
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: oauth2ThreeLegged
  source: openapi/acc-admin-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: oauth2TwoLegged
  source: openapi/acc-admin-openapi.yml
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: oauth2ThreeLegged
  source: openapi/acc-issues-openapi.yml
scope_count: 4
scope_names:
- account:read
- account:write
- data:read
- data:write
scopes:
- description: Read account data
  flows:
  - authorizationCode
  - clientCredentials
  scope: account:read
- description: Modify account data
  flows:
  - authorizationCode
  scope: account:write
- description: Read project data
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:read
- description: Write project data
  flows:
  - authorizationCode
  scope: data:write
slug: autodesk-construction-cloud-scopes
source_filename: autodesk-construction-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acc-admin-openapi.yml, openapi/acc-issues-openapi.yml\nschemes:\n- name: oauth2ThreeLegged\n  source: openapi/acc-admin-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: oauth2TwoLegged\n  source: openapi/acc-admin-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: oauth2ThreeLegged\n  source: openapi/acc-issues-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\nscopes:\n- scope: account:read\n  description: Read account data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/acc-admin-openapi.yml\n\
  - scope: account:write\n  description: Modify account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/acc-admin-openapi.yml\n- scope: data:read\n  description: Read project data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/acc-admin-openapi.yml\n  - openapi/acc-issues-openapi.yml\n- scope: data:write\n  description: Write project data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/acc-admin-openapi.yml\n  - openapi/acc-issues-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/scopes/autodesk-construction-cloud-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Construction
- BIM
- Project Management
- AEC
- CAD
- Architecture
- Engineering
- Field Management
token_urls:
- https://developer.api.autodesk.com/authentication/v2/token
---
