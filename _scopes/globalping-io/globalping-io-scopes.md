---
api_specs:
- filename: globalping-io-limits-api-openapi.yml
  format: yaml
  label: Globalping Limits API
  slug: globalping-io-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-limits-api-openapi.yml
- filename: globalping-io-measurements-api-openapi.yml
  format: yaml
  label: Globalping Measurements API
  slug: globalping-io-measurements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-measurements-api-openapi.yml
- filename: globalping-io-probes-api-openapi.yml
  format: yaml
  label: Globalping Probes API
  slug: globalping-io-probes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-probes-api-openapi.yml
authorization_urls:
- https://auth.globalping.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Globalping Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Globalping publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Globalping API on a user''s behalf.


  Tokens are issued from https://auth.globalping.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Globalping
provider_slug: globalping-io
schemes:
- description: 'For developers building applications on top of Globalping - if you want to allow end users to sign in and run measurements under their own accounts,

    we can provide OAuth2 access. Please e-mail d@globalping.io for more information.'
  flows:
  - authorizationUrl: https://auth.globalping.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.globalping.io/oauth/token
  name: OAuth2
  source: openapi/globalping-io-openapi.yaml
scope_count: 1
scope_names:
- measurements
scopes:
- description: execute measurements under your account
  flows:
  - authorizationCode
  scope: measurements
slug: globalping-io-scopes
source_filename: globalping-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/globalping-io-openapi.yaml\nschemes:\n- name: OAuth2\n  source: openapi/globalping-io-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.globalping.io/oauth/authorize\n    tokenUrl: https://auth.globalping.io/oauth/token\n  description: |-\n    For developers building applications on top of Globalping - if you want to allow end users to sign in and run measurements under their own accounts,\n    we can provide OAuth2 access. Please e-mail d@globalping.io for more information.\nscopes:\n- scope: measurements\n  description: execute measurements under your account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/globalping-io-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/globalping-io/scopes/globalping-io-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Networks
- Monitoring
- Open Source
- Free
token_bound: false
token_urls:
- https://auth.globalping.io/oauth/token
---
