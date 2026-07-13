---
api_specs:
- filename: mapmyfitness-openapi.yml
  format: yaml
  label: MapMyFitness API
  slug: mapmyfitness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/under-armour/refs/heads/main/openapi/mapmyfitness-openapi.yml
authorization_urls:
- https://www.mapmyfitness.com/v7.1/oauth2/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Under Armour Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Under Armour publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Under Armour API on a user''s behalf.


  Tokens are issued from https://api.ua.com/v7.1/oauth2/access_token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Under Armour
provider_slug: under-armour
schemes:
- description: OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://www.mapmyfitness.com/v7.1/oauth2/authorize/
    flow: authorizationCode
    tokenUrl: https://api.ua.com/v7.1/oauth2/access_token/
  name: oauth2
  source: openapi/mapmyfitness-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to fitness data
  flows:
  - authorizationCode
  scope: read
- description: Write access to fitness data
  flows:
  - authorizationCode
  scope: write
slug: under-armour-scopes
source_filename: under-armour-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mapmyfitness-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/mapmyfitness-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.mapmyfitness.com/v7.1/oauth2/authorize/\n    tokenUrl: https://api.ua.com/v7.1/oauth2/access_token/\n  description: OAuth 2.0 authentication\nscopes:\n- scope: read\n  description: Read access to fitness data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mapmyfitness-openapi.yml\n- scope: write\n  description: Write access to fitness data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mapmyfitness-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/under-armour/refs/heads/main/scopes/under-armour-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Fitness
- Health
- Wearables
- Connected Fitness
- Sports
- Fortune 1000
token_urls:
- https://api.ua.com/v7.1/oauth2/access_token/
---
