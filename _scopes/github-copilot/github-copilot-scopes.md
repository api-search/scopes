---
api_specs:
- filename: api.github.com.json
  format: json
  label: GitHub Copilot API
  slug: github-copilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot for Business API
  slug: github-copilot-for-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot User Management API
  slug: github-copilot-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot Metrics API
  slug: github-copilot-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot Usage Metrics API
  slug: github-copilot-usage-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: api.github.com.json
  format: json
  label: GitHub Copilot Content Exclusion API
  slug: github-copilot-content-exclusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
authorization_urls:
- https://github.com/login/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Github Copilot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GitHub Copilot publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GitHub Copilot API on a user''s behalf.


  Tokens are issued from https://github.com/login/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GitHub Copilot
provider_slug: github-copilot
schemes:
- flows:
  - authorizationUrl: https://github.com/login/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://github.com/login/oauth/access_token
  name: OAuthToken
  source: openapi/github-copilot-openapi.yml
scope_count: 4
scope_names:
- copilot
- manage_billing:copilot
- read:enterprise
- read:org
scopes:
- description: Manage Copilot content exclusion settings
  flows:
  - authorizationCode
  scope: copilot
- description: Manage Copilot billing settings
  flows:
  - authorizationCode
  scope: manage_billing:copilot
- description: Read enterprise data
  flows:
  - authorizationCode
  scope: read:enterprise
- description: Read organization membership and settings
  flows:
  - authorizationCode
  scope: read:org
slug: github-copilot-scopes
source_filename: github-copilot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/github-copilot-openapi.yml\nschemes:\n- name: OAuthToken\n  source: openapi/github-copilot-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://github.com/login/oauth/authorize\n    tokenUrl: https://github.com/login/oauth/access_token\nscopes:\n- scope: copilot\n  description: Manage Copilot content exclusion settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/github-copilot-openapi.yml\n- scope: manage_billing:copilot\n  description: Manage Copilot billing settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/github-copilot-openapi.yml\n- scope: read:enterprise\n  description: Read enterprise data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/github-copilot-openapi.yml\n- scope: read:org\n  description: Read organization membership and settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/github-copilot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/scopes/github-copilot-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Agents
- AI
- Artificial Intelligence
- Code Generation
- Code Review
- Coding Agent
- Custom Instructions
- Developer Tools
- Extensions
- IDE
- Machine Learning
- MCP
- Metrics
- Model Context Protocol
- Productivity
token_urls:
- https://github.com/login/oauth/access_token
---
