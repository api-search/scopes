---
api_specs:
- filename: engine.oas3.json
  format: json
  label: Seldon Inference API
  slug: seldon-inference-api
  spec_type: OpenAPI
  url: https://github.com/SeldonIO/seldon-core/blob/master/openapi/engine.oas3.json
- filename: seldon-enterprise-platform-api-openapi.yml
  format: yaml
  label: Seldon Enterprise Platform REST API
  slug: seldon-enterprise-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/openapi/seldon-enterprise-platform-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Seldon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Seldon publishes 5 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Seldon API on a user''s behalf.


  Tokens are issued from https://Y.Y.Y.Y.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Seldon
provider_slug: seldon
schemes:
- flows:
  - flow: password
    tokenUrl: https://Y.Y.Y.Y
  name: OAuth2
  source: openapi/seldon-enterprise-platform-api-openapi.yml
scope_count: 5
scope_names:
- '[]'
- email
- groups
- openid
- profile
scopes:
- description: ''
  flows: []
  scope: '[]'
- description: ''
  flows:
  - password
  scope: email
- description: ''
  flows:
  - password
  scope: groups
- description: ''
  flows:
  - password
  scope: openid
- description: ''
  flows:
  - password
  scope: profile
slug: seldon-scopes
source_filename: seldon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seldon-enterprise-platform-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/seldon-enterprise-platform-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://Y.Y.Y.Y\nscopes:\n- scope: '[]'\n  sources:\n  - openapi/seldon-enterprise-platform-api-openapi.yml\n- scope: email\n  flows:\n  - password\n  sources:\n  - openapi/seldon-enterprise-platform-api-openapi.yml\n- scope: groups\n  flows:\n  - password\n  sources:\n  - openapi/seldon-enterprise-platform-api-openapi.yml\n- scope: openid\n  flows:\n  - password\n  sources:\n  - openapi/seldon-enterprise-platform-api-openapi.yml\n- scope: profile\n  flows:\n  - password\n  sources:\n  - openapi/seldon-enterprise-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/scopes/seldon-scopes.yml
summary_line: 5 scopes · password
tags:
- MLOps
- Machine Learning
- Model Serving
- Inference
- Kubernetes
- AI Operations
- Drift Detection
- Explainability
- Canary Deployment
- A/B Testing
- LLMOps
token_urls:
- https://Y.Y.Y.Y
---
