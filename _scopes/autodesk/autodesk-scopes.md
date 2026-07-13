---
api_specs:
- filename: autodesk-authentication-openapi.yml
  format: yaml
  label: Autodesk Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-authentication-openapi.yml
- filename: autodesk-data-management-openapi.yml
  format: yaml
  label: Autodesk Data Management API
  slug: data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-data-management-openapi.yml
- filename: autodesk-model-derivative-openapi.yml
  format: yaml
  label: Autodesk Model Derivative API
  slug: model-derivative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-model-derivative-openapi.yml
- filename: autodesk-design-automation-openapi.yml
  format: yaml
  label: Autodesk Design Automation API
  slug: design-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-design-automation-openapi.yml
- filename: autodesk-webhooks-openapi.yml
  format: yaml
  label: Autodesk Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-webhooks-openapi.yml
- filename: autodesk-reality-capture-openapi.yml
  format: yaml
  label: Autodesk Reality Capture API
  slug: reality-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-reality-capture-openapi.yml
- filename: autodesk-sustainability-data-openapi.yml
  format: yaml
  label: Autodesk Sustainability Data API
  slug: sustainability-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-sustainability-data-openapi.yml
- filename: autodesk-parameters-openapi.yml
  format: yaml
  label: Autodesk Parameters API
  slug: parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-parameters-openapi.yml
- filename: autodesk-tandem-data-openapi.yml
  format: yaml
  label: Autodesk Tandem Data API
  slug: tandem-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-tandem-data-openapi.yml
- filename: autodesk-flow-graph-engine-openapi.yml
  format: yaml
  label: Autodesk Flow Graph Engine API
  slug: flow-graph-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-flow-graph-engine-openapi.yml
- filename: autodesk-acc-account-admin-openapi.yml
  format: yaml
  label: Autodesk ACC Account Admin API
  slug: acc-account-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-acc-account-admin-openapi.yml
- filename: autodesk-bim360-openapi.yml
  format: yaml
  label: Autodesk BIM 360 API
  slug: bim-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-bim360-openapi.yml
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
name: Autodesk Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Autodesk publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Autodesk API on a user''s behalf.


  Tokens are issued from https://developer.api.autodesk.com/authentication/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Autodesk
provider_slug: autodesk
schemes:
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  source: openapi/autodesk-acc-account-admin-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  source: openapi/autodesk-authentication-openapi.yml
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  source: openapi/autodesk-authentication-openapi.yml
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  source: openapi/autodesk-bim360-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  source: openapi/autodesk-data-management-openapi.yml
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  source: openapi/autodesk-data-management-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  source: openapi/autodesk-design-automation-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  source: openapi/autodesk-flow-graph-engine-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  source: openapi/autodesk-model-derivative-openapi.yml
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  source: openapi/autodesk-model-derivative-openapi.yml
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  source: openapi/autodesk-parameters-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  source: openapi/autodesk-reality-capture-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  source: openapi/autodesk-sustainability-data-openapi.yml
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  source: openapi/autodesk-tandem-data-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  source: openapi/autodesk-webhooks-openapi.yml
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  source: openapi/autodesk-webhooks-openapi.yml
scope_count: 12
scope_names:
- account:read
- account:write
- bucket:create
- bucket:delete
- bucket:read
- bucket:update
- code:all
- data:create
- data:read
- data:search
- data:write
- user-profile:read
scopes:
- description: Read account data
  flows:
  - authorizationCode
  - clientCredentials
  scope: account:read
- description: Write account data
  flows:
  - authorizationCode
  - clientCredentials
  scope: account:write
- description: Create OSS buckets
  flows:
  - clientCredentials
  scope: bucket:create
- description: Delete OSS buckets
  flows:
  - clientCredentials
  scope: bucket:delete
- description: Read OSS buckets
  flows:
  - clientCredentials
  scope: bucket:read
- description: Update OSS buckets
  flows:
  - clientCredentials
  scope: bucket:update
- description: Execute Design Automation activities
  flows:
  - clientCredentials
  scope: code:all
- description: Create new data
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:create
- description: Read access to data
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:read
- description: Search data
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:search
- description: Write access to data
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:write
- description: Read user profile
  flows:
  - authorizationCode
  scope: user-profile:read
slug: autodesk-scopes
source_filename: autodesk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/autodesk-acc-account-admin-openapi.yml, openapi/autodesk-authentication-openapi.yml,\n  openapi/autodesk-bim360-openapi.yml, openapi/autodesk-data-management-openapi.yml, openapi/autodesk-design-automation-openapi.yml,\n  openapi/autodesk-flow-graph-engine-openapi.yml, openapi/autodesk-model-derivative-openapi.yml,\n  openapi/autodesk-parameters-openapi.yml, openapi/autodesk-reality-capture-openapi.yml, openapi/autodesk-sustainability-data-openapi.yml,\n  openapi/autodesk-tandem-data-openapi.yml, openapi/autodesk-webhooks-openapi.yml\nschemes:\n- name: OAuth2ThreeLegged\n  source: openapi/autodesk-acc-account-admin-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2TwoLegged\n  source: openapi/autodesk-authentication-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2ThreeLegged\n  source: openapi/autodesk-authentication-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2ThreeLegged\n  source: openapi/autodesk-bim360-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2TwoLegged\n  source: openapi/autodesk-data-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2ThreeLegged\n  source: openapi/autodesk-data-management-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n\
  \    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2TwoLegged\n  source: openapi/autodesk-design-automation-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2TwoLegged\n  source: openapi/autodesk-flow-graph-engine-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2TwoLegged\n  source: openapi/autodesk-model-derivative-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2ThreeLegged\n  source: openapi/autodesk-model-derivative-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2ThreeLegged\n  source: openapi/autodesk-parameters-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2TwoLegged\n  source: openapi/autodesk-reality-capture-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2TwoLegged\n  source: openapi/autodesk-sustainability-data-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2ThreeLegged\n  source: openapi/autodesk-tandem-data-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n- name: OAuth2TwoLegged\n  source: openapi/autodesk-webhooks-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n\
  - name: OAuth2ThreeLegged\n  source: openapi/autodesk-webhooks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\nscopes:\n- scope: account:read\n  description: Read account data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/autodesk-acc-account-admin-openapi.yml\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-bim360-openapi.yml\n- scope: account:write\n  description: Write account data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/autodesk-acc-account-admin-openapi.yml\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-bim360-openapi.yml\n- scope: bucket:create\n  description: Create OSS buckets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n\
  - scope: bucket:delete\n  description: Delete OSS buckets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n- scope: bucket:read\n  description: Read OSS buckets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n- scope: bucket:update\n  description: Update OSS buckets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n- scope: code:all\n  description: Execute Design Automation activities\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-design-automation-openapi.yml\n  - openapi/autodesk-flow-graph-engine-openapi.yml\n- scope: data:create\n  description: Create new data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  -\
  \ openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n  - openapi/autodesk-model-derivative-openapi.yml\n  - openapi/autodesk-reality-capture-openapi.yml\n- scope: data:read\n  description: Read access to data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-bim360-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n  - openapi/autodesk-model-derivative-openapi.yml\n  - openapi/autodesk-parameters-openapi.yml\n  - openapi/autodesk-reality-capture-openapi.yml\n  - openapi/autodesk-sustainability-data-openapi.yml\n  - openapi/autodesk-tandem-data-openapi.yml\n  - openapi/autodesk-webhooks-openapi.yml\n- scope: data:search\n  description: Search data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n- scope: data:write\n  description:\
  \ Write access to data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-bim360-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n  - openapi/autodesk-model-derivative-openapi.yml\n  - openapi/autodesk-parameters-openapi.yml\n  - openapi/autodesk-reality-capture-openapi.yml\n  - openapi/autodesk-tandem-data-openapi.yml\n  - openapi/autodesk-webhooks-openapi.yml\n- scope: user-profile:read\n  description: Read user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/scopes/autodesk-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Fortune 1000
- 3D Modeling
- Architecture
- BIM
- CAD
- Construction
- Design
- Digital Twins
- Engineering
- Manufacturing
- Media and Entertainment
- Sustainability
token_urls:
- https://developer.api.autodesk.com/authentication/v2/token
---
