---
authorization_urls:
- https://authn.read.ai/oauth2/auth
description: Scopes advertised by Read AI's OAuth 2.1 authorization server (authn.read.ai) and by the MCP resource server's RFC 9728 protected-resource metadata. Read AI does not publish a standalone scope-reference page; the descriptions below are the standard OIDC meanings plus the two Read-specific scopes named in the provider's registration example.
docs: https://support.read.ai/hc/en-us/articles/49380809380371-API-Keys-Authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Read Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Read AI publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Read AI API on a user''s behalf.


  Tokens are issued from https://authn.read.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Read AI
provider_slug: read-ai
schemes:
- flows:
  - authorizationUrl: https://authn.read.ai/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://authn.read.ai/oauth2/token
  name: OAuth2
  source: well-known/read-ai-oauth-authorization-server.json
scope_count: 7
scope_names:
- openid
- profile
- email
- offline_access
- offline
- meeting:read
- mcp:execute
scopes:
- description: OpenID Connect — request an ID token identifying the Read AI user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated Read AI user.
  flows:
  - authorizationCode
  scope: profile
- description: The user's primary email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the client can renew the 10-minute access token without a new browser round trip.
  flows:
  - authorizationCode
  scope: offline_access
- description: Legacy alias for offline_access, advertised by the authorization server.
  flows:
  - authorizationCode
  scope: offline
- description: Read access to the authenticated user's meeting reports — metadata, participants, summaries, chapter summaries, action items, key questions, topics, transcripts, metrics and recording download URLs. Backs GET /v1/meetings, GET /v1/meetings/{id} and GET /v1/meetings/{id}/live.
  flows:
  - authorizationCode
  scope: meeting:read
- description: Permission to invoke tools on the Read AI MCP server at https://api.read.ai/mcp.
  flows:
  - authorizationCode
  scope: mcp:execute
slug: read-ai-scopes
source_filename: read-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://api.read.ai/.well-known/oauth-protected-resource/mcp\ndocs: https://support.read.ai/hc/en-us/articles/49380809380371-API-Keys-Authentication\ndescription: >-\n  Scopes advertised by Read AI's OAuth 2.1 authorization server (authn.read.ai) and\n  by the MCP resource server's RFC 9728 protected-resource metadata. Read AI does not\n  publish a standalone scope-reference page; the descriptions below are the standard\n  OIDC meanings plus the two Read-specific scopes named in the provider's\n  registration example.\nschemes:\n  - name: OAuth2\n    source: well-known/read-ai-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://authn.read.ai/oauth2/auth\n        tokenUrl: https://authn.read.ai/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect — request an ID token identifying the Read AI user.\n    flows: [authorizationCode]\n    sources: [well-known/read-ai-openid-configuration.json]\n\
  \  - scope: profile\n    description: Basic profile claims for the authenticated Read AI user.\n    flows: [authorizationCode]\n    sources: [well-known/read-ai-openid-configuration.json]\n  - scope: email\n    description: The user's primary email address claim.\n    flows: [authorizationCode]\n    sources: [well-known/read-ai-openid-configuration.json]\n  - scope: offline_access\n    description: >-\n      Issue a refresh token so the client can renew the 10-minute access token\n      without a new browser round trip.\n    flows: [authorizationCode]\n    sources: [well-known/read-ai-openid-configuration.json]\n  - scope: offline\n    description: Legacy alias for offline_access, advertised by the authorization server.\n    flows: [authorizationCode]\n    sources: [well-known/read-ai-oauth-authorization-server.json]\n  - scope: 'meeting:read'\n    description: >-\n      Read access to the authenticated user's meeting reports — metadata,\n      participants, summaries, chapter summaries,\
  \ action items, key questions,\n      topics, transcripts, metrics and recording download URLs. Backs GET\n      /v1/meetings, GET /v1/meetings/{id} and GET /v1/meetings/{id}/live.\n    flows: [authorizationCode]\n    sources:\n      - well-known/read-ai-oauth-protected-resource-mcp.json\n      - https://support.read.ai/hc/en-us/articles/49380809380371-API-Keys-Authentication\n  - scope: 'mcp:execute'\n    description: >-\n      Permission to invoke tools on the Read AI MCP server at https://api.read.ai/mcp.\n    flows: [authorizationCode]\n    sources:\n      - well-known/read-ai-oauth-protected-resource-mcp.json\n      - https://support.read.ai/hc/en-us/articles/49380809380371-API-Keys-Authentication\naudience:\n  - https://api.read.ai/v1/meetings\n  - https://api.read.ai/mcp\nnotes:\n  - >-\n    Read AI's own dynamic-client-registration example requests the full set:\n    \"openid email offline_access profile meeting:read mcp:execute\".\n  - >-\n    No write scopes are advertised. The\
  \ public API surface is read-only over meeting\n    data; every documented endpoint is a GET.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://api.read.ai/.well-known/oauth-protected-resource/mcp\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/read-ai/refs/heads/main/scopes/read-ai-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Meeting Intelligence
- Artificial Intelligence
- Transcription
- Productivity
- Collaboration
- Model Context Protocol
- Agents
- Webhooks
- SaaS
token_urls:
- https://authn.read.ai/oauth2/token
---
