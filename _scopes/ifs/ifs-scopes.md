---
api_specs:
- filename: ifs-cloud-erp-openapi.yml
  format: yaml
  label: IFS Cloud ERP API
  slug: ifs-cloud-erp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-cloud-erp-openapi.yml
authorization_urls:
- https://login.ifs.cloud/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ifs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'IFS publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the IFS API on a user''s behalf.


  Tokens are issued from https://login.ifs.cloud/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IFS
provider_slug: ifs
schemes:
- flows:
  - authorizationUrl: https://login.ifs.cloud/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.ifs.cloud/oauth2/token
  name: OAuth2
  source: openapi/ifs-cloud-erp-openapi.yml
scope_count: 2
scope_names:
- ifs.read
- ifs.write
scopes:
- description: Read IFS data
  flows:
  - authorizationCode
  scope: ifs.read
- description: Write IFS data
  flows:
  - authorizationCode
  scope: ifs.write
slug: ifs-scopes
source_filename: ifs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ifs-cloud-erp-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/ifs-cloud-erp-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.ifs.cloud/oauth2/authorize\n    tokenUrl: https://login.ifs.cloud/oauth2/token\nscopes:\n- scope: ifs.read\n  description: Read IFS data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ifs-cloud-erp-openapi.yml\n- scope: ifs.write\n  description: Write IFS data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ifs-cloud-erp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/scopes/ifs-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- ERP
- Field Service
- Asset Management
- Manufacturing
- Energy
- Cloud
token_urls:
- https://login.ifs.cloud/oauth2/token
---
