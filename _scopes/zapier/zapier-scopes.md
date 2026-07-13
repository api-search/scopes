---
api_specs:
- filename: zapier-partner-api.yml
  format: yaml
  label: Zapier Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-partner-api.yml
authorization_urls:
- https://zapier.com/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Zapier Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zapier publishes 10 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zapier API on a user''s behalf.


  Tokens are issued from https://zapier.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zapier
provider_slug: zapier
schemes:
- description: 'See our OAuth2 authentication documentation here: https://docs.zapier.com/powered-by-zapier/api-reference/authentication'
  flows:
  - authorizationUrl: https://zapier.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://zapier.com/oauth/token/
  - authorizationUrl: https://zapier.com/oauth/authorize/
    flow: implicit
  name: OAuth
  source: openapi/zapier-partner-api.yml
scope_count: 10
scope_names:
- action:run
- authentication
- authentication:write
- connection:read
- connection:write
- profile
- zap
- zap:all
- zap:runs
- zap:write
scopes:
- description: Run an Action
  flows:
  - authorizationCode
  - implicit
  scope: action:run
- description: Read Authentications
  flows:
  - authorizationCode
  - implicit
  scope: authentication
- description: Write Authentications
  flows:
  - authorizationCode
  - implicit
  scope: authentication:write
- description: ''
  flows: []
  scope: connection:read
- description: ''
  flows: []
  scope: connection:write
- description: Read profile information about the currently-authenticated user
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Read Zaps
  flows:
  - authorizationCode
  - implicit
  scope: zap
- description: Read Zaps accessible to the account
  flows:
  - authorizationCode
  - implicit
  scope: zap:all
- description: Read Zap Runs
  flows:
  - authorizationCode
  - implicit
  scope: zap:runs
- description: Write Zaps
  flows:
  - authorizationCode
  - implicit
  scope: zap:write
slug: zapier-scopes
source_filename: zapier-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zapier-partner-api.yml\nschemes:\n- name: OAuth\n  source: openapi/zapier-partner-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://zapier.com/oauth/authorize/\n    tokenUrl: https://zapier.com/oauth/token/\n  - flow: implicit\n    authorizationUrl: https://zapier.com/oauth/authorize/\n  description: 'See our OAuth2 authentication documentation here: https://docs.zapier.com/powered-by-zapier/api-reference/authentication'\nscopes:\n- scope: action:run\n  description: Run an Action\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/zapier-partner-api.yml\n- scope: authentication\n  description: Read Authentications\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/zapier-partner-api.yml\n- scope: authentication:write\n  description: Write Authentications\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/zapier-partner-api.yml\n\
  - scope: connection:read\n  sources:\n  - openapi/zapier-partner-api.yml\n- scope: connection:write\n  sources:\n  - openapi/zapier-partner-api.yml\n- scope: profile\n  description: Read profile information about the currently-authenticated user\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/zapier-partner-api.yml\n- scope: zap\n  description: Read Zaps\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/zapier-partner-api.yml\n- scope: zap:all\n  description: Read Zaps accessible to the account\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/zapier-partner-api.yml\n- scope: zap:runs\n  description: Read Zap Runs\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/zapier-partner-api.yml\n- scope: zap:write\n  description: Write Zaps\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/zapier-partner-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/scopes/zapier-scopes.yml
summary_line: 10 scopes · authorizationCode/implicit
tags:
- Integrations
- iPaaS
token_urls:
- https://zapier.com/oauth/token/
---
