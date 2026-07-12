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
name: Erasmus University Rotterdam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Erasmus University Rotterdam publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Erasmus University Rotterdam API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Erasmus University Rotterdam
provider_slug: erasmus-university-rotterdam
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/erasmus-university-rotterdam-figshare-data.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: erasmus-university-rotterdam-scopes
source_filename: erasmus-university-rotterdam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/erasmus-university-rotterdam-figshare-data.yaml\nschemes:\n- name: OAuth2\n  source: openapi/erasmus-university-rotterdam-figshare-data.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/erasmus-university-rotterdam-figshare-data.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/scopes/erasmus-university-rotterdam-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Repository
- OAI-PMH
- Netherlands
token_urls:
- https://api.figshare.com/v2/token
---
