---
api_specs:
- filename: blue-prism-enterprise-api-openapi.yml
  format: yaml
  label: Blue Prism API
  slug: blue-prism
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-enterprise-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Blue Prism Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blue Prism publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blue Prism API on a user''s behalf.


  Tokens are issued from https://auth-server/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blue Prism
provider_slug: blue-prism
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth-server/connect/token
  name: OAuth2
  source: openapi/blue-prism-enterprise-api-openapi.yml
scope_count: 2
scope_names:
- bp-api
- bpserver
scopes:
- description: API scope
  flows:
  - clientCredentials
  scope: bp-api
- description: Blue Prism Application scope
  flows:
  - clientCredentials
  scope: bpserver
slug: blue-prism-scopes
source_filename: blue-prism-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/blue-prism-enterprise-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/blue-prism-enterprise-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-server/connect/token\nscopes:\n- scope: bp-api\n  description: API scope\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/blue-prism-enterprise-api-openapi.yml\n- scope: bpserver\n  description: Blue Prism Application scope\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/blue-prism-enterprise-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/scopes/blue-prism-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- AI Automation
- RPA
- Intelligent Automation
- Business Process Management
- Process Orchestration
- Agentic AI
- Workflow-Automation
- Enterprise Software
token_urls:
- https://auth-server/connect/token
---
