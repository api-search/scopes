---
api_specs:
- filename: piwik-pro-access-control-api-openapi.yml
  format: yaml
  label: Piwik PRO Access Control API
  slug: piwik-pro-access-control-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-access-control-api-openapi.yml
- filename: piwik-pro-analytics-api-openapi.yml
  format: yaml
  label: Piwik PRO Analytics API
  slug: piwik-pro-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-analytics-api-openapi.yml
- filename: piwik-pro-apps-api-openapi.yml
  format: yaml
  label: Piwik PRO Apps API
  slug: piwik-pro-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-apps-api-openapi.yml
- filename: piwik-pro-audit-log-api-openapi.yml
  format: yaml
  label: Piwik PRO Audit Log API
  slug: piwik-pro-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-audit-log-api-openapi.yml
- filename: piwik-pro-container-settings-api-openapi.yml
  format: yaml
  label: Piwik PRO Container Settings API
  slug: piwik-pro-container-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-container-settings-api-openapi.yml
- filename: piwik-pro-data-activation-api-openapi.yml
  format: yaml
  label: Piwik PRO Data Activation API
  slug: piwik-pro-data-activation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-data-activation-api-openapi.yml
- filename: piwik-pro-meta-sites-api-openapi.yml
  format: yaml
  label: Piwik PRO Meta sites API
  slug: piwik-pro-meta-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-meta-sites-api-openapi.yml
- filename: piwik-pro-modules-api-openapi.yml
  format: yaml
  label: Piwik PRO Modules API
  slug: piwik-pro-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-modules-api-openapi.yml
- filename: piwik-pro-oauth-api-openapi.yml
  format: yaml
  label: Piwik PRO OAuth API
  slug: piwik-pro-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-oauth-api-openapi.yml
- filename: piwik-pro-tag-manager-api-openapi.yml
  format: yaml
  label: Piwik PRO Tag Manager API
  slug: piwik-pro-tag-manager-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tag-manager-api-openapi.yml
- filename: piwik-pro-tracker-api-openapi.yml
  format: yaml
  label: Piwik PRO Tracker API
  slug: piwik-pro-tracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tracker-api-openapi.yml
- filename: piwik-pro-tracker-settings-api-openapi.yml
  format: yaml
  label: Piwik PRO Tracker Settings API
  slug: piwik-pro-tracker-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tracker-settings-api-openapi.yml
- filename: piwik-pro-user-groups-api-openapi.yml
  format: yaml
  label: Piwik PRO User Groups API
  slug: piwik-pro-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-user-groups-api-openapi.yml
- filename: piwik-pro-users-api-openapi.yml
  format: yaml
  label: Piwik PRO Users API
  slug: piwik-pro-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Piwik PRO Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Piwik PRO uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Piwik PRO
provider_slug: piwik-pro
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: OAuth2ClientCredentials
  source: openapi/piwik-pro-web-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: piwik-pro-scopes
source_filename: piwik-pro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: none\nsource: openapi/piwik-pro-web-api-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/piwik-pro-web-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/piwik-pro/scopes/piwik-pro-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Privacy
- Data Activation
- Enterprise
- Compliance
token_bound: false
token_urls:
- /auth/token
---
