---
api_specs:
- filename: upwind-security-management-v2-openapi.yml
  format: yaml
  label: Upwind Management REST API v2
  slug: management-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/openapi/upwind-security-management-v2-openapi.yml
- filename: upwind-security-management-v1-openapi.yml
  format: yaml
  label: Upwind Management REST API v1
  slug: management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/openapi/upwind-security-management-v1-openapi.yml
authorization_urls:
- https://oauth.upwind.io/realms/upwind/protocol/openid-connect/auth
description: ''
docs: https://docs.upwind.io/settings/credentials
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Upwind Security Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Upwind Security publishes 26 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Upwind Security API on a user''s behalf.


  Tokens are issued from https://auth.upwind.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Upwind Security
provider_slug: upwind-security
schemes:
- flows:
  - audiences:
    - https://api.upwind.io
    - https://api.eu.upwind.io
    - https://api.me.upwind.io
    flow: clientCredentials
    tokenUrl: https://auth.upwind.io/oauth/token
  name: OAuth2 (client_credentials)
  source: well-known/upwind-security-auth-openid-configuration.json
- flows:
  - authorizationUrl: https://oauth.upwind.io/realms/upwind/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://oauth.upwind.io/realms/upwind/protocol/openid-connect/token
  issuer: https://oauth.upwind.io/realms/upwind
  name: OpenID Connect (platform realm)
  source: well-known/upwind-security-api-openid-configuration.json
scope_count: 26
scope_names:
- get:client-credentials
- list:client-credentials
- create:client-credentials
- update:client-credentials
- delete:client-credentials
- get:credentials
- create:credentials
- delete:credentials
- get:byoc-credentials
- create:byoc-credentials
- update:byoc-credentials
- delete:byoc-credentials
- list:inventory-assets
- get:inventory-common-keys
- list:detections
- create:heartbeats
- create:cloud-logs
- get:external-ids
- get:serverless-reporters
- create:serverless-reporters
- update:serverless-reporters
- delete:serverless-reporters
- get:scim
- create:scim
- org-id-scope
- service_account
scopes:
- description: ''
  flows: []
  scope: get:client-credentials
- description: ''
  flows: []
  scope: list:client-credentials
- description: ''
  flows: []
  scope: create:client-credentials
- description: ''
  flows: []
  scope: update:client-credentials
- description: ''
  flows: []
  scope: delete:client-credentials
- description: ''
  flows: []
  scope: get:credentials
- description: ''
  flows: []
  scope: create:credentials
- description: ''
  flows: []
  scope: delete:credentials
- description: ''
  flows: []
  scope: get:byoc-credentials
- description: ''
  flows: []
  scope: create:byoc-credentials
- description: ''
  flows: []
  scope: update:byoc-credentials
- description: ''
  flows: []
  scope: delete:byoc-credentials
- description: ''
  flows: []
  scope: list:inventory-assets
- description: ''
  flows: []
  scope: get:inventory-common-keys
- description: ''
  flows: []
  scope: list:detections
- description: ''
  flows: []
  scope: create:heartbeats
- description: ''
  flows: []
  scope: create:cloud-logs
- description: ''
  flows: []
  scope: get:external-ids
- description: ''
  flows: []
  scope: get:serverless-reporters
- description: ''
  flows: []
  scope: create:serverless-reporters
- description: ''
  flows: []
  scope: update:serverless-reporters
- description: ''
  flows: []
  scope: delete:serverless-reporters
- description: ''
  flows: []
  scope: get:scim
- description: ''
  flows: []
  scope: create:scim
- description: ''
  flows: []
  scope: org-id-scope
- description: ''
  flows: []
  scope: service_account
slug: upwind-security-scopes
source_filename: upwind-security-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.upwind.io/.well-known/openid-configuration\ndocs: https://docs.upwind.io/settings/credentials\nnotes: >-\n  Upwind's Management REST API uses OAuth 2.0 client_credentials (Auth0 tenant\n  at auth.upwind.io for API tokens; a Keycloak realm at\n  oauth.upwind.io/realms/upwind backs the platform and MCP hosts). The\n  platform scope strings below are published in scopes_supported of the\n  OIDC discovery document served at api.upwind.io and mcp.upwind.io. Public\n  docs do not map scopes to endpoints; API credential permissions are\n  assigned as RBAC scope + roles in the console (Settings -> Access\n  Management -> Credentials) and tokens inherit them.\nschemes:\n  - name: OAuth2 (client_credentials)\n    source: well-known/upwind-security-auth-openid-configuration.json\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.upwind.io/oauth/token\n        audiences:\n          - https://api.upwind.io\n\
  \          - https://api.eu.upwind.io\n          - https://api.me.upwind.io\n  - name: OpenID Connect (platform realm)\n    source: well-known/upwind-security-api-openid-configuration.json\n    issuer: https://oauth.upwind.io/realms/upwind\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://oauth.upwind.io/realms/upwind/protocol/openid-connect/auth\n        tokenUrl: https://oauth.upwind.io/realms/upwind/protocol/openid-connect/token\nscopes:\n  - scope: get:client-credentials\n  - scope: list:client-credentials\n  - scope: create:client-credentials\n  - scope: update:client-credentials\n  - scope: delete:client-credentials\n  - scope: get:credentials\n  - scope: create:credentials\n  - scope: delete:credentials\n  - scope: get:byoc-credentials\n  - scope: create:byoc-credentials\n  - scope: update:byoc-credentials\n  - scope: delete:byoc-credentials\n  - scope: list:inventory-assets\n  - scope: get:inventory-common-keys\n  - scope: list:detections\n  - scope:\
  \ create:heartbeats\n  - scope: create:cloud-logs\n  - scope: get:external-ids\n  - scope: get:serverless-reporters\n  - scope: create:serverless-reporters\n  - scope: update:serverless-reporters\n  - scope: delete:serverless-reporters\n  - scope: get:scim\n  - scope: create:scim\n  - scope: org-id-scope\n  - scope: service_account\nstandard_oidc_scopes:\n  - openid\n  - profile\n  - email\n  - phone\n  - address\n  - roles\n  - offline_access\n  - acr\n  - basic\n  - web-origins\n  - microprofile-jwt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/scopes/upwind-security-scopes.yml
summary_line: 26 scopes · clientCredentials/authorizationCode
tags:
- Company
- Cybersecurity
- Cloud Security
- CNAPP
- Runtime Security
- Vulnerability Management
- API Security
- Kubernetes
token_urls:
- https://auth.upwind.io/oauth/token
- https://oauth.upwind.io/realms/upwind/protocol/openid-connect/token
---
