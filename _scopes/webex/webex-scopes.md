---
authorization_urls:
- /
- https://webexapis.com/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Webex Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Webex publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Webex API on a user''s behalf.


  Tokens are issued from /.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Webex
provider_slug: webex
schemes:
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-admin-openapi.json
- description: OAuth 2.0 Bearer token authentication
  flows:
  - authorizationUrl: https://webexapis.com/v1/authorize
    flow: authorizationCode
    tokenUrl: https://webexapis.com/v1/access_token
  name: bearerAuth
  source: openapi/webex-admin-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-broadworks-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-cloud-calling-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-contact-center-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-device-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-meeting-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-messaging-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-ucm-openapi.json
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    tokenUrl: /
  name: oauth2
  source: openapi/webex-wholesale-openapi.json
scope_count: 1
scope_names:
- spark:applications_token
scopes:
- description: Create access tokens for Service Apps
  flows:
  - authorizationCode
  scope: spark:applications_token
slug: webex-scopes
source_filename: webex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/webex-admin-openapi.json, openapi/webex-broadworks-openapi.json, openapi/webex-cloud-calling-openapi.json,\n  openapi/webex-contact-center-openapi.json, openapi/webex-device-openapi.json, openapi/webex-meeting-openapi.json,\n  openapi/webex-messaging-openapi.json, openapi/webex-ucm-openapi.json, openapi/webex-wholesale-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/webex-admin-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: bearerAuth\n  source: openapi/webex-admin-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://webexapis.com/v1/authorize\n    tokenUrl: https://webexapis.com/v1/access_token\n  description: OAuth 2.0 Bearer token authentication\n- name: oauth2\n  source: openapi/webex-broadworks-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: oauth2\n  source: openapi/webex-cloud-calling-openapi.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: oauth2\n  source: openapi/webex-contact-center-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: oauth2\n  source: openapi/webex-device-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: oauth2\n  source: openapi/webex-meeting-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: oauth2\n  source: openapi/webex-messaging-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: oauth2\n  source: openapi/webex-ucm-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n- name: oauth2\n  source: openapi/webex-wholesale-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\nscopes:\n- scope: spark:applications_token\n  description:\
  \ Create access tokens for Service Apps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webex-admin-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/scopes/webex-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Calling
- Collaboration
- Communication
- Enterprise
- Messaging
- Video Conferencing
token_urls:
- /
- https://webexapis.com/v1/access_token
---
