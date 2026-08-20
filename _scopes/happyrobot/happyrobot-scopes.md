---
api_specs:
- filename: happyrobot-public-api-openapi.json
  format: json
  label: Happyrobot Public API
  slug: happyrobot-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-public-api-openapi.json
- filename: happyrobot-platform-v1-openapi.json
  format: json
  label: Happyrobot Platform API v1
  slug: happyrobot-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-platform-v1-openapi.json
- filename: happyrobot-public-api-openapi.json
  format: json
  label: Happyrobot Public API (EU cluster)
  slug: happyrobot-public-api-eu-cluster
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-public-api-openapi.json
authorization_urls:
- https://platform.happyrobot.ai/mcp/authorize
- https://docs.happyrobot.ai/mcp/oauth/authorize
- https://auth.happyrobot.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Happyrobot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Happyrobot publishes 8 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Happyrobot API on a user''s behalf.


  Tokens are issued from https://platform.happyrobot.ai/api/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Happyrobot
provider_slug: happyrobot
schemes:
- flows:
  - authorizationUrl: https://platform.happyrobot.ai/mcp/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://platform.happyrobot.ai/api/mcp/token
  - flow: clientCredentials
    tokenUrl: https://platform.happyrobot.ai/api/mcp/token
  issuer: https://platform.happyrobot.ai
  kind: oauth2
  name: platform-mcp
  registration_endpoint: https://platform.happyrobot.ai/api/mcp/register
  source: https://platform.happyrobot.ai/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
- flows:
  - authorizationUrl: https://docs.happyrobot.ai/mcp/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://docs.happyrobot.ai/mcp/oauth/token
  - flow: clientCredentials
    tokenUrl: https://docs.happyrobot.ai/mcp/oauth/token
  issuer: https://docs.happyrobot.ai/mcp/oauth
  kind: oauth2
  name: docs-mcp
  registration_endpoint: https://docs.happyrobot.ai/mcp/oauth/register
  source: https://docs.happyrobot.ai/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
- flows:
  - authorizationUrl: https://auth.happyrobot.ai/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.happyrobot.ai/oauth/token
  issuer: https://auth.happyrobot.ai/
  kind: openIdConnect
  name: console-oidc
  source: https://auth.happyrobot.ai/.well-known/openid-configuration
scope_count: 8
scope_names:
- mcp:full
- mcp:search
- openid
- profile
- email
- offline_access
- phone
- address
scopes:
- description: Full access to the Happyrobot platform MCP surface. The only scope the platform authorization server advertises; there is no narrower read-only or per-resource alternative.
  flows: []
  scope: mcp:full
- description: Search the Happyrobot documentation through the docs MCP server.
  flows: []
  scope: mcp:search
- description: Standard OIDC scope requesting an ID token.
  flows: []
  scope: openid
- description: Standard OIDC scope for the end user's profile claims.
  flows: []
  scope: profile
- description: Standard OIDC scope for the end user's email address and verification status.
  flows: []
  scope: email
- description: Requests a refresh token for long-lived console sessions.
  flows: []
  scope: offline_access
- description: Standard OIDC scope for phone_number claims (advertised by the tenant).
  flows: []
  scope: phone
- description: Standard OIDC scope for address claims (advertised by the tenant).
  flows: []
  scope: address
slug: happyrobot-scopes
source_filename: happyrobot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: >-\n  https://platform.happyrobot.ai/.well-known/oauth-authorization-server,\n  https://docs.happyrobot.ai/.well-known/oauth-authorization-server,\n  https://auth.happyrobot.ai/.well-known/openid-configuration\nnotes: >-\n  Neither OpenAPI document declares an oauth2 securityScheme — the Public API uses a bearer API key — so\n  `derive-oauth-scopes.py` correctly found nothing. The scopes below were instead read from the three live\n  RFC 8414 / OIDC discovery documents Happyrobot publishes. Two of the three planes expose exactly one\n  coarse scope each; there is no per-resource or read/write scope taxonomy on either MCP surface.\nschemes:\n- name: platform-mcp\n  kind: oauth2\n  source: https://platform.happyrobot.ai/.well-known/oauth-authorization-server\n  issuer: https://platform.happyrobot.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.happyrobot.ai/mcp/authorize\n    tokenUrl: https://platform.happyrobot.ai/api/mcp/token\n\
  \    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://platform.happyrobot.ai/api/mcp/token\n  registration_endpoint: https://platform.happyrobot.ai/api/mcp/register\n  token_endpoint_auth_methods:\n  - none\n- name: docs-mcp\n  kind: oauth2\n  source: https://docs.happyrobot.ai/.well-known/oauth-authorization-server\n  issuer: https://docs.happyrobot.ai/mcp/oauth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docs.happyrobot.ai/mcp/oauth/authorize\n    tokenUrl: https://docs.happyrobot.ai/mcp/oauth/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://docs.happyrobot.ai/mcp/oauth/token\n  registration_endpoint: https://docs.happyrobot.ai/mcp/oauth/register\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n- name: console-oidc\n  kind: openIdConnect\n  source: https://auth.happyrobot.ai/.well-known/openid-configuration\n  issuer: https://auth.happyrobot.ai/\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://auth.happyrobot.ai/authorize\n    tokenUrl: https://auth.happyrobot.ai/oauth/token\n    pkce: S256\nscopes:\n- scope: mcp:full\n  description: >-\n    Full access to the Happyrobot platform MCP surface. The only scope the platform authorization server\n    advertises; there is no narrower read-only or per-resource alternative.\n  schemes:\n  - platform-mcp\n  sources:\n  - https://platform.happyrobot.ai/.well-known/oauth-authorization-server\n- scope: mcp:search\n  description: Search the Happyrobot documentation through the docs MCP server.\n  schemes:\n  - docs-mcp\n  sources:\n  - https://docs.happyrobot.ai/.well-known/oauth-authorization-server\n- scope: openid\n  description: Standard OIDC scope requesting an ID token.\n  schemes:\n  - console-oidc\n  sources:\n  - https://auth.happyrobot.ai/.well-known/openid-configuration\n- scope: profile\n  description: Standard OIDC scope for the end user's profile claims.\n  schemes:\n  - console-oidc\n- scope:\
  \ email\n  description: Standard OIDC scope for the end user's email address and verification status.\n  schemes:\n  - console-oidc\n- scope: offline_access\n  description: Requests a refresh token for long-lived console sessions.\n  schemes:\n  - console-oidc\n- scope: phone\n  description: Standard OIDC scope for phone_number claims (advertised by the tenant).\n  schemes:\n  - console-oidc\n- scope: address\n  description: Standard OIDC scope for address claims (advertised by the tenant).\n  schemes:\n  - console-oidc\nobserved_console_request:\n  url: https://app.happyrobot.ai/login\n  redirects_to: https://auth.happyrobot.ai/authorize\n  scope: openid profile email offline_access\n  response_type: code\n  code_challenge_method: S256\ngaps:\n- The Public API itself has no OAuth scope model — a bearer API key is all-or-nothing within its\n  organization and environment.\n- The platform MCP server advertises a single `mcp:full` scope, so an agent granted MCP access to the\n  platform\
  \ inherits the full 205-operation surface, including destructive operations such as\n  DELETE /workflows/{workflow_id} and POST /runs/{run_id}/cancel.\nx-evidence:\n  fetched: '2026-08-01'\n  probes:\n  - url: https://platform.happyrobot.ai/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://docs.happyrobot.ai/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://auth.happyrobot.ai/.well-known/openid-configuration\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/scopes/happyrobot-scopes.yml
summary_line: 8 scopes · authorizationCode/clientCredentials
tags:
- AI Agents
- Agent Orchestration
- Voice AI
- Conversational AI
- Logistics
- Freight
- Supply Chain
- Workflow-Automation
- Contact Center
- Telephony
- MCP
- agent-native
- Agent Governance
- Enterprise Automation
token_urls:
- https://platform.happyrobot.ai/api/mcp/token
- https://docs.happyrobot.ai/mcp/oauth/token
- https://auth.happyrobot.ai/oauth/token
---
