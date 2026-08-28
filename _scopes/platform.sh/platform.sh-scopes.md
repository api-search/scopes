---
api_specs:
- filename: platform.sh-rest-api-openapi.json
  format: json
  label: Platform.sh REST API
  slug: platform.sh-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform.sh/refs/heads/main/openapi/platform.sh-rest-api-openapi.json
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
name: Platform.Sh Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Platform.sh publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Platform.sh API on a user''s behalf.


  Tokens are issued from https://auth.api.platform.sh/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Platform.sh
provider_slug: platform.sh
schemes:
- flows:
  - authorizationUrl: https://auth.api.platform.sh/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.api.platform.sh/oauth2/token
  name: OAuth2
  source: openapi/platform.sh-rest-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.api.platform.sh/oauth2/token
  name: OAuth2Admin
  source: openapi/platform.sh-rest-api-openapi.json
scope_count: 1
scope_names:
- admin
scopes:
- description: administrative operations
  flows:
  - clientCredentials
  scope: admin
slug: platform.sh-scopes
source_filename: platform.sh-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/platform.sh-rest-api-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/platform.sh-rest-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.api.platform.sh/oauth2/authorize\n    tokenUrl: https://auth.api.platform.sh/oauth2/token\n- name: OAuth2Admin\n  source: openapi/platform.sh-rest-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.api.platform.sh/oauth2/token\nscopes:\n- scope: admin\n  description: administrative operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/platform.sh-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platform.sh/refs/heads/main/scopes/platform.sh-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Platform as a Service
- Cloud Hosting
- Application Hosting
- Deployment
- DevOps
- Continuous Deployment
- Containers
- Managed Services
- Developer Tools
- Infrastructure
- Multicloud
- Web Hosting
token_urls:
- https://auth.api.platform.sh/oauth2/token
---
