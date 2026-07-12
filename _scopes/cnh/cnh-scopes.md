---
authorization_urls:
- https://develop.cnh.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cnh Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CNH publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CNH API on a user''s behalf.


  Tokens are issued from https://develop.cnh.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CNH
provider_slug: cnh
schemes:
- flows:
  - authorizationUrl: https://develop.cnh.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://develop.cnh.com/oauth/token
  name: oauth2
  source: openapi/cnh-fieldops-openapi.yml
scope_count: 5
scope_names:
- equipment
- farm
- prescriptions
- telemetry
- webhooks
scopes:
- description: Access equipment metadata
  flows:
  - authorizationCode
  scope: equipment
- description: Access farm setup
  flows:
  - authorizationCode
  scope: farm
- description: Send prescription Rx files
  flows:
  - authorizationCode
  scope: prescriptions
- description: Access vehicle telemetry data
  flows:
  - authorizationCode
  scope: telemetry
- description: Manage webhook subscriptions
  flows:
  - authorizationCode
  scope: webhooks
slug: cnh-scopes
source_filename: cnh-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cnh-fieldops-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cnh-fieldops-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://develop.cnh.com/oauth/authorize\n    tokenUrl: https://develop.cnh.com/oauth/token\nscopes:\n- scope: equipment\n  description: Access equipment metadata\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cnh-fieldops-openapi.yml\n- scope: farm\n  description: Access farm setup\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cnh-fieldops-openapi.yml\n- scope: prescriptions\n  description: Send prescription Rx files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cnh-fieldops-openapi.yml\n- scope: telemetry\n  description: Access vehicle telemetry data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cnh-fieldops-openapi.yml\n- scope: webhooks\n  description: Manage webhook subscriptions\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/cnh-fieldops-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/scopes/cnh-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Agriculture
- Construction
- Telematics
- Equipment
- FieldOps
token_urls:
- https://develop.cnh.com/oauth/token
---
