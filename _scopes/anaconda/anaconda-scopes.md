---
api_specs:
- filename: anaconda-server-openapi-original.json
  format: json
  label: Anaconda Server API
  slug: server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-server-openapi-original.json
- filename: anaconda-org-management-openapi-original.json
  format: json
  label: Anaconda Organization Management API
  slug: org-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-org-management-openapi-original.json
- filename: anaconda-audit-logs-openapi-original.json
  format: json
  label: Anaconda Audit Logs API
  slug: audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-audit-logs-openapi-original.json
- filename: anaconda-ai-navigator-openapi-original.json
  format: json
  label: Anaconda AI Navigator API
  slug: ai-navigator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-ai-navigator-openapi-original.json
- filename: anaconda-desktop-openapi-original.json
  format: json
  label: Anaconda Desktop API
  slug: desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/openapi/anaconda-desktop-openapi-original.json
authorization_urls:
- https://anaconda.com/api/auth/oauth2/authorize
description: ''
docs: https://anaconda.com/docs/cli-reference/anaconda-auth/getting-started
flows:
- authorizationCode
- clientCredentials
- deviceCode
- password
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Anaconda Scopes
name_suffix: OAuth Scopes
note: No Anaconda OpenAPI declares an oauth2 securityScheme, so no scopes could be derived from the specifications (derive-oauth-scopes.py returned zero). The scope set below is what Anaconda's own OIDC discovery document advertises. The Anaconda Server repository API additionally exposes a runtime scope registry at `GET /system/scopes` (operationId repo.endpoints.system.scopes), but that endpoint requires authentication, so its contents are not enumerated here.
overview: 'Anaconda publishes 3 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, password, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Anaconda API on a user''s behalf.


  Tokens are issued from https://anaconda.com/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Anaconda
provider_slug: anaconda
schemes:
- discovery: https://anaconda.com/.well-known/openid-configuration
  flows:
  - authorizationUrl: https://anaconda.com/api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://anaconda.com/api/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://anaconda.com/api/auth/oauth2/token
  - deviceAuthorizationUrl: https://anaconda.com/api/auth/oauth2/device/authorize
    flow: deviceCode
    tokenUrl: https://anaconda.com/api/auth/oauth2/token
  - flow: password
    tokenUrl: https://anaconda.com/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://anaconda.com/api/auth/oauth2/token
  issuer: https://auth.anaconda.com/api/auth
  name: Anaconda OIDC
  source: well-known/anaconda-openid-configuration.json
  type: openIdConnect
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: Standard OIDC scope requesting an ID token.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Access to the authenticated user's basic profile claims.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Access to the authenticated user's email address claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
slug: anaconda-scopes
source_filename: anaconda-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://anaconda.com/.well-known/openid-configuration\ndocs: https://anaconda.com/docs/cli-reference/anaconda-auth/getting-started\nnote: No Anaconda OpenAPI declares an oauth2 securityScheme, so no scopes could be\n  derived from the specifications (derive-oauth-scopes.py returned zero). The scope\n  set below is what Anaconda's own OIDC discovery document advertises. The Anaconda\n  Server repository API additionally exposes a runtime scope registry at `GET /system/scopes`\n  (operationId repo.endpoints.system.scopes), but that endpoint requires authentication,\n  so its contents are not enumerated here.\nschemes:\n- name: Anaconda OIDC\n  type: openIdConnect\n  issuer: https://auth.anaconda.com/api/auth\n  discovery: https://anaconda.com/.well-known/openid-configuration\n  source: well-known/anaconda-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://anaconda.com/api/auth/oauth2/authorize\n\
  \    tokenUrl: https://anaconda.com/api/auth/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://anaconda.com/api/auth/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://anaconda.com/api/auth/oauth2/device/authorize\n    tokenUrl: https://anaconda.com/api/auth/oauth2/token\n  - flow: password\n    tokenUrl: https://anaconda.com/api/auth/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://anaconda.com/api/auth/oauth2/token\nscopes:\n- scope: openid\n  description: Standard OIDC scope requesting an ID token.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/anaconda-openid-configuration.json]\n- scope: profile\n  description: Access to the authenticated user's basic profile claims.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/anaconda-openid-configuration.json]\n- scope: email\n  description: Access to the authenticated user's email address claim.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/anaconda-openid-configuration.json]\n\
  runtime_scope_registry:\n  endpoint: GET /system/scopes\n  api: anaconda:server-api\n  operation_id: repo.endpoints.system.scopes\n  summary: Get all possible scopes in system\n  auth_required: true\n  enumerated: false\nx-evidence:\n  fetched: '2026-08-02'\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anaconda/refs/heads/main/scopes/anaconda-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials/deviceCode/password/refreshToken
tags:
- Company
- Data Science
- Machine Learning
- Artificial Intelligence
- Package Management
- Python
- Developer Tools
- Software Supply Chain
- Repository
- Package Registry
- Conda
- MCP
token_urls:
- https://anaconda.com/api/auth/oauth2/token
---
