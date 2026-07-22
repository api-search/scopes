---
authorization_urls:
- https://auth.thinkingmachines.ai/oauth2/authorize
description: ''
docs: https://tinker-docs.thinkingmachines.ai/
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Thinking Machines Lab Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Thinking Machines Lab publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Thinking Machines Lab API on a user''s behalf.


  Tokens are issued from https://auth.thinkingmachines.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Thinking Machines Lab
provider_slug: thinking-machines-lab
schemes:
- flows:
  - authorizationUrl: https://auth.thinkingmachines.ai/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.thinkingmachines.ai/oauth2/token
  - deviceAuthorizationUrl: https://auth.thinkingmachines.ai/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://auth.thinkingmachines.ai/oauth2/token
  name: OAuth2
  source: well-known/thinking-machines-lab-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Access to the user's email address claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issue a refresh token for long-lived / headless access.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: thinking-machines-lab-scopes
source_filename: thinking-machines-lab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://auth.thinkingmachines.ai/.well-known/oauth-authorization-server\ndocs: https://tinker-docs.thinkingmachines.ai/\nschemes:\n- name: OAuth2\n  source: well-known/thinking-machines-lab-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.thinkingmachines.ai/oauth2/authorize\n    tokenUrl: https://auth.thinkingmachines.ai/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.thinkingmachines.ai/oauth2/device_authorization\n    tokenUrl: https://auth.thinkingmachines.ai/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  flows: [authorizationCode, deviceCode]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  flows: [authorizationCode, deviceCode]\n- scope: email\n  description: Access to the user's email address claim.\n  flows: [authorizationCode, deviceCode]\n\
  - scope: offline_access\n  description: Issue a refresh token for long-lived / headless access.\n  flows: [authorizationCode, deviceCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thinking-machines-lab/refs/heads/main/scopes/thinking-machines-lab-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Company
- Ai
- Machine Learning
- LLM
- Fine Tuning
- Model Training
- Developer Tools
- Reinforcement Learning
token_urls:
- https://auth.thinkingmachines.ai/oauth2/token
---
