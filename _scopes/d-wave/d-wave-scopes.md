---
authorization_urls:
- https://cloud.dwavesys.com/leap/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: D Wave Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'D-Wave publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the D-Wave API on a user''s behalf.


  Tokens are issued from https://cloud.dwavesys.com/leap/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: D-Wave
provider_slug: d-wave
schemes:
- flows:
  - authorizationUrl: https://cloud.dwavesys.com/leap/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://cloud.dwavesys.com/leap/oauth/token
  name: LeapOAuth
  source: openapi/d-wave-leap-account-api-openapi.yml
scope_count: 1
scope_names:
- account
scopes:
- description: Read account, projects, and tokens
  flows:
  - authorizationCode
  scope: account
slug: d-wave-scopes
source_filename: d-wave-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/d-wave-leap-account-api-openapi.yml\nschemes:\n- name: LeapOAuth\n  source: openapi/d-wave-leap-account-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud.dwavesys.com/leap/oauth/authorize\n    tokenUrl: https://cloud.dwavesys.com/leap/oauth/token\nscopes:\n- scope: account\n  description: Read account, projects, and tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/d-wave-leap-account-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/scopes/d-wave-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Quantum Computing
- Quantum Annealing
- Optimization
- Hybrid Quantum-Classical
- Ising
- QUBO
- Industrial Optimization
- Sampling
- Leap
- Ocean SDK
- SAPI
token_urls:
- https://cloud.dwavesys.com/leap/oauth/token
---
