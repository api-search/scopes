---
api_specs:
- filename: aps-sdk-openapi
  format: yaml
  label: Autodesk Fusion API
  slug: autodesk-fusion-api
  spec_type: OpenAPI
  url: https://github.com/autodesk-platform-services/aps-sdk-openapi
authorization_urls:
- https://developer.api.autodesk.com/authentication/v2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- implicit
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Autodesk Fusion Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Autodesk Fusion publishes 14 OAuth 2.0 scopes via the clientCredentials, implicit, and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Autodesk Fusion API on a user''s behalf.


  Tokens are issued from https://developer.api.autodesk.com/authentication/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Autodesk Fusion
provider_slug: autodesk-fusion
schemes:
- flows:
  - flow: clientCredentials
  name: 2-legged
  source: openapi/accountadmin.yaml
- flows:
  - flow: implicit
  name: 3-legged-implicit
  source: openapi/accountadmin.yaml
- flows:
  - flow: authorizationCode
  name: 3-legged
  source: openapi/accountadmin.yaml
- description: User context required.
  flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 3-legged
  source: openapi/authentication.yaml
- description: Application context required.
  flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 2-legged
  source: openapi/authentication.yaml
- description: User context required.
  flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 3-legged
  source: openapi/datamanagement.yaml
- description: Application context required.
  flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 2-legged
  source: openapi/datamanagement.yaml
- flows:
  - flow: clientCredentials
  name: 2-legged
  source: openapi/issues.yaml
- flows:
  - flow: authorizationCode
  name: 3-legged
  source: openapi/issues.yaml
- flows:
  - flow: implicit
  name: 3-legged-implicit
  source: openapi/issues.yaml
- description: User context required.
  flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 3-legged
  source: openapi/modelderivative.yaml
- description: Application context required.
  flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 2-legged
  source: openapi/modelderivative.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authentication/v1/authenticate
  name: oauth2_application
  source: openapi/oss.yaml
- description: User context required.
  flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 3-legged
  source: openapi/oss.yaml
- description: Application context required.
  flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 2-legged
  source: openapi/oss.yaml
- description: Application context required.
  flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 2-legged
  source: openapi/secureserviceaccount.yaml
- description: User context required.
  flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 3-legged
  source: openapi/webhooks.yaml
- description: Application context required.
  flows:
  - flow: clientCredentials
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: 2-legged
  source: openapi/webhooks.yaml
scope_count: 14
scope_names:
- application:service_account:read
- application:service_account:write
- application:service_account_key:read
- application:service_account_key:write
- bucket:create
- bucket:delete
- bucket:read
- bucket:update
- data:create
- data:read
- data:search
- data:write
- viewable:read
- viewables:read
scopes:
- description: Grant read access to Service Accounts
  flows:
  - clientCredentials
  scope: application:service_account:read
- description: Grant write access to Service Accounts
  flows:
  - clientCredentials
  scope: application:service_account:write
- description: Grant read access to Service Account Keys
  flows:
  - clientCredentials
  scope: application:service_account_key:read
- description: Grant write access to Service Account Keys
  flows:
  - clientCredentials
  scope: application:service_account_key:write
- description: The application will be able to create an OSS bucket it will own.
  flows:
  - clientCredentials
  scope: bucket:create
- description: The application will be able to delete an OSS bucket it will own.
  flows:
  - clientCredentials
  scope: bucket:delete
- description: The application will be able to read the metadata and list contents for OSS buckets that it has access to.
  flows:
  - clientCredentials
  scope: bucket:read
- description: The application will be able to set permissions and entitlements for OSS buckets that it has permission to modify.
  flows:
  - clientCredentials
  scope: bucket:update
- description: create new data
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:create
- description: read your data
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:read
- description: ''
  flows: []
  scope: data:search
- description: modify your data
  flows:
  - authorizationCode
  - clientCredentials
  scope: data:write
- description: ''
  flows: []
  scope: viewable:read
- description: ''
  flows: []
  scope: viewables:read
slug: autodesk-fusion-scopes
source_filename: autodesk-fusion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accountadmin.yaml, openapi/authentication.yaml, openapi/datamanagement.yaml,\n  openapi/issues.yaml, openapi/modelderivative.yaml, openapi/oss.yaml, openapi/secureserviceaccount.yaml,\n  openapi/webhooks.yaml\nschemes:\n- name: 2-legged\n  source: openapi/accountadmin.yaml\n  flows:\n  - flow: clientCredentials\n- name: 3-legged-implicit\n  source: openapi/accountadmin.yaml\n  flows:\n  - flow: implicit\n- name: 3-legged\n  source: openapi/accountadmin.yaml\n  flows:\n  - flow: authorizationCode\n- name: 3-legged\n  source: openapi/authentication.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: User context required.\n- name: 2-legged\n  source: openapi/authentication.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n\
  \  description: Application context required.\n- name: 3-legged\n  source: openapi/datamanagement.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: User context required.\n- name: 2-legged\n  source: openapi/datamanagement.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: Application context required.\n- name: 2-legged\n  source: openapi/issues.yaml\n  flows:\n  - flow: clientCredentials\n- name: 3-legged\n  source: openapi/issues.yaml\n  flows:\n  - flow: authorizationCode\n- name: 3-legged-implicit\n  source: openapi/issues.yaml\n  flows:\n  - flow: implicit\n- name: 3-legged\n  source: openapi/modelderivative.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n\
  \    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: User context required.\n- name: 2-legged\n  source: openapi/modelderivative.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: Application context required.\n- name: oauth2_application\n  source: openapi/oss.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authentication/v1/authenticate\n- name: 3-legged\n  source: openapi/oss.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: User context required.\n- name: 2-legged\n  source: openapi/oss.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: Application context required.\n- name: 2-legged\n  source: openapi/secureserviceaccount.yaml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: Application context required.\n- name: 3-legged\n  source: openapi/webhooks.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: User context required.\n- name: 2-legged\n  source: openapi/webhooks.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n  description: Application context required.\nscopes:\n- scope: application:service_account:read\n  description: Grant read access to Service Accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/secureserviceaccount.yaml\n- scope: application:service_account:write\n  description: Grant write access to Service Accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/secureserviceaccount.yaml\n\
  - scope: application:service_account_key:read\n  description: Grant read access to Service Account Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/secureserviceaccount.yaml\n- scope: application:service_account_key:write\n  description: Grant write access to Service Account Keys\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/secureserviceaccount.yaml\n- scope: bucket:create\n  description: The application will be able to create an OSS bucket it will own.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oss.yaml\n- scope: bucket:delete\n  description: The application will be able to delete an OSS bucket it will own.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oss.yaml\n- scope: bucket:read\n  description: The application will be able to read the metadata and list contents for OSS buckets\n    that it has access to.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oss.yaml\n- scope: bucket:update\n  description: The application will\
  \ be able to set permissions and entitlements for OSS buckets\n    that it has permission to modify.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oss.yaml\n- scope: data:create\n  description: create new data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/authentication.yaml\n  - openapi/datamanagement.yaml\n  - openapi/modelderivative.yaml\n  - openapi/oss.yaml\n  - openapi/webhooks.yaml\n- scope: data:read\n  description: read your data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/authentication.yaml\n  - openapi/datamanagement.yaml\n  - openapi/modelderivative.yaml\n  - openapi/oss.yaml\n  - openapi/webhooks.yaml\n- scope: data:search\n  sources:\n  - openapi/datamanagement.yaml\n- scope: data:write\n  description: modify your data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/authentication.yaml\n  - openapi/datamanagement.yaml\n  - openapi/modelderivative.yaml\n  -\
  \ openapi/oss.yaml\n  - openapi/webhooks.yaml\n- scope: viewable:read\n  sources:\n  - openapi/modelderivative.yaml\n- scope: viewables:read\n  sources:\n  - openapi/oss.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-fusion/refs/heads/main/scopes/autodesk-fusion-scopes.yml
summary_line: 14 scopes · clientCredentials/implicit/authorizationCode
tags:
- CAD
- CAM
- CAE
- Manufacturing
- Design Automation
- GraphQL
- REST
- Autodesk Platform Services
token_urls:
- https://developer.api.autodesk.com/authentication/v2/token
- /authentication/v1/authenticate
---
