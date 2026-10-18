---
api_specs:
- filename: alteryx-collections-api-openapi.yml
  format: yaml
  label: Alteryx Collections API
  slug: alteryx-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-collections-api-openapi.yml
- filename: alteryx-credentials-api-openapi.yml
  format: yaml
  label: Alteryx Credentials API
  slug: alteryx-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-credentials-api-openapi.yml
- filename: alteryx-jobs-api-openapi.yml
  format: yaml
  label: Alteryx Jobs API
  slug: alteryx-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-jobs-api-openapi.yml
- filename: alteryx-schedules-api-openapi.yml
  format: yaml
  label: Alteryx Schedules API
  slug: alteryx-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-schedules-api-openapi.yml
- filename: alteryx-users-api-openapi.yml
  format: yaml
  label: Alteryx Users API
  slug: alteryx-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-users-api-openapi.yml
- filename: alteryx-workflows-api-openapi.yml
  format: yaml
  label: Alteryx Workflows API
  slug: alteryx-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-workflows-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Alteryx Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Alteryx uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{serverHostname}/webapi/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alteryx
provider_slug: alteryx
schemes:
- description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained from the Server User Interface under the Keys section.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{serverHostname}/webapi/oauth2/token
  name: oauth2
  source: openapi/alteryx-collections-api-openapi.yml
- description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained from the Server User Interface under the Keys section.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{serverHostname}/webapi/oauth2/token
  name: oauth2
  source: openapi/alteryx-credentials-api-openapi.yml
- description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained from the Server User Interface under the Keys section.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{serverHostname}/webapi/oauth2/token
  name: oauth2
  source: openapi/alteryx-jobs-api-openapi.yml
- description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained from the Server User Interface under the Keys section.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{serverHostname}/webapi/oauth2/token
  name: oauth2
  source: openapi/alteryx-schedules-api-openapi.yml
- description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained from the Server User Interface under the Keys section.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{serverHostname}/webapi/oauth2/token
  name: oauth2
  source: openapi/alteryx-users-api-openapi.yml
- description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained from the Server User Interface under the Keys section.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{serverHostname}/webapi/oauth2/token
  name: oauth2
  source: openapi/alteryx-workflows-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: alteryx-scopes
source_filename: alteryx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/alteryx-collections-api-openapi.yml, openapi/alteryx-credentials-api-openapi.yml,\n  openapi/alteryx-jobs-api-openapi.yml, openapi/alteryx-schedules-api-openapi.yml, openapi/alteryx-users-api-openapi.yml,\n  openapi/alteryx-workflows-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/alteryx-collections-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{serverHostname}/webapi/oauth2/token\n  description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained\n    from the Server User Interface under the Keys section.\n- name: oauth2\n  source: openapi/alteryx-credentials-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{serverHostname}/webapi/oauth2/token\n  description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained\n    from the Server User Interface under the Keys section.\n- name: oauth2\n  source:\
  \ openapi/alteryx-jobs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{serverHostname}/webapi/oauth2/token\n  description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained\n    from the Server User Interface under the Keys section.\n- name: oauth2\n  source: openapi/alteryx-schedules-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{serverHostname}/webapi/oauth2/token\n  description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained\n    from the Server User Interface under the Keys section.\n- name: oauth2\n  source: openapi/alteryx-users-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{serverHostname}/webapi/oauth2/token\n  description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained\n    from the Server User Interface under the Keys section.\n- name: oauth2\n  source: openapi/alteryx-workflows-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{serverHostname}/webapi/oauth2/token\n  description: OAuth 2.0 authentication using API Access Key and API Access Secret obtained\n    from the Server User Interface under the Keys section.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/scopes/alteryx-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
token_bound: false
token_urls:
- https://{serverHostname}/webapi/oauth2/token
---
