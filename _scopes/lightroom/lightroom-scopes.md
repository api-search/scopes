---
authorization_urls:
- https://ims-na1.adobelogin.com/ims/authorize/v2
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Lightroom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adobe Lightroom publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adobe Lightroom API on a user''s behalf.


  Tokens are issued from https://ims-na1.adobelogin.com/ims/token/v3.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Lightroom
provider_slug: lightroom
schemes:
- flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  source: openapi/lightroom-albums-openapi.yml
- flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  source: openapi/lightroom-assets-openapi.yml
- flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  source: openapi/lightroom-catalog-openapi.yml
- description: OAuth 2.0 via Adobe IMS for Firefly Services
  flows:
  - flow: clientCredentials
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  source: openapi/lightroom-firefly-services-openapi.yml
- description: OAuth 2.0 authorization code flow via Adobe Identity Management System (IMS). Partner applications must be registered in the Adobe Developer Console.
  flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  source: openapi/lightroom-services-openapi.yml
scope_count: 3
scope_names:
- firefly_api
- lr_partner_apis
- openid
scopes:
- description: Access Firefly Services APIs
  flows:
  - clientCredentials
  scope: firefly_api
- description: Access Lightroom partner APIs
  flows:
  - authorizationCode
  scope: lr_partner_apis
- description: OpenID Connect
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
slug: lightroom-scopes
source_filename: lightroom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lightroom-albums-openapi.yml, openapi/lightroom-assets-openapi.yml, openapi/lightroom-catalog-openapi.yml,\n  openapi/lightroom-firefly-services-openapi.yml, openapi/lightroom-services-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/lightroom-albums-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n- name: oauth2\n  source: openapi/lightroom-assets-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n- name: oauth2\n  source: openapi/lightroom-catalog-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n- name: oauth2\n  source:\
  \ openapi/lightroom-firefly-services-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n  description: OAuth 2.0 via Adobe IMS for Firefly Services\n- name: oauth2\n  source: openapi/lightroom-services-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n  description: OAuth 2.0 authorization code flow via Adobe Identity Management System (IMS).\n    Partner applications must be registered in the Adobe Developer Console.\nscopes:\n- scope: firefly_api\n  description: Access Firefly Services APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lightroom-firefly-services-openapi.yml\n- scope: lr_partner_apis\n  description: Access Lightroom partner APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightroom-albums-openapi.yml\n  - openapi/lightroom-assets-openapi.yml\n  - openapi/lightroom-catalog-openapi.yml\n\
  \  - openapi/lightroom-services-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/lightroom-firefly-services-openapi.yml\n  - openapi/lightroom-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/scopes/lightroom-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
token_urls:
- https://ims-na1.adobelogin.com/ims/token/v3
---
