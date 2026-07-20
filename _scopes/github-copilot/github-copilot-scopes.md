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
docs: https://docs.github.com/en/rest/copilot/copilot-user-management
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Github Copilot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GitHub Copilot publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GitHub Copilot API on a user''s behalf.


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
scope_count: 5
scope_names:
- manage_billing:copilot
- read:org
- admin:org
- read:enterprise
- copilot
scopes:
- description: Manage Copilot billing and seat assignments — required for adding/removing users or teams from Copilot subscriptions and viewing billing information.
  flows:
  - authorizationCode
  scope: manage_billing:copilot
- description: Read organization membership and settings — sufficient (alongside manage_billing:copilot) for read operations such as viewing Copilot billing, seats, and metrics.
  flows:
  - authorizationCode
  scope: read:org
- description: Full organization administration — alternative to manage_billing:copilot for write operations (adding/removing users or teams from Copilot subscriptions).
  flows:
  - authorizationCode
  scope: admin:org
- description: Read enterprise data — required for enterprise-level Copilot usage metrics reports.
  flows:
  - authorizationCode
  scope: read:enterprise
- description: Copilot scope covering Copilot content-exclusion and related settings on fine-grained/classic tokens.
  flows:
  - authorizationCode
  scope: copilot
slug: github-copilot-scopes
source_filename: github-copilot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/github-copilot-openapi.yml\ndocs: https://docs.github.com/en/rest/copilot/copilot-user-management\nschemes:\n- name: OAuthToken\n  source: openapi/github-copilot-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://github.com/login/oauth/authorize\n    tokenUrl: https://github.com/login/oauth/access_token\nscopes:\n- scope: manage_billing:copilot\n  description: >-\n    Manage Copilot billing and seat assignments — required for adding/removing\n    users or teams from Copilot subscriptions and viewing billing information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/github-copilot-openapi.yml\n  - https://docs.github.com/en/rest/copilot/copilot-user-management\n- scope: read:org\n  description: >-\n    Read organization membership and settings — sufficient (alongside\n    manage_billing:copilot) for read operations such as viewing Copilot billing,\n    seats, and metrics.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/github-copilot-openapi.yml\n  - https://docs.github.com/en/rest/copilot/copilot-user-management\n- scope: admin:org\n  description: >-\n    Full organization administration — alternative to manage_billing:copilot for\n    write operations (adding/removing users or teams from Copilot subscriptions).\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.github.com/en/rest/copilot/copilot-user-management\n- scope: read:enterprise\n  description: Read enterprise data — required for enterprise-level Copilot usage metrics reports.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/github-copilot-openapi.yml\n- scope: copilot\n  description: >-\n    Copilot scope covering Copilot content-exclusion and related settings on\n    fine-grained/classic tokens.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/github-copilot-openapi.yml\nnotes: >-\n  Fine-grained personal access tokens use the \"GitHub Copilot Business\"\
  \ (read)\n  and organization \"Administration\" permissions instead of the classic OAuth\n  scopes above. See https://docs.github.com/en/rest/copilot/copilot-user-management\n  for the per-endpoint permission matrix.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/scopes/github-copilot-scopes.yml
summary_line: 5 scopes · authorizationCode
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
