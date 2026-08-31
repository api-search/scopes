---
api_specs:
- filename: fireflies-transcripts-api-openapi.yml
  format: yaml
  label: Fireflies.ai Transcripts API
  slug: fireflies-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/openapi/fireflies-transcripts-api-openapi.yml
authorization_urls:
- https://api.fireflies.ai/authorize
- https://mcp.fireflies.ai/authorize
description: Fireflies' OAuth surface exists ONLY for the hosted MCP server — the GraphQL API itself is bearer-API-key auth with no OAuth and no scopes. The scopes below are read from the provider's own RFC 8414 authorization-server metadata, not from an OpenAPI securityScheme (the specs in openapi/ declare only BearerAuth, which is why derive-oauth-scopes.py finds nothing).
docs: https://docs.fireflies.ai/getting-started/mcp-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Fireflies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fireflies.ai publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fireflies.ai API on a user''s behalf.


  Tokens are issued from https://api.fireflies.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fireflies.ai
provider_slug: fireflies
schemes:
- applies_to: https://api.fireflies.ai/mcp
  flows:
  - authorizationUrl: https://api.fireflies.ai/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    registrationUrl: https://api.fireflies.ai/register
    revocationUrl: https://api.fireflies.ai/revoke
    tokenUrl: https://api.fireflies.ai/token
    token_endpoint_auth_methods:
    - client_secret_post
    - none
  issuer: https://api.fireflies.ai/
  name: FirefliesMCPOAuth
  source: https://api.fireflies.ai/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: https://mcp.fireflies.ai/mcp
  flows:
  - authorizationUrl: https://mcp.fireflies.ai/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    registrationUrl: https://mcp.fireflies.ai/register
    revocationUrl: https://mcp.fireflies.ai/revoke
    tokenUrl: https://mcp.fireflies.ai/token
    token_endpoint_auth_methods:
    - client_secret_post
    - none
  issuer: https://mcp.fireflies.ai/
  name: FirefliesMCPOAuthAlt
  note: mcp.fireflies.ai serves an identical metadata document under its own issuer. Both hosts front the same MCP product; use api.fireflies.ai/mcp, which is the URL the docs publish.
  source: https://mcp.fireflies.ai/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 2
scope_names:
- profile
- email
scopes:
- description: Basic Fireflies user profile. Declared in scopes_supported on both the authorization-server and protected-resource metadata.
  flows:
  - authorizationCode
  scope: profile
- description: Fireflies account email address. Declared in scopes_supported on both metadata documents.
  flows:
  - authorizationCode
  scope: email
slug: fireflies-scopes
source_filename: fireflies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://api.fireflies.ai/.well-known/oauth-authorization-server\ndocs: https://docs.fireflies.ai/getting-started/mcp-configuration\ndescription: >-\n  Fireflies' OAuth surface exists ONLY for the hosted MCP server — the GraphQL API itself is\n  bearer-API-key auth with no OAuth and no scopes. The scopes below are read from the provider's\n  own RFC 8414 authorization-server metadata, not from an OpenAPI securityScheme (the specs in\n  openapi/ declare only BearerAuth, which is why derive-oauth-scopes.py finds nothing).\nscope_source: rfc8414-discovery\nschemes:\n- name: FirefliesMCPOAuth\n  type: oauth2\n  source: https://api.fireflies.ai/.well-known/oauth-authorization-server\n  issuer: https://api.fireflies.ai/\n  applies_to: https://api.fireflies.ai/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.fireflies.ai/authorize\n    tokenUrl: https://api.fireflies.ai/token\n    revocationUrl: https://api.fireflies.ai/revoke\n\
  \    registrationUrl: https://api.fireflies.ai/register\n    pkce: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post, none]\n    dynamic_client_registration: true\n- name: FirefliesMCPOAuthAlt\n  type: oauth2\n  source: https://mcp.fireflies.ai/.well-known/oauth-authorization-server\n  issuer: https://mcp.fireflies.ai/\n  applies_to: https://mcp.fireflies.ai/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.fireflies.ai/authorize\n    tokenUrl: https://mcp.fireflies.ai/token\n    revocationUrl: https://mcp.fireflies.ai/revoke\n    registrationUrl: https://mcp.fireflies.ai/register\n    pkce: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post, none]\n    dynamic_client_registration: true\n  note: >-\n    mcp.fireflies.ai serves an identical metadata document under its own issuer. Both hosts front\n    the same MCP product; use api.fireflies.ai/mcp,\
  \ which is the URL the docs publish.\nscopes:\n- scope: profile\n  description: Basic Fireflies user profile. Declared in scopes_supported on both the authorization-server and protected-resource metadata.\n  flows: [authorizationCode]\n  sources: ['https://api.fireflies.ai/.well-known/oauth-authorization-server', 'https://api.fireflies.ai/.well-known/oauth-protected-resource']\n- scope: email\n  description: Fireflies account email address. Declared in scopes_supported on both metadata documents.\n  flows: [authorizationCode]\n  sources: ['https://api.fireflies.ai/.well-known/oauth-authorization-server', 'https://api.fireflies.ai/.well-known/oauth-protected-resource']\nscope_count: 2\nanalysis: >-\n  IMPORTANT GRANULARITY FINDING — the two published scopes are identity scopes only. There is no\n  scope that expresses read-vs-write, and no scope that names transcripts, meetings, channels,\n  soundbites, analytics or user administration. A consenting user therefore cannot grant an agent\n\
  \  read-only access: the same token that reads transcripts also drives the write tools\n  (fireflies_share_meeting, fireflies_create_soundbite, fireflies_update_meeting_title,\n  fireflies_move_meeting, fireflies_revoke_meeting_access). Authorization is enforced downstream by\n  Fireflies plan tier and meeting ownership/admin role, not by OAuth scope.\nprotected_resources:\n- resource: https://api.fireflies.ai/mcp\n  authorization_servers: ['https://api.fireflies.ai/']\n  scopes_supported: [profile, email]\n  documentation: https://docs.fireflies.ai/\n  spec: RFC 9728\n  file: ../well-known/fireflies-api-oauth-protected-resource.json\n- resource: https://mcp.fireflies.ai/mcp\n  authorization_servers: ['https://mcp.fireflies.ai/']\n  scopes_supported: [profile, email]\n  documentation: https://docs.fireflies.ai/\n  spec: RFC 9728\n  file: ../well-known/fireflies-mcp-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-14'\n  probes:\n  - {url: 'https://api.fireflies.ai/.well-known/oauth-authorization-server',\
  \ http_status: 200}\n  - {url: 'https://api.fireflies.ai/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://mcp.fireflies.ai/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://mcp.fireflies.ai/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://api.fireflies.ai/.well-known/openid-configuration', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/scopes/fireflies-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Artificial Intelligence
- Meeting Assistant
- Transcription
- Summary
- Action Items
- GraphQL
- Meetings
- Productivity
- Collaboration
- Conversation Intelligence
token_urls:
- https://api.fireflies.ai/token
- https://mcp.fireflies.ai/token
---
