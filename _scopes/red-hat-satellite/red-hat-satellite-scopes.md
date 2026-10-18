---
api_specs:
- filename: red-hat-satellite-content-views-api-openapi.yml
  format: yaml
  label: Red Hat Satellite Content Views API
  slug: red-hat-satellite-content-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/openapi/red-hat-satellite-content-views-api-openapi.yml
- filename: red-hat-satellite-hosts-api-openapi.yml
  format: yaml
  label: Red Hat Satellite Hosts API
  slug: red-hat-satellite-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/openapi/red-hat-satellite-hosts-api-openapi.yml
- filename: red-hat-satellite-lifecycle-environments-api-openapi.yml
  format: yaml
  label: Red Hat Satellite Lifecycle Environments API
  slug: red-hat-satellite-lifecycle-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/openapi/red-hat-satellite-lifecycle-environments-api-openapi.yml
- filename: red-hat-satellite-organizations-api-openapi.yml
  format: yaml
  label: Red Hat Satellite Organizations API
  slug: red-hat-satellite-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/openapi/red-hat-satellite-organizations-api-openapi.yml
- filename: red-hat-satellite-subscriptions-api-openapi.yml
  format: yaml
  label: Red Hat Satellite Subscriptions API
  slug: red-hat-satellite-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/openapi/red-hat-satellite-subscriptions-api-openapi.yml
authorization_urls:
- https://satellite.example.com/users/extlogin
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: none
name: Red Hat Satellite Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Red Hat Satellite uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schemes:
- description: OAuth 2.0 Personal Access Token authentication for Satellite users.
  flows:
  - authorizationUrl: https://satellite.example.com/users/extlogin
    flow: implicit
  name: oAuth2
  source: openapi/red-hat-satellite-content-views-api-openapi.yml
- description: OAuth 2.0 Personal Access Token authentication for Satellite users.
  flows:
  - authorizationUrl: https://satellite.example.com/users/extlogin
    flow: implicit
  name: oAuth2
  source: openapi/red-hat-satellite-hosts-api-openapi.yml
- description: OAuth 2.0 Personal Access Token authentication for Satellite users.
  flows:
  - authorizationUrl: https://satellite.example.com/users/extlogin
    flow: implicit
  name: oAuth2
  source: openapi/red-hat-satellite-lifecycle-environments-api-openapi.yml
- description: OAuth 2.0 Personal Access Token authentication for Satellite users.
  flows:
  - authorizationUrl: https://satellite.example.com/users/extlogin
    flow: implicit
  name: oAuth2
  source: openapi/red-hat-satellite-organizations-api-openapi.yml
- description: OAuth 2.0 Personal Access Token authentication for Satellite users.
  flows:
  - authorizationUrl: https://satellite.example.com/users/extlogin
    flow: implicit
  name: oAuth2
  source: openapi/red-hat-satellite-subscriptions-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: red-hat-satellite-scopes
source_filename: red-hat-satellite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/red-hat-satellite-content-views-api-openapi.yml, openapi/red-hat-satellite-hosts-api-openapi.yml,\n  openapi/red-hat-satellite-lifecycle-environments-api-openapi.yml, openapi/red-hat-satellite-organizations-api-openapi.yml,\n  openapi/red-hat-satellite-subscriptions-api-openapi.yml\nschemes:\n- name: oAuth2\n  source: openapi/red-hat-satellite-content-views-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://satellite.example.com/users/extlogin\n  description: OAuth 2.0 Personal Access Token authentication for Satellite users.\n- name: oAuth2\n  source: openapi/red-hat-satellite-hosts-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://satellite.example.com/users/extlogin\n  description: OAuth 2.0 Personal Access Token authentication for Satellite users.\n- name: oAuth2\n  source: openapi/red-hat-satellite-lifecycle-environments-api-openapi.yml\n  flows:\n  - flow: implicit\n\
  \    authorizationUrl: https://satellite.example.com/users/extlogin\n  description: OAuth 2.0 Personal Access Token authentication for Satellite users.\n- name: oAuth2\n  source: openapi/red-hat-satellite-organizations-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://satellite.example.com/users/extlogin\n  description: OAuth 2.0 Personal Access Token authentication for Satellite users.\n- name: oAuth2\n  source: openapi/red-hat-satellite-subscriptions-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://satellite.example.com/users/extlogin\n  description: OAuth 2.0 Personal Access Token authentication for Satellite users.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/scopes/red-hat-satellite-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
token_bound: false
token_urls: []
---
