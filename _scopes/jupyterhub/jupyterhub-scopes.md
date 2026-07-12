---
authorization_urls:
- /hub/api/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Jupyterhub Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'JupyterHub publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the JupyterHub API on a user''s behalf.


  Tokens are issued from /hub/api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: JupyterHub
provider_slug: jupyterhub
schemes:
- flows:
  - authorizationUrl: /hub/api/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /hub/api/oauth2/token
  name: oauth2
  source: openapi/jupyterhub-rest-api-openapi.yml
scope_count: 9
scope_names:
- admin:groups
- admin:servers
- admin:users
- list:users
- proxy
- read:groups
- read:services
- read:users
- self
scopes:
- description: Administer groups.
  flows:
  - authorizationCode
  scope: admin:groups
- description: Administer single-user servers.
  flows:
  - authorizationCode
  scope: admin:servers
- description: Administer users.
  flows:
  - authorizationCode
  scope: admin:users
- description: List users.
  flows:
  - authorizationCode
  scope: list:users
- description: Manage the proxy.
  flows:
  - authorizationCode
  scope: proxy
- description: Read group information.
  flows:
  - authorizationCode
  scope: read:groups
- description: Read service information.
  flows:
  - authorizationCode
  scope: read:services
- description: Read user information.
  flows:
  - authorizationCode
  scope: read:users
- description: Access to the current user.
  flows:
  - authorizationCode
  scope: self
slug: jupyterhub-scopes
source_filename: jupyterhub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupyterhub-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/jupyterhub-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /hub/api/oauth2/authorize\n    tokenUrl: /hub/api/oauth2/token\nscopes:\n- scope: admin:groups\n  description: Administer groups.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n- scope: admin:servers\n  description: Administer single-user servers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n- scope: admin:users\n  description: Administer users.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n- scope: list:users\n  description: List users.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n- scope: proxy\n  description: Manage the proxy.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/jupyterhub-rest-api-openapi.yml\n- scope: read:groups\n  description: Read group information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n- scope: read:services\n  description: Read service information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n- scope: read:users\n  description: Read user information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n- scope: self\n  description: Access to the current user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/scopes/jupyterhub-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Authentication
- Data Science
- Education
- Hub
- Multi-User
- Notebooks
- OAuth2
- Python
token_urls:
- /hub/api/oauth2/token
---
