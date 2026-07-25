---
api_specs:
- filename: propelplm-assembly-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Assembly API
  slug: propelplm-assembly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-assembly-api-openapi.yml
- filename: propelplm-assets-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) assets API
  slug: propelplm-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-assets-api-openapi.yml
- filename: propelplm-attachment-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Attachment API
  slug: propelplm-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-attachment-api-openapi.yml
- filename: propelplm-bill-of-material-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Bill of Material API
  slug: propelplm-bill-of-material-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-bill-of-material-api-openapi.yml
- filename: propelplm-bom-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) BOM API
  slug: propelplm-bom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-bom-api-openapi.yml
- filename: propelplm-categories-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) categories API
  slug: propelplm-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-categories-api-openapi.yml
- filename: propelplm-change-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) change API
  slug: propelplm-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-change-api-openapi.yml
- filename: propelplm-channels-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) channels API
  slug: propelplm-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-channels-api-openapi.yml
- filename: propelplm-configuration-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Configuration API
  slug: propelplm-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-configuration-api-openapi.yml
- filename: propelplm-item-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Item API
  slug: propelplm-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-item-api-openapi.yml
- filename: propelplm-manufactureritem-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) ManufacturerItem API
  slug: propelplm-manufactureritem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-manufactureritem-api-openapi.yml
- filename: propelplm-manufacturerpart-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) ManufacturerPart API
  slug: propelplm-manufacturerpart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-manufacturerpart-api-openapi.yml
- filename: propelplm-markup-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) markup API
  slug: propelplm-markup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-markup-api-openapi.yml
- filename: propelplm-products-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) products API
  slug: propelplm-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-products-api-openapi.yml
- filename: propelplm-variants-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) variants API
  slug: propelplm-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-variants-api-openapi.yml
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
