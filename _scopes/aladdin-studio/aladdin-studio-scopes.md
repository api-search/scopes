---
authorization_urls:
- https://api.blackrock.com/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Aladdin Studio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aladdin Studio publishes 7 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aladdin Studio API on a user''s behalf.


  Tokens are issued from https://api.blackrock.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schemes:
- description: OAuth 2.0 with access tokens for Data Cloud authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.blackrock.com/oauth/token
  name: OAuth2
  source: openapi/aladdin-studio-data-cloud-openapi.yaml
- description: OAuth 2.0 authentication supporting client_credentials and refresh_token flows
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.blackrock.com/oauth/token
  - authorizationUrl: https://api.blackrock.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.blackrock.com/oauth/token
  name: OAuth2
  source: openapi/aladdin-studio-graph-openapi.yaml
- description: OAuth 2.0 authentication for research data access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.blackrock.com/oauth/token
  name: OAuth2
  source: openapi/aladdin-studio-investment-research-openapi.yaml
- description: OAuth 2.0 authentication for trading operations
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.blackrock.com/oauth/token
  name: OAuth2
  source: openapi/aladdin-studio-trading-openapi.yaml
scope_count: 7
scope_names:
- adc:read
- analytics:read
- portfolio:read
- research:read
- risk:read
- trading:read
- trading:write
scopes:
- description: Read Data Cloud data
  flows:
  - clientCredentials
  scope: adc:read
- description: Read analytics data
  flows:
  - clientCredentials
  scope: analytics:read
- description: Read portfolio data
  flows:
  - authorizationCode
  - clientCredentials
  scope: portfolio:read
- description: Read research data
  flows:
  - clientCredentials
  scope: research:read
- description: Read risk analytics
  flows:
  - authorizationCode
  - clientCredentials
  scope: risk:read
- description: Read trading data
  flows:
  - clientCredentials
  scope: trading:read
- description: Create and manage orders
  flows:
  - clientCredentials
  scope: trading:write
slug: aladdin-studio-scopes
source_filename: aladdin-studio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aladdin-studio-data-cloud-openapi.yaml, openapi/aladdin-studio-graph-openapi.yaml,\n  openapi/aladdin-studio-investment-research-openapi.yaml, openapi/aladdin-studio-trading-openapi.yaml\nschemes:\n- name: OAuth2\n  source: openapi/aladdin-studio-data-cloud-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.blackrock.com/oauth/token\n  description: OAuth 2.0 with access tokens for Data Cloud authentication\n- name: OAuth2\n  source: openapi/aladdin-studio-graph-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.blackrock.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.blackrock.com/oauth/authorize\n    tokenUrl: https://api.blackrock.com/oauth/token\n  description: OAuth 2.0 authentication supporting client_credentials and refresh_token flows\n- name: OAuth2\n  source: openapi/aladdin-studio-investment-research-openapi.yaml\n  flows:\n\
  \  - flow: clientCredentials\n    tokenUrl: https://api.blackrock.com/oauth/token\n  description: OAuth 2.0 authentication for research data access\n- name: OAuth2\n  source: openapi/aladdin-studio-trading-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.blackrock.com/oauth/token\n  description: OAuth 2.0 authentication for trading operations\nscopes:\n- scope: adc:read\n  description: Read Data Cloud data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aladdin-studio-data-cloud-openapi.yaml\n- scope: analytics:read\n  description: Read analytics data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aladdin-studio-investment-research-openapi.yaml\n- scope: portfolio:read\n  description: Read portfolio data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aladdin-studio-graph-openapi.yaml\n- scope: research:read\n  description: Read research data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aladdin-studio-investment-research-openapi.yaml\n\
  - scope: risk:read\n  description: Read risk analytics\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aladdin-studio-graph-openapi.yaml\n- scope: trading:read\n  description: Read trading data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aladdin-studio-graph-openapi.yaml\n  - openapi/aladdin-studio-trading-openapi.yaml\n- scope: trading:write\n  description: Create and manage orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aladdin-studio-graph-openapi.yaml\n  - openapi/aladdin-studio-trading-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/scopes/aladdin-studio-scopes.yml
summary_line: 7 scopes · clientCredentials/authorizationCode
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
token_urls:
- https://api.blackrock.com/oauth/token
---
