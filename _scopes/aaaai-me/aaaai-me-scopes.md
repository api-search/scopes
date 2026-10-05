---
api_specs:
- filename: aaaai-me-agents-api-openapi.yml
  format: yaml
  label: AAA AI Agents API
  slug: aaaai-me-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-agents-api-openapi.yml
- filename: aaaai-me-approvals-api-openapi.yml
  format: yaml
  label: AAA AI Approvals API
  slug: aaaai-me-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-approvals-api-openapi.yml
- filename: aaaai-me-auth-api-openapi.yml
  format: yaml
  label: AAA AI Auth API
  slug: aaaai-me-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-auth-api-openapi.yml
- filename: aaaai-me-chat-api-openapi.yml
  format: yaml
  label: AAA AI Chat API
  slug: aaaai-me-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-chat-api-openapi.yml
- filename: aaaai-me-code-api-openapi.yml
  format: yaml
  label: AAA AI Code API
  slug: aaaai-me-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-code-api-openapi.yml
- filename: aaaai-me-cognitive-scaling-api-openapi.yml
  format: yaml
  label: AAA AI Cognitive Scaling API
  slug: aaaai-me-cognitive-scaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-cognitive-scaling-api-openapi.yml
- filename: aaaai-me-cron-api-openapi.yml
  format: yaml
  label: AAA AI Cron API
  slug: aaaai-me-cron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-cron-api-openapi.yml
- filename: aaaai-me-debug-api-openapi.yml
  format: yaml
  label: AAA AI Debug API
  slug: aaaai-me-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-debug-api-openapi.yml
- filename: aaaai-me-deep-agent-api-openapi.yml
  format: yaml
  label: AAA AI Deep Agent API
  slug: aaaai-me-deep-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-deep-agent-api-openapi.yml
- filename: aaaai-me-dynamic-experts-api-openapi.yml
  format: yaml
  label: AAA AI Dynamic Experts API
  slug: aaaai-me-dynamic-experts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-dynamic-experts-api-openapi.yml
- filename: aaaai-me-experts-api-openapi.yml
  format: yaml
  label: AAA AI Experts API
  slug: aaaai-me-experts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-experts-api-openapi.yml
- filename: aaaai-me-health-api-openapi.yml
  format: yaml
  label: AAA AI Health API
  slug: aaaai-me-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-health-api-openapi.yml
- filename: aaaai-me-nodes-api-openapi.yml
  format: yaml
  label: AAA AI Nodes API
  slug: aaaai-me-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-nodes-api-openapi.yml
- filename: aaaai-me-settings-api-openapi.yml
  format: yaml
  label: AAA AI Settings API
  slug: aaaai-me-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-settings-api-openapi.yml
- filename: aaaai-me-user-api-openapi.yml
  format: yaml
  label: AAA AI User API
  slug: aaaai-me-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-user-api-openapi.yml
- filename: aaaai-me-video-api-openapi.yml
  format: yaml
  label: AAA AI Video API
  slug: aaaai-me-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-video-api-openapi.yml
authorization_urls:
- https://web.aaaai.me/
description: ''
docs: https://aaaai.me/auth.md
flows:
- authorizationCode
- refreshToken
- password
kind: oauth-scopes
layout: scope
method: searched
name: Aaaai Me Scopes
name_suffix: OAuth Scopes
note: 'openapi/aaaai-me-openapi.json declares NO oauth2 security scheme (its only scheme is the X-User-Login apiKey header), so derive-oauth-scopes.py has nothing to derive. The scopes below are the ones AAA AI publishes in its OAuth 2.0 authorization-server metadata and OpenID Provider metadata, both served from the marketing host aaaai.me for issuer https://web.aaaai.me, and described for agents at https://aaaai.me/auth.md ("authenticate against the platform issuer https://web.aaaai.me using the metadata at /.well-known/oauth-authorization-server"). VERIFICATION 2026-09-19: the issuer host serves neither metadata document (404) nor the declared JWKS (404); the authorization_endpoint is the application root (https://web.aaaai.me/), the token_endpoint is the email/password login route (POST /api/auth/login, which answered a bare POST with 400 "Login and password required"), and no operation in the contract requires any of these scopes. Treat this as a PUBLISHED scope vocabulary whose authorization
  flow could not be exercised anonymously, not as a working OAuth 2.0 server.'
overview: 'AAA AI publishes 5 OAuth 2.0 scopes via the authorizationCode, refreshToken, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AAA AI API on a user''s behalf.


  Tokens are issued from https://web.aaaai.me/api/auth/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AAA AI
provider_slug: aaaai-me
schemes:
- agent_auth:
    credential_types:
    - api_key
    - session
    - oauth
    supported_identity_types:
    - human
    - service
  flows:
  - authorizationUrl: https://web.aaaai.me/
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://web.aaaai.me/api/auth/login
  - flow: refreshToken
    tokenUrl: https://web.aaaai.me/api/auth/login
  - flow: password
    note: Deprecated in OAuth 2.1; declared here.
    tokenUrl: https://web.aaaai.me/api/auth/login
  issuer: https://web.aaaai.me
  name: oauth-authorization-server (RFC 8414 metadata)
  registration_endpoint: https://aaaai.me/register.html
  registration_note: A human sign-up page, not RFC 7591 dynamic client registration.
  revocation_endpoint: https://web.aaaai.me/api/auth/logout
  served_from: https://aaaai.me/.well-known/oauth-authorization-server
  source: well-known/aaaai-me-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
- id_token_signing_alg_values_supported:
  - RS256
  issuer: https://web.aaaai.me
  jwks_status: 404
  jwks_uri: https://web.aaaai.me/.well-known/jwks.json
  name: openid-configuration (OIDC Discovery metadata)
  response_types_supported:
  - code
  - id_token
  - token
  served_from: https://aaaai.me/.well-known/openid-configuration
  source: well-known/aaaai-me-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - none
scope_count: 5
scope_names:
- openid
- profile
- email
- api
- offline_access
scopes:
- description: OpenID Connect authentication (declared in both documents).
  flows:
  - authorizationCode
  scope: openid
- description: Profile claims (declared in both documents; not described further by the provider).
  flows:
  - authorizationCode
  scope: profile
- description: Email claim (declared in both documents).
  flows:
  - authorizationCode
  scope: email
- description: Access to the platform API (resource https://web.aaaai.me/api per the protected-resource document). Declared in the authorization-server and protected-resource documents only.
  flows:
  - authorizationCode
  scope: api
- description: Refresh tokens (declared in the OpenID Provider metadata only).
  flows:
  - authorizationCode
  scope: offline_access
slug: aaaai-me-scopes
source_filename: aaaai-me-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://aaaai.me/.well-known/oauth-authorization-server\ndocs: https://aaaai.me/auth.md\nnote: >-\n  openapi/aaaai-me-openapi.json declares NO oauth2 security scheme (its only scheme is the\n  X-User-Login apiKey header), so derive-oauth-scopes.py has nothing to derive. The scopes below are\n  the ones AAA AI publishes in its OAuth 2.0 authorization-server metadata and OpenID Provider\n  metadata, both served from the marketing host aaaai.me for issuer https://web.aaaai.me, and\n  described for agents at https://aaaai.me/auth.md (\"authenticate against the platform issuer\n  https://web.aaaai.me using the metadata at /.well-known/oauth-authorization-server\").\n  VERIFICATION 2026-09-19: the issuer host serves neither metadata document (404) nor the declared\n  JWKS (404); the authorization_endpoint is the application root (https://web.aaaai.me/), the\n  token_endpoint is the email/password login route (POST /api/auth/login,\
  \ which answered a bare POST\n  with 400 \"Login and password required\"), and no operation in the contract requires any of these\n  scopes. Treat this as a PUBLISHED scope vocabulary whose authorization flow could not be exercised\n  anonymously, not as a working OAuth 2.0 server.\nschemes:\n- name: oauth-authorization-server (RFC 8414 metadata)\n  source: well-known/aaaai-me-oauth-authorization-server.json\n  issuer: https://web.aaaai.me\n  served_from: https://aaaai.me/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://web.aaaai.me/\n    tokenUrl: https://web.aaaai.me/api/auth/login\n    pkce: [S256]\n  - flow: refreshToken\n    tokenUrl: https://web.aaaai.me/api/auth/login\n  - flow: password\n    tokenUrl: https://web.aaaai.me/api/auth/login\n    note: Deprecated in OAuth 2.1; declared here.\n  token_endpoint_auth_methods_supported: [client_secret_post, none]\n  revocation_endpoint: https://web.aaaai.me/api/auth/logout\n  registration_endpoint:\
  \ https://aaaai.me/register.html\n  registration_note: A human sign-up page, not RFC 7591 dynamic client registration.\n  agent_auth:\n    supported_identity_types: [human, service]\n    credential_types: [api_key, session, oauth]\n- name: openid-configuration (OIDC Discovery metadata)\n  source: well-known/aaaai-me-openid-configuration.json\n  issuer: https://web.aaaai.me\n  served_from: https://aaaai.me/.well-known/openid-configuration\n  jwks_uri: https://web.aaaai.me/.well-known/jwks.json\n  jwks_status: 404\n  response_types_supported: [code, id_token, token]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, none]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (declared in both documents).\n  flows: [authorizationCode]\n  sources: [well-known/aaaai-me-oauth-authorization-server.json, well-known/aaaai-me-openid-configuration.json]\n- scope: profile\n  description: Profile claims\
  \ (declared in both documents; not described further by the provider).\n  flows: [authorizationCode]\n  sources: [well-known/aaaai-me-oauth-authorization-server.json, well-known/aaaai-me-openid-configuration.json]\n- scope: email\n  description: Email claim (declared in both documents).\n  flows: [authorizationCode]\n  sources: [well-known/aaaai-me-oauth-authorization-server.json, well-known/aaaai-me-openid-configuration.json]\n- scope: api\n  description: Access to the platform API (resource https://web.aaaai.me/api per the protected-resource document). Declared in the authorization-server and protected-resource documents only.\n  flows: [authorizationCode]\n  sources: [well-known/aaaai-me-oauth-authorization-server.json, well-known/aaaai-me-oauth-protected-resource.json]\n- scope: offline_access\n  description: Refresh tokens (declared in the OpenID Provider metadata only).\n  flows: [authorizationCode]\n  sources: [well-known/aaaai-me-openid-configuration.json]\nprotected_resource:\n\
  \  source: well-known/aaaai-me-oauth-protected-resource.json\n  resource: https://web.aaaai.me/api\n  authorization_servers: [https://web.aaaai.me]\n  scopes_supported: [openid, profile, email, api]\n  bearer_methods_supported: [header, body]\n  resource_signing_alg_values_supported: [RS256]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/scopes/aaaai-me-scopes.yml
summary_line: 5 scopes · authorizationCode/refreshToken/password
tags:
- Artificial Intelligence
- Agents
- Multi-Agent
- LLM Orchestration
- Meetings
- Voice
- Video
- Workflows
- MCP
- Agentic Commerce
- OpenAI-Compatible
- Self-Hosted
- Agent-Native
- Montenegro
token_bound: false
token_urls:
- https://web.aaaai.me/api/auth/login
---
