---
api_specs:
- filename: bloomberg-data-license-api.yml
  format: yaml
  label: Bloomberg Data License API
  slug: bloomberg-data-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-data-license-api.yml
- filename: bloomberg-emsx-api.yml
  format: yaml
  label: Bloomberg EMSX API
  slug: bloomberg-emsx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-emsx-api.yml
- filename: bloomberg-http-api.yml
  format: yaml
  label: Bloomberg HTTP API
  slug: bloomberg-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-http-api.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bloomberg Aim Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bloomberg AIM publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bloomberg AIM API on a user''s behalf.


  Tokens are issued from https://bsso.blpprofessional.com/ext/api/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schemes:
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://bsso.blpprofessional.com/ext/api/as/token.oauth2
  name: oauth2
  source: openapi/bloomberg-data-license-api.yml
scope_count: 3
scope_names:
- eap
- eap.catalogs.read
- eap.catalogs.write
scopes:
- description: Access to Enterprise Access Point data
  flows:
  - clientCredentials
  scope: eap
- description: Read catalog data
  flows:
  - clientCredentials
  scope: eap.catalogs.read
- description: Write catalog data
  flows:
  - clientCredentials
  scope: eap.catalogs.write
slug: bloomberg-aim-scopes
source_filename: bloomberg-aim-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bloomberg-data-license-api.yml\nschemes:\n- name: oauth2\n  source: openapi/bloomberg-data-license-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bsso.blpprofessional.com/ext/api/as/token.oauth2\n  description: OAuth 2.0 client credentials flow\nscopes:\n- scope: eap\n  description: Access to Enterprise Access Point data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n- scope: eap.catalogs.read\n  description: Read catalog data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n- scope: eap.catalogs.write\n  description: Write catalog data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bloomberg-data-license-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/scopes/bloomberg-aim-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
token_urls:
- https://bsso.blpprofessional.com/ext/api/as/token.oauth2
---
