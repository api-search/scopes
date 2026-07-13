---
api_specs:
- filename: v2.json
  format: json
  label: Red Hat Satellite REST API
  slug: red-hat-satellite-rest-api
  spec_type: OpenAPI
  url: https://satellite.example.com/apidoc/v2.json
authorization_urls:
- https://satellite.example.com/users/extlogin
description: ''
docs: https://docs.redhat.com/en/documentation/red_hat_satellite/6.11/html/api_guide/chap-red_hat_satellite-api_guide-authenticating_api_calls
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Red Hat Satellite Scopes
name_suffix: OAuth Scopes
note: Red Hat Satellite does not use OAuth 2.0 scopes; the REST API authenticates via HTTP basic auth, Personal Access Tokens, SSO sessions, or legacy 1-legged OAuth 1.0a, with authorization governed by Foreman role-based permissions (roles and filters) rather than scopes (https://docs.redhat.com/en/documentation/red_hat_satellite/6.11/html/api_guide/chap-red_hat_satellite-api_guide-authenticating_api_calls).
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
  source: openapi/red-hat-satellite-api.yml
scope_count: 0
scope_names: []
scopes: []
slug: red-hat-satellite-scopes
source_filename: red-hat-satellite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/red-hat-satellite-api.yml\ndocs: https://docs.redhat.com/en/documentation/red_hat_satellite/6.11/html/api_guide/chap-red_hat_satellite-api_guide-authenticating_api_calls\nnote: >-\n  Red Hat Satellite does not use OAuth 2.0 scopes; the REST API authenticates via\n  HTTP basic auth, Personal Access Tokens, SSO sessions, or legacy 1-legged OAuth\n  1.0a, with authorization governed by Foreman role-based permissions (roles and\n  filters) rather than scopes\n  (https://docs.redhat.com/en/documentation/red_hat_satellite/6.11/html/api_guide/chap-red_hat_satellite-api_guide-authenticating_api_calls).\nschemes:\n- name: oAuth2\n  source: openapi/red-hat-satellite-api.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://satellite.example.com/users/extlogin\n  description: OAuth 2.0 Personal Access Token authentication for Satellite users.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/scopes/red-hat-satellite-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
token_urls: []
---
