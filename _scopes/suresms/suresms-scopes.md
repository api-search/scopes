---
api_specs:
- filename: suresms-authenticate-api-openapi.yml
  format: yaml
  label: SureSMS Authenticate API
  slug: suresms-authenticate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-authenticate-api-openapi.yml
- filename: suresms-coverage-api-openapi.yml
  format: yaml
  label: SureSMS Coverage API
  slug: suresms-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-coverage-api-openapi.yml
- filename: suresms-message-api-openapi.yml
  format: yaml
  label: SureSMS Message API
  slug: suresms-message-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-message-api-openapi.yml
- filename: suresms-messagestatus-api-openapi.yml
  format: yaml
  label: SureSMS Message Status API
  slug: suresms-messagestatus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-messagestatus-api-openapi.yml
- filename: suresms-price-api-openapi.yml
  format: yaml
  label: SureSMS Price API
  slug: suresms-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-price-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: SureSMS Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SureSMS publishes 2 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SureSMS API on a user''s behalf.


  Tokens are issued from json/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SureSMS
provider_slug: suresms
schemes:
- description: OAuth2 Password Grant
  flows:
  - flow: password
    tokenUrl: json/token
  name: oauth2
  source: openapi/suresms-openapi.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to protected resources
  flows:
  - password
  scope: read
- description: Write access to protected resources
  flows:
  - password
  scope: write
slug: suresms-scopes
source_filename: suresms-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/suresms-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/suresms-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: json/token\n  description: OAuth2 Password Grant\nscopes:\n- scope: ''\n  sources:\n  - openapi/suresms-openapi.json\n- scope: read\n  description: Read access to protected resources\n  flows:\n  - password\n  sources:\n  - openapi/suresms-openapi.json\n- scope: write\n  description: Write access to protected resources\n  flows:\n  - password\n  sources:\n  - openapi/suresms-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/suresms/scopes/suresms-scopes.yml
summary_line: 2 scopes · password
tags:
- SMS Gateway
- Communications Platform
- Industry Solutions
- Integration Services
token_bound: false
token_urls:
- json/token
---
