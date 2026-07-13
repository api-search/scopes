---
api_specs:
- filename: university-of-chicago-fence.yaml
  format: yaml
  label: Gen3 Data Commons APIs (CTDS)
  slug: gen3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-chicago/refs/heads/main/openapi/university-of-chicago-fence.yaml
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: University Of Chicago Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Chicago publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Chicago API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Chicago
provider_slug: university-of-chicago
schemes:
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/university-of-chicago-fence.yaml
scope_count: 3
scope_names:
- admin
- data
- user
scopes:
- description: ''
  flows: []
  scope: admin
- description: ''
  flows: []
  scope: data
- description: generic user access
  flows:
  - authorizationCode
  scope: user
slug: university-of-chicago-scopes
source_filename: university-of-chicago-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-chicago-fence.yaml\nschemes:\n- name: OAuth2\n  source: openapi/university-of-chicago-fence.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\nscopes:\n- scope: admin\n  sources:\n  - openapi/university-of-chicago-fence.yaml\n- scope: data\n  sources:\n  - openapi/university-of-chicago-fence.yaml\n- scope: user\n  description: generic user access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/university-of-chicago-fence.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-chicago/refs/heads/main/scopes/university-of-chicago-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Education
- Higher Education
- University
- Research Data
- Open Source
- IIIF
- Identity
- United States
token_urls:
- /oauth/token
---
