---
api_specs:
- filename: jupyterhub-activity-api-openapi.yml
  format: yaml
  label: JupyterHub Activity API
  slug: jupyterhub-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-activity-api-openapi.yml
- filename: jupyterhub-admin-api-openapi.yml
  format: yaml
  label: JupyterHub Admin API
  slug: jupyterhub-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-admin-api-openapi.yml
- filename: jupyterhub-authorizations-api-openapi.yml
  format: yaml
  label: JupyterHub Authorizations API
  slug: jupyterhub-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-authorizations-api-openapi.yml
- filename: jupyterhub-general-api-openapi.yml
  format: yaml
  label: JupyterHub General API
  slug: jupyterhub-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-general-api-openapi.yml
- filename: jupyterhub-groups-api-openapi.yml
  format: yaml
  label: JupyterHub Groups API
  slug: jupyterhub-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-groups-api-openapi.yml
- filename: jupyterhub-oauth2-api-openapi.yml
  format: yaml
  label: JupyterHub OAuth2 API
  slug: jupyterhub-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-oauth2-api-openapi.yml
- filename: jupyterhub-proxy-api-openapi.yml
  format: yaml
  label: JupyterHub Proxy API
  slug: jupyterhub-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-proxy-api-openapi.yml
- filename: jupyterhub-servers-api-openapi.yml
  format: yaml
  label: JupyterHub Servers API
  slug: jupyterhub-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-servers-api-openapi.yml
- filename: jupyterhub-services-api-openapi.yml
  format: yaml
  label: JupyterHub Services API
  slug: jupyterhub-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-services-api-openapi.yml
- filename: jupyterhub-tokens-api-openapi.yml
  format: yaml
  label: JupyterHub Tokens API
  slug: jupyterhub-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-tokens-api-openapi.yml
- filename: jupyterhub-users-api-openapi.yml
  format: yaml
  label: JupyterHub Users API
  slug: jupyterhub-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-users-api-openapi.yml
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
