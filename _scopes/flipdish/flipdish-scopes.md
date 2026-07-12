---
authorization_urls:
- https://api.flipdish.co/identity/connect/authorize
description: ''
docs: ''
flows:
- implicit
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Flipdish Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flipdish publishes 1 OAuth 2.0 scope via the implicit and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flipdish API on a user''s behalf.


  Tokens are issued from https://api.flipdish.co/identity/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flipdish
provider_slug: flipdish
schemes:
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-apps-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-catalog-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-customers-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-devices-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-marketing-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-menus-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-orders-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-payments-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-platform-openapi.json
- description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access token).
  flows:
  - authorizationUrl: https://api.flipdish.co/identity/connect/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://api.flipdish.co/identity/connect/token
  name: oauth2
  source: openapi/flipdish-stores-openapi.json
scope_count: 1
scope_names:
- api
scopes:
- description: Access to the Flipdish API
  flows:
  - clientCredentials
  - implicit
  scope: api
slug: flipdish-scopes
source_filename: flipdish-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flipdish-apps-openapi.json, openapi/flipdish-catalog-openapi.json, openapi/flipdish-customers-openapi.json,\n  openapi/flipdish-devices-openapi.json, openapi/flipdish-marketing-openapi.json, openapi/flipdish-menus-openapi.json,\n  openapi/flipdish-orders-openapi.json, openapi/flipdish-payments-openapi.json, openapi/flipdish-platform-openapi.json,\n  openapi/flipdish-stores-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/flipdish-apps-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-catalog-openapi.json\n  flows:\n\
  \  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-customers-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-devices-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n\
  \  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-marketing-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-menus-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n\
  \  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-orders-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-payments-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client\
  \ credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-platform-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client ID + Secret Key for a bearer access\n    token).\n- name: oauth2\n  source: openapi/flipdish-stores-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.flipdish.co/identity/connect/authorize\n  - flow: clientCredentials\n    tokenUrl: https://api.flipdish.co/identity/connect/token\n  description: OAuth 2.0. Implicit grant for first-party portal apps; client credentials grant\n    for server-to-server App Store apps (exchange Client\
  \ ID + Secret Key for a bearer access\n    token).\nscopes:\n- scope: api\n  description: Access to the Flipdish API\n  flows:\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/flipdish-apps-openapi.json\n  - openapi/flipdish-catalog-openapi.json\n  - openapi/flipdish-customers-openapi.json\n  - openapi/flipdish-devices-openapi.json\n  - openapi/flipdish-marketing-openapi.json\n  - openapi/flipdish-menus-openapi.json\n  - openapi/flipdish-orders-openapi.json\n  - openapi/flipdish-payments-openapi.json\n  - openapi/flipdish-platform-openapi.json\n  - openapi/flipdish-stores-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/scopes/flipdish-scopes.yml
summary_line: 1 scope · implicit/clientCredentials
tags:
- Restaurant
- Online Ordering
- Mobile Apps
- Point of Sale
- Orders
- Menu
- Payments
- Webhooks
token_urls:
- https://api.flipdish.co/identity/connect/token
---
