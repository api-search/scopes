---
api_specs:
- filename: appyway-availability-realtime-api-openapi.yml
  format: yaml
  label: AppyWay Availability RealTime API
  slug: appyway-availability-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-availability-realtime-api-openapi.yml
- filename: appyway-traffic-data-api-openapi.yml
  format: yaml
  label: AppyWay Traffic Data API
  slug: appyway-traffic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-traffic-data-api-openapi.yml
- filename: appyway-explorer-api-openapi.yml
  format: yaml
  label: AppyWay Explorer API
  slug: appyway-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-explorer-api-openapi.yml
- filename: appyway-platform-api-openapi.yml
  format: yaml
  label: AppyWay Platform API
  slug: appyway-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/openapi/appyway-platform-api-openapi.yml
authorization_urls:
- https://auth.appyway.com/authorize
description: ''
docs: https://docs.appyway.com/docs/public-docs/50055c042f423-authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Appyway Scopes
name_suffix: OAuth Scopes
note: AppyWay does not publish OAuth scopes; its authentication docs state API requests are authenticated using API keys, with invalid keys returning 401 Unauthorized (https://docs.appyway.com/docs/public-docs/50055c042f423-authentication).
overview: 'AppyWay uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.appyway.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AppyWay
provider_slug: appyway
schemes:
- flows:
  - authorizationUrl: https://auth.appyway.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.appyway.com/oauth/token
  name: oAuth2
  source: openapi/appyway-availability-realtime-api-openapi.yml
- flows:
  - authorizationUrl: https://auth.appyway.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.appyway.com/oauth/token
  name: oAuth2
  source: openapi/appyway-explorer-api-openapi.yml
- flows:
  - authorizationUrl: https://auth.appyway.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.appyway.com/oauth/token
  name: oAuth2
  source: openapi/appyway-platform-api-openapi.yml
- flows:
  - authorizationUrl: https://auth.appyway.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.appyway.com/oauth/token
  name: oAuth2
  source: openapi/appyway-traffic-data-api-openapi.yml
- flows:
  - authorizationUrl: https://auth.appyway.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.appyway.com/oauth/token
  name: oAuth2
  source: openapi/availability-realtime-api-openapi.yml
- flows:
  - authorizationUrl: https://auth.appyway.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.appyway.com/oauth/token
  name: oAuth2
  source: openapi/explorer-api-openapi.yml
- flows:
  - authorizationUrl: https://auth.appyway.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.appyway.com/oauth/token
  name: oAuth2
  source: openapi/traffic-data-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: appyway-scopes
source_filename: appyway-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\ndocs: https://docs.appyway.com/docs/public-docs/50055c042f423-authentication\nnote: AppyWay does not publish OAuth scopes; its authentication docs state API requests\n  are authenticated using API keys, with invalid keys returning 401 Unauthorized\n  (https://docs.appyway.com/docs/public-docs/50055c042f423-authentication).\nsource: openapi/appyway-availability-realtime-api-openapi.yml, openapi/appyway-explorer-api-openapi.yml,\n  openapi/appyway-platform-api-openapi.yml, openapi/appyway-traffic-data-api-openapi.yml, openapi/availability-realtime-api-openapi.yml,\n  openapi/explorer-api-openapi.yml, openapi/traffic-data-api-openapi.yml\nschemes:\n- name: oAuth2\n  source: openapi/appyway-availability-realtime-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.appyway.com/authorize\n    tokenUrl: https://auth.appyway.com/oauth/token\n- name: oAuth2\n  source: openapi/appyway-explorer-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.appyway.com/authorize\n    tokenUrl: https://auth.appyway.com/oauth/token\n- name: oAuth2\n  source: openapi/appyway-platform-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.appyway.com/authorize\n    tokenUrl: https://auth.appyway.com/oauth/token\n- name: oAuth2\n  source: openapi/appyway-traffic-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.appyway.com/authorize\n    tokenUrl: https://auth.appyway.com/oauth/token\n- name: oAuth2\n  source: openapi/availability-realtime-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.appyway.com/authorize\n    tokenUrl: https://auth.appyway.com/oauth/token\n- name: oAuth2\n  source: openapi/explorer-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.appyway.com/authorize\n    tokenUrl: https://auth.appyway.com/oauth/token\n\
  - name: oAuth2\n  source: openapi/traffic-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.appyway.com/authorize\n    tokenUrl: https://auth.appyway.com/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appyway/refs/heads/main/scopes/appyway-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Parking
- Traffic
- Urban Mobility
- Smart Cities
- EV Charging
token_urls:
- https://auth.appyway.com/oauth/token
---
