---
authorization_urls:
- https://signin.sensecore.cn/oauth2/auth
description: ''
docs: https://platform.sensenova.cn/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Sensetime Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SenseTime publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the SenseTime API on a user''s behalf.


  Tokens are issued from https://signin.sensecore.cn/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SenseTime
provider_slug: sensetime
schemes:
- flows:
  - authorizationUrl: https://signin.sensecore.cn/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://signin.sensecore.cn/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://signin.sensecore.cn/oauth2/token
  issuer: https://signin.sensecore.cn/
  name: SenseCoreOIDC
  source: well-known/sensetime-openid-configuration.json
scope_count: 3
scope_names:
- openid
- offline
- offline_access
scopes:
- description: OpenID Connect sign-in; issue an ID token identifying the subject.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Request offline access (issue a refresh token).
  flows:
  - authorizationCode
  scope: offline
- description: Standard OIDC offline access; issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
slug: sensetime-scopes
source_filename: sensetime-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: well-known/sensetime-openid-configuration.json\ndocs: https://platform.sensenova.cn/.well-known/openid-configuration\nschemes:\n- name: SenseCoreOIDC\n  source: well-known/sensetime-openid-configuration.json\n  issuer: https://signin.sensecore.cn/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://signin.sensecore.cn/oauth2/auth\n    tokenUrl: https://signin.sensecore.cn/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://signin.sensecore.cn/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issue an ID token identifying the subject.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/sensetime-openid-configuration.json]\n- scope: offline\n  description: Request offline access (issue a refresh token).\n  flows: [authorizationCode]\n  sources: [well-known/sensetime-openid-configuration.json]\n- scope: offline_access\n  description: Standard OIDC offline\
  \ access; issue a refresh token for long-lived access.\n  flows: [authorizationCode]\n  sources: [well-known/sensetime-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensetime/refs/heads/main/scopes/sensetime-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Foundation Models
- Large Language Models
- Generative AI
- Computer Vision
- LLM API
token_urls:
- https://signin.sensecore.cn/oauth2/token
---
