---
api_specs:
- filename: upsun-openapi-original.json
  format: json
  label: Upsun REST API
  slug: upsun-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upsun/refs/heads/main/openapi/upsun-openapi-original.json
authorization_urls:
- https://auth.api.platform.sh/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Upsun Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Upsun publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Upsun API on a user''s behalf.


  Tokens are issued from https://auth.api.platform.sh/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Upsun
provider_slug: upsun
schemes:
- flows:
  - authorizationUrl: https://auth.api.platform.sh/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.api.platform.sh/oauth2/token
  name: OAuth2
  source: openapi/upsun-openapi-original.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.api.platform.sh/oauth2/token
  name: OAuth2Admin
  source: openapi/upsun-openapi-original.json
scope_count: 1
scope_names:
- admin
scopes:
- description: administrative operations
  flows:
  - clientCredentials
  scope: admin
slug: upsun-scopes
source_filename: upsun-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/upsun-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/upsun-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.api.platform.sh/oauth2/authorize\n    tokenUrl: https://auth.api.platform.sh/oauth2/token\n- name: OAuth2Admin\n  source: openapi/upsun-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.api.platform.sh/oauth2/token\nscopes:\n- scope: admin\n  description: administrative operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/upsun-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upsun/refs/heads/main/scopes/upsun-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Infrastructure Saas
- Cloud
- PaaS
- Hosting
- Deployment
- DevOps
- Containers
- Observability
token_urls:
- https://auth.api.platform.sh/oauth2/token
---
