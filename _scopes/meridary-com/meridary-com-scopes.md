---
api_specs:
- filename: meridary-com-agent-api-openapi.yml
  format: yaml
  label: Meridary Agent API
  slug: meridary-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meridary-com/openapi/meridary-com-agent-api-openapi.yml
- filename: meridary-com-calculators-api-openapi.yml
  format: yaml
  label: Meridary Calculators API
  slug: meridary-com-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meridary-com/openapi/meridary-com-calculators-api-openapi.yml
authorization_urls:
- https://www.meridary.com/api/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Meridary Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Meridary publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Meridary API on a user''s behalf.


  Tokens are issued from https://www.meridary.com/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meridary
provider_slug: meridary-com
schemes:
- flows:
  - authorizationUrl: https://www.meridary.com/api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.meridary.com/api/auth/oauth2/token
  name: agentOAuth
  source: openapi/meridary-com-openapi.yml
scope_count: 7
scope_names:
- agent:account:delete
- agent:analysis
- agent:checkout
- agent:plans:read
- agent:plans:write
- offline_access
- openid
scopes:
- description: Cancel billing and permanently delete Agent data
  flows:
  - authorizationCode
  scope: agent:account:delete
- description: Run prepaid analyses
  flows:
  - authorizationCode
  scope: agent:analysis
- description: Create a hosted checkout URL
  flows:
  - authorizationCode
  scope: agent:checkout
- description: Read agent-only plans
  flows:
  - authorizationCode
  scope: agent:plans:read
- description: Write agent-only plans
  flows:
  - authorizationCode
  scope: agent:plans:write
- description: Refresh access without another browser handoff
  flows:
  - authorizationCode
  scope: offline_access
- description: Identify the account
  flows:
  - authorizationCode
  scope: openid
slug: meridary-com-scopes
source_filename: meridary-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/meridary-com-openapi.yml\nschemes:\n- name: agentOAuth\n  source: openapi/meridary-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.meridary.com/api/auth/oauth2/authorize\n    tokenUrl: https://www.meridary.com/api/auth/oauth2/token\nscopes:\n- scope: agent:account:delete\n  description: Cancel billing and permanently delete Agent data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meridary-com-openapi.yml\n- scope: agent:analysis\n  description: Run prepaid analyses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meridary-com-openapi.yml\n- scope: agent:checkout\n  description: Create a hosted checkout URL\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meridary-com-openapi.yml\n- scope: agent:plans:read\n  description: Read agent-only plans\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meridary-com-openapi.yml\n- scope: agent:plans:write\n\
  \  description: Write agent-only plans\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meridary-com-openapi.yml\n- scope: offline_access\n  description: Refresh access without another browser handoff\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meridary-com-openapi.yml\n- scope: openid\n  description: Identify the account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meridary-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/meridary-com/scopes/meridary-com-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Finance
- Retirement
- Planning
- Calculator
- Software-as-a-Service
token_bound: false
token_urls:
- https://www.meridary.com/api/auth/oauth2/token
---
