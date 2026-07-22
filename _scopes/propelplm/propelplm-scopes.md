---
api_specs:
- filename: propelplm-core-openapi.yml
  format: yaml
  label: Propel PLM Core REST API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-core-openapi.yml
- filename: propelplm-pim-openapi.yml
  format: yaml
  label: Propel PIM API
  slug: pim
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-pim-openapi.yml
authorization_urls:
- '{{url}}{{site}}/services/oauth2/authorize'
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Propelplm Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Propel Software (Propel PLM) publishes 4 OAuth 2.0 scopes via the implicit and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Propel Software (Propel PLM) API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Propel Software (Propel PLM)
provider_slug: propelplm
schemes:
- description: This API uses OAuth 2 with the implicit grant flow.
  flows:
  - authorizationUrl: '{{url}}{{site}}/services/oauth2/authorize'
    flow: implicit
  name: oAuth2Implicit
  source: openapi/propelplm-configuration-openapi.yml
- description: Salesforce OAuth 2.0 (Connected App). Server-side (authorization code) flow.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: salesforceOAuth
  source: openapi/propelplm-core-openapi.yml
- description: This API uses OAuth 2 with the implicit grant flow.
  flows:
  - authorizationUrl: '{{url}}{{site}}/services/oauth2/authorize'
    flow: implicit
  name: oAuth2Implicit
  source: openapi/propelplm-manufacturer-item-openapi.yml
- description: This API uses OAuth 2 with the implicit grant flow.
  flows:
  - authorizationUrl: '{{url}}{{site}}/services/oauth2/authorize'
    flow: implicit
  name: oAuth2Implicit
  source: openapi/propelplm-manufacturer-part-openapi.yml
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: salesforceOAuth
  source: openapi/propelplm-pim-openapi.yml
scope_count: 4
scope_names:
- api
- full
- refresh_token
- web
scopes:
- description: Enable read and write access to Propel objects
  flows:
  - authorizationCode
  - implicit
  scope: api
- description: Full access
  flows:
  - authorizationCode
  scope: full
- description: Obtain refresh tokens for offline access
  flows:
  - authorizationCode
  scope: refresh_token
- description: Web access
  flows:
  - authorizationCode
  scope: web
slug: propelplm-scopes
source_filename: propelplm-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/propelplm-configuration-openapi.yml, openapi/propelplm-core-openapi.yml, openapi/propelplm-manufacturer-item-openapi.yml,\n  openapi/propelplm-manufacturer-part-openapi.yml, openapi/propelplm-pim-openapi.yml\nschemes:\n- name: oAuth2Implicit\n  source: openapi/propelplm-configuration-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: '{{url}}{{site}}/services/oauth2/authorize'\n  description: This API uses OAuth 2 with the implicit grant flow.\n- name: salesforceOAuth\n  source: openapi/propelplm-core-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 (Connected App). Server-side (authorization code) flow.\n- name: oAuth2Implicit\n  source: openapi/propelplm-manufacturer-item-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl:\
  \ '{{url}}{{site}}/services/oauth2/authorize'\n  description: This API uses OAuth 2 with the implicit grant flow.\n- name: oAuth2Implicit\n  source: openapi/propelplm-manufacturer-part-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: '{{url}}{{site}}/services/oauth2/authorize'\n  description: This API uses OAuth 2 with the implicit grant flow.\n- name: salesforceOAuth\n  source: openapi/propelplm-pim-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\nscopes:\n- scope: api\n  description: Enable read and write access to Propel objects\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/propelplm-configuration-openapi.yml\n  - openapi/propelplm-core-openapi.yml\n  - openapi/propelplm-manufacturer-item-openapi.yml\n  - openapi/propelplm-manufacturer-part-openapi.yml\n  - openapi/propelplm-pim-openapi.yml\n- scope:\
  \ full\n  description: Full access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/propelplm-core-openapi.yml\n- scope: refresh_token\n  description: Obtain refresh tokens for offline access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/propelplm-core-openapi.yml\n- scope: web\n  description: Web access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/propelplm-core-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/scopes/propelplm-scopes.yml
summary_line: 4 scopes · implicit/authorizationCode
tags:
- Company
- Product Lifecycle Management
- PLM
- Quality Management
- QMS
- Product Information Management
- PIM
- Manufacturing
- Salesforce
- Bill of Materials
- Change Management
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
