---
authorization_urls: []
description: ''
docs: https://docs.datarobot.com/en/docs/agentic-ai/agentic-develop/agentic-authentication.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Datarobot Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the DataRobot OIDC authorization server (app.datarobot.com). DataRobot's primary REST API auth is personal API keys (bearer); OAuth2 scopes below apply to the OIDC/agent authorization flows.
overview: 'DataRobot publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the DataRobot API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DataRobot
provider_slug: datarobot
schemes:
- authorizationUrl: https://app.datarobot.com/oauth2/auth
  issuer: https://app.datarobot.com
  name: oauth2
  source: https://app.datarobot.com/.well-known/openid-configuration
  tokenUrl: https://app.datarobot.com/oauth2/token
scope_count: 3
scope_names:
- openid
- offline
- offline_access
scopes:
- description: OIDC — issue an ID token identifying the authenticated subject.
  flows: []
  scope: openid
- description: Request offline access.
  flows: []
  scope: offline
- description: Issue a refresh token for long-lived offline access.
  flows: []
  scope: offline_access
slug: datarobot-scopes
source_filename: datarobot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.datarobot.com/.well-known/openid-configuration\ndocs: https://docs.datarobot.com/en/docs/agentic-ai/agentic-develop/agentic-authentication.html\nnote: >-\n  Scopes advertised by the DataRobot OIDC authorization server (app.datarobot.com).\n  DataRobot's primary REST API auth is personal API keys (bearer); OAuth2 scopes\n  below apply to the OIDC/agent authorization flows.\nschemes:\n  - name: oauth2\n    source: https://app.datarobot.com/.well-known/openid-configuration\n    issuer: https://app.datarobot.com\n    authorizationUrl: https://app.datarobot.com/oauth2/auth\n    tokenUrl: https://app.datarobot.com/oauth2/token\nscopes:\n  - scope: openid\n    description: OIDC — issue an ID token identifying the authenticated subject.\n  - scope: offline\n    description: Request offline access.\n  - scope: offline_access\n    description: Issue a refresh token for long-lived offline access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datarobot/refs/heads/main/scopes/datarobot-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- MLOps
- Data Science
- Agentic AI
- Predictive Analytics
- Generative AI
token_urls: []
---
