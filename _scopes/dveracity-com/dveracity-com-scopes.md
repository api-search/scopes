---
api_specs:
- filename: dveracity-com-openapi-generated.yml
  format: yaml
  label: dVeracity API
  slug: dveracity-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dveracity-com/openapi/_ae-authored/dveracity-com-openapi-generated.yml
authorization_urls:
- https://api.dveracity.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Dveracity Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'dVeracity publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the dVeracity API on a user''s behalf.


  Tokens are issued from https://api.dveracity.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: dVeracity
provider_slug: dveracity-com
schemes:
- flows:
  - authorizationUrl: https://api.dveracity.com/authorize
    flow: authorizationCode
    tokenUrl: https://api.dveracity.com/token
  name: OAuth_2.0
  source: openapi/dveracity-com-openapi-generated.yml
scope_count: 7
scope_names:
- compliance:evaluate
- compliance:read
- offline_access
- ofp:read
- ofp:validate
- semantic:query
- semantic:templates
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: compliance:evaluate
- description: ''
  flows:
  - authorizationCode
  scope: compliance:read
- description: ''
  flows:
  - authorizationCode
  scope: offline_access
- description: ''
  flows:
  - authorizationCode
  scope: ofp:read
- description: ''
  flows:
  - authorizationCode
  scope: ofp:validate
- description: ''
  flows:
  - authorizationCode
  scope: semantic:query
- description: ''
  flows:
  - authorizationCode
  scope: semantic:templates
slug: dveracity-com-scopes
source_filename: dveracity-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dveracity-com-openapi-generated.yml\nschemes:\n- name: OAuth_2.0\n  source: openapi/dveracity-com-openapi-generated.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.dveracity.com/authorize\n    tokenUrl: https://api.dveracity.com/token\nscopes:\n- scope: compliance:evaluate\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dveracity-com-openapi-generated.yml\n- scope: compliance:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dveracity-com-openapi-generated.yml\n- scope: offline_access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dveracity-com-openapi-generated.yml\n- scope: ofp:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dveracity-com-openapi-generated.yml\n- scope: ofp:validate\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dveracity-com-openapi-generated.yml\n- scope: semantic:query\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/dveracity-com-openapi-generated.yml\n- scope: semantic:templates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dveracity-com-openapi-generated.yml\n"
source_yaml_url: https://artifacts.apis.io/dveracity-com/scopes/dveracity-com-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Emissions
- Verification
- Carbon Accounting
- Open Standard
token_bound: false
token_urls:
- https://api.dveracity.com/token
---
