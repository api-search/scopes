---
api_specs:
- filename: hilberts-ai-program-api-openapi.yml
  format: yaml
  label: Hilbert's Program API
  slug: hilberts-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilberts-ai/refs/heads/main/openapi/hilberts-ai-program-api-openapi.yml
authorization_urls:
- https://hilbert-app.us.auth0.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Hilberts Ai Scopes
name_suffix: OAuth Scopes
note: 'The published OpenAPI declares no oauth2 securityScheme, so derive-oauth-scopes.py found nothing to derive (0 oauth2 schemes, 0 scopes). Hilbert nevertheless runs OAuth 2.0 / OIDC: the application authenticates against the Auth0 tenant hilbert-app.us.auth0.com with audience https://app-api.hilberts.ai. The scopes below are the tenant''s own advertised scopes_supported, read verbatim from its discovery document. These are OIDC identity scopes, not Hilbert API permission scopes. The one API-permission string Hilbert does name anywhere public is admin:project, described in the MetricCalculationRequest schema of the OpenAPI; it is recorded separately below because it is a documented authorization requirement, not a scope the discovery document advertises. No public scopes/permissions reference page exists.'
overview: 'Hilbert''s AI publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hilbert''s AI API on a user''s behalf.


  Tokens are issued from https://hilbert-app.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hilbert's AI
provider_slug: hilberts-ai
schemes:
- audience: https://app-api.hilberts.ai
  flows:
  - authorizationUrl: https://hilbert-app.us.auth0.com/authorize
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    pkce: true
    tokenUrl: https://hilbert-app.us.auth0.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://hilbert-app.us.auth0.com/oauth/token
  - deviceAuthorizationUrl: https://hilbert-app.us.auth0.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://hilbert-app.us.auth0.com/oauth/token
  issuer: https://hilbert-app.us.auth0.com/
  name: auth0-oidc
  source: https://hilbert-app.us.auth0.com/.well-known/openid-configuration
  type: oauth2
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- email
- email_verified
- name
- given_name
- family_name
- nickname
- picture
- phone
- address
- created_at
- identities
scopes:
- description: Request an ID token
  flows: []
  scope: openid
- description: Basic profile claims
  flows: []
  scope: profile
- description: Issue a refresh token
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: email_verified
- description: ''
  flows: []
  scope: name
- description: ''
  flows: []
  scope: given_name
- description: ''
  flows: []
  scope: family_name
- description: ''
  flows: []
  scope: nickname
- description: ''
  flows: []
  scope: picture
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: address
- description: ''
  flows: []
  scope: created_at
- description: ''
  flows: []
  scope: identities
slug: hilberts-ai-scopes
source_filename: hilberts-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://hilbert-app.us.auth0.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  The published OpenAPI declares no oauth2 securityScheme, so derive-oauth-scopes.py\n  found nothing to derive (0 oauth2 schemes, 0 scopes). Hilbert nevertheless runs OAuth\n  2.0 / OIDC: the application authenticates against the Auth0 tenant\n  hilbert-app.us.auth0.com with audience https://app-api.hilberts.ai. The scopes below\n  are the tenant's own advertised scopes_supported, read verbatim from its discovery\n  document. These are OIDC identity scopes, not Hilbert API permission scopes. The one\n  API-permission string Hilbert does name anywhere public is admin:project, described in\n  the MetricCalculationRequest schema of the OpenAPI; it is recorded separately below\n  because it is a documented authorization requirement, not a scope the discovery\n  document advertises. No public scopes/permissions reference page exists.\nschemes:\n\
  - name: auth0-oidc\n  type: oauth2\n  source: https://hilbert-app.us.auth0.com/.well-known/openid-configuration\n  issuer: https://hilbert-app.us.auth0.com/\n  audience: https://app-api.hilberts.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hilbert-app.us.auth0.com/authorize\n    tokenUrl: https://hilbert-app.us.auth0.com/oauth/token\n    pkce: true\n    code_challenge_methods: [S256, plain]\n  - flow: clientCredentials\n    tokenUrl: https://hilbert-app.us.auth0.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://hilbert-app.us.auth0.com/oauth/device/code\n    tokenUrl: https://hilbert-app.us.auth0.com/oauth/token\nscopes:\n- scope: openid\n  kind: oidc\n  description: Request an ID token\n- scope: profile\n  kind: oidc\n  description: Basic profile claims\n- scope: offline_access\n  kind: oidc\n  description: Issue a refresh token\n- scope: email\n  kind: oidc\n- scope: email_verified\n  kind: oidc\n- scope: name\n  kind: oidc\n- scope:\
  \ given_name\n  kind: oidc\n- scope: family_name\n  kind: oidc\n- scope: nickname\n  kind: oidc\n- scope: picture\n  kind: oidc\n- scope: phone\n  kind: oidc\n- scope: address\n  kind: oidc\n- scope: created_at\n  kind: oidc\n- scope: identities\n  kind: oidc\napi_permissions:\n- name: admin:project\n  source: openapi/hilberts-ai-program-api-openapi.yml#/components/schemas/MetricCalculationRequest\n  description: >-\n    Named in the spec as the authorization under which organizationId must be supplied\n    on a metric calculation request. Hilbert publishes no permissions reference, so the\n    full permission set is unknown.\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://hilbert-app.us.auth0.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilberts-ai/refs/heads/main/scopes/hilberts-ai-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Artificial Intelligence
- Growth
- Analytics
- Marketing
- Data Science
- Automation
- Agentic AI
- B2C
token_urls:
- https://hilbert-app.us.auth0.com/oauth/token
---
