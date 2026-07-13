---
api_specs:
- filename: uon-open-research-figshare.yaml
  format: yaml
  label: Open Research Newcastle (Figshare REST API)
  slug: open-research-figshare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-open-research-figshare.yaml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Uon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Newcastle Australia publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Newcastle Australia API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Newcastle Australia
provider_slug: uon
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/uon-open-research-figshare.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: uon-scopes
source_filename: uon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uon-open-research-figshare.yaml\nschemes:\n- name: OAuth2\n  source: openapi/uon-open-research-figshare.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/uon-open-research-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/scopes/uon-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research
- Open Research
- Open Access
- Repository
- OAI-PMH
- Australia
token_urls:
- https://api.figshare.com/v2/token
---
