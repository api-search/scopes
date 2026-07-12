---
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Stockholm Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Stockholm University publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Stockholm University API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stockholm University
provider_slug: stockholm
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/stockholm-figshare.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: stockholm-scopes
source_filename: stockholm-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stockholm-figshare.yaml\nschemes:\n- name: OAuth2\n  source: openapi/stockholm-figshare.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stockholm-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockholm/refs/heads/main/scopes/stockholm-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Sweden
- Europe
token_urls:
- https://api.figshare.com/v2/token
---
