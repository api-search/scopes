---
authorization_urls:
- https://api.fireflies.ai/authorize
description: ''
docs: https://docs.fireflies.ai/fundamentals/authorization
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Fireflies Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fireflies.ai publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fireflies.ai API on a user''s behalf.


  Tokens are issued from https://api.fireflies.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fireflies.ai
provider_slug: fireflies-ai
schemes:
- flows:
  - authorizationUrl: https://api.fireflies.ai/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.fireflies.ai/token
  name: oauth2
  source: well-known/fireflies-ai-oauth-authorization-server.json
scope_count: 2
scope_names:
- profile
- email
scopes:
- description: Access to profile information.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the account email address.
  flows:
  - authorizationCode
  scope: email
slug: fireflies-ai-scopes
source_filename: fireflies-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.fireflies.ai/.well-known/oauth-authorization-server\ndocs: https://docs.fireflies.ai/fundamentals/authorization\nschemes:\n  - name: oauth2\n    source: well-known/fireflies-ai-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.fireflies.ai/authorize\n        tokenUrl: https://api.fireflies.ai/token\n        pkce: S256\nscopes:\n  - scope: profile\n    description: Access to profile information.\n    flows: [authorizationCode]\n    sources: [well-known/fireflies-ai-oauth-authorization-server.json]\n  - scope: email\n    description: Access to the account email address.\n    flows: [authorizationCode]\n    sources: [well-known/fireflies-ai-oauth-authorization-server.json]\nnotes: >-\n  Scopes are those advertised in the RFC 8414 authorization-server metadata\n  (scopes_supported: profile, email). The bearer-token GraphQL API itself is not\n  scope-gated;\
  \ access is governed by team role and plan tier.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireflies-ai/refs/heads/main/scopes/fireflies-ai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Meetings
- Transcription
- Speech to Text
- Conversation Intelligence
- Artificial Intelligence
- GraphQL
- MCP
- Productivity
token_urls:
- https://api.fireflies.ai/token
---
