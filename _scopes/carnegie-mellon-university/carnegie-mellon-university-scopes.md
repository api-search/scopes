---
api_specs:
- filename: carnegie-mellon-university-kilthub-figshare.yaml
  format: yaml
  label: KiltHub Repository OAI-PMH (figshare)
  slug: kilthub-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-kilthub-figshare.yaml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Carnegie Mellon University Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Carnegie Mellon University publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Carnegie Mellon University API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Carnegie Mellon University
provider_slug: carnegie-mellon-university
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/carnegie-mellon-university-kilthub-figshare.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: carnegie-mellon-university-scopes
source_filename: carnegie-mellon-university-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/carnegie-mellon-university-kilthub-figshare.yaml\nschemes:\n- name: OAuth2\n  source: openapi/carnegie-mellon-university-kilthub-figshare.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/carnegie-mellon-university-kilthub-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/scopes/carnegie-mellon-university-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- United States
- Research
- Epidemiology
- Open Data
- Library
- Institutional Repository
token_urls:
- https://api.figshare.com/v2/token
---
