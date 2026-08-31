---
api_specs:
- filename: 6sense-company-api-openapi.yml
  format: yaml
  label: 6sense Company API
  slug: 6sense-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-api-openapi.yml
- filename: 6sense-enrichment-api-openapi.yml
  format: yaml
  label: 6sense Enrichment API
  slug: 6sense-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-enrichment-api-openapi.yml
- filename: 6sense-people-api-openapi.yml
  format: yaml
  label: 6sense People API
  slug: 6sense-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-api-openapi.yml
- filename: 6sense-scoring-api-openapi.yml
  format: yaml
  label: 6sense Scoring API
  slug: 6sense-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-scoring-api-openapi.yml
authorization_urls:
- https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/authorize
description: ''
docs: https://support.6sense.com/docs/set-up-the-6sense-mcp-in-claude
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: 6Sense Scopes
name_suffix: OAuth Scopes
note: '6sense declares no oauth2 securityScheme in any published OpenAPI — the REST APIs are API-token only. The OAuth surface below is real but exists solely for the 6sense remote MCP server: it was read from the live RFC 8414 Authorization Server Metadata and RFC 9728 Protected Resource Metadata documents served anonymously from api.6sense.com, both saved verbatim in well-known/. Exactly one scope is advertised. No scope reference page is published; the docs describe authorization as a per-user consent screen rather than a scope catalog.'
overview: '6sense publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the 6sense API on a user''s behalf.


  Tokens are issued from https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 6sense
provider_slug: 6sense
schemes:
- additional_grant_types:
  - refresh_token
  - urn:openid:params:grant-type:ciba
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  dpop_supported: true
  dynamic_client_registration: true
  endpoints:
    backchannel_authentication: https://auth.6sense.com/oauth2/v1/apps/bc-authorize
    jwks: https://auth.6sense.com/P32lusHUPY06hG8MJtqJnKEmq7hJ/.well-known/jwks.json
    registration: https://auth.6sense.com/v1/mgmt/mcp/client/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/register
    revocation: https://auth.6sense.com/oauth2/v1/apps/P32lusHUPY06hG8MJtqJnKEmq7hJ/revoke
    userinfo: https://auth.6sense.com/oauth2/v1/apps/P32lusHUPY06hG8MJtqJnKEmq7hJ/userinfo
  flows:
  - authorizationUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token
  - flow: clientCredentials
    tokenUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token
  issuer: https://auth.6sense.com/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN
  name: 6sense Agentic OAuth (MCP)
  protected_resource: https://api.6sense.com/mcp
  source: well-known/6sense-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
scope_count: 1
scope_names:
- mcp:use
scopes:
- description: Authorizes an MCP client to call the 6sense remote MCP server at https://api.6sense.com/mcp on behalf of the consenting user. 6sense does not subdivide this further; the effective permission set is whatever the authorizing user can already see in the 6sense Revenue Marketing platform, and the server is documented as read-only.
  flows:
  - authorizationCode
  scope: mcp:use
slug: 6sense-scopes
source_filename: 6sense-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.6sense.com/.well-known/oauth-authorization-server\ndocs: https://support.6sense.com/docs/set-up-the-6sense-mcp-in-claude\nnote: >-\n  6sense declares no oauth2 securityScheme in any published OpenAPI — the REST\n  APIs are API-token only. The OAuth surface below is real but exists solely for\n  the 6sense remote MCP server: it was read from the live RFC 8414 Authorization\n  Server Metadata and RFC 9728 Protected Resource Metadata documents served\n  anonymously from api.6sense.com, both saved verbatim in well-known/. Exactly\n  one scope is advertised. No scope reference page is published; the docs describe\n  authorization as a per-user consent screen rather than a scope catalog.\n\nschemes:\n- name: 6sense Agentic OAuth (MCP)\n  type: oauth2\n  source: well-known/6sense-oauth-authorization-server.json\n  issuer: https://auth.6sense.com/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN\n\
  \  protected_resource: https://api.6sense.com/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/authorize\n    tokenUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token\n  additional_grant_types:\n  - refresh_token\n  - urn:openid:params:grant-type:ciba\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  endpoints:\n    registration: https://auth.6sense.com/v1/mgmt/mcp/client/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/register\n    revocation: https://auth.6sense.com/oauth2/v1/apps/P32lusHUPY06hG8MJtqJnKEmq7hJ/revoke\n    userinfo: https://auth.6sense.com/oauth2/v1/apps/P32lusHUPY06hG8MJtqJnKEmq7hJ/userinfo\n\
  \    jwks: https://auth.6sense.com/P32lusHUPY06hG8MJtqJnKEmq7hJ/.well-known/jwks.json\n    backchannel_authentication: https://auth.6sense.com/oauth2/v1/apps/bc-authorize\n  dynamic_client_registration: true\n  dpop_supported: true\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n\nscopes:\n- scope: mcp:use\n  description: >-\n    Authorizes an MCP client to call the 6sense remote MCP server at\n    https://api.6sense.com/mcp on behalf of the consenting user. 6sense does not\n    subdivide this further; the effective permission set is whatever the\n    authorizing user can already see in the 6sense Revenue Marketing platform,\n    and the server is documented as read-only.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/6sense-oauth-authorization-server.json\n  - well-known/6sense-oauth-protected-resource-mcp.json\n\nauthorization_model:\n  granularity: coarse\n  per_user_consent: true\n  inherits_platform_permissions: true\n  note:\
  \ >-\n    A single coarse scope with entitlement enforced downstream by the user's\n    existing 6sense role. Agents cannot request a narrower grant, and there is no\n    published mapping from scope to data domain.\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://api.6sense.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://api.6sense.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/scopes/6sense-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- ABM
- Account-Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- Artificial Intelligence
- Marketing Technology
token_urls:
- https://auth.6sense.com/oauth2/v1/apps/agentic/P32lusHUPY06hG8MJtqJnKEmq7hJ/MS3CTIZ4l7VZ4pFeraAIy18Y6wIVN/token
---
