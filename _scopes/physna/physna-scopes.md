---
api_specs:
- filename: physna-openapi-original.json
  format: json
  label: Physna Public API
  slug: physna-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-openapi-original.json
authorization_urls:
- https://physna.okta.com/oauth2/default/v1/authorize
description: ''
docs: https://physna.github.io/public-api-guide/api-reference/authentication.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Physna Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Physna publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Physna API on a user''s behalf.


  Tokens are issued from https://physna.okta.com/oauth2/default/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Physna
provider_slug: physna
schemes:
- flows:
  - authorizationUrl: https://physna.okta.com/oauth2/default/v1/authorize
    flow: authorizationCode
    tokenUrl: https://physna.okta.com/oauth2/default/v1/token
  name: okta
  source: openapi/physna-openapi-original.json
scope_count: 6
scope_names:
- Administrators
- Authors
- Viewers
- openid
- roles
- tenant
scopes:
- description: ''
  flows: []
  scope: Administrators
- description: ''
  flows: []
  scope: Authors
- description: ''
  flows: []
  scope: Viewers
- description: ''
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: roles
- description: ''
  flows:
  - authorizationCode
  scope: tenant
slug: physna-scopes
source_filename: physna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/physna-openapi-original.json\ndocs: https://physna.github.io/public-api-guide/api-reference/authentication.html\nnotes: >-\n  Scopes declared on the okta authorizationCode flow are openid, tenant, and\n  roles. The public API guide's client_credentials example additionally\n  requests the composite scope string `tenantApp roles`. Administrators,\n  Authors, and Viewers are role values surfaced through the roles scope, not\n  standalone OAuth scopes.\nschemes:\n- name: okta\n  source: openapi/physna-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://physna.okta.com/oauth2/default/v1/authorize\n    tokenUrl: https://physna.okta.com/oauth2/default/v1/token\nscopes:\n- scope: Administrators\n  sources:\n  - openapi/physna-openapi-original.json\n- scope: Authors\n  sources:\n  - openapi/physna-openapi-original.json\n- scope: Viewers\n  sources:\n  - openapi/physna-openapi-original.json\n\
  - scope: openid\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/physna-openapi-original.json\n- scope: roles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/physna-openapi-original.json\n- scope: tenant\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/physna-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/scopes/physna-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Ai
- 3D
- Geometric Search
- Manufacturing
- Engineering
- Machine Learning
- Search
- Computer Vision
- Product Development
token_urls:
- https://physna.okta.com/oauth2/default/v1/token
---
