---
api_specs:
- filename: typeface-api-openapi.json
  format: json
  label: Typeface API
  slug: typeface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-api-openapi.json
- filename: typeface-content-workflow-openapi.json
  format: json
  label: Typeface Content Workflow API
  slug: typeface-content-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-workflow-openapi.json
- filename: typeface-documents-search-openapi.json
  format: json
  label: Typeface Documents Search API
  slug: typeface-documents-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-documents-search-openapi.json
- filename: typeface-team-users-openapi.json
  format: json
  label: Typeface Team Users API
  slug: typeface-team-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-team-users-openapi.json
authorization_urls:
- https://auth-us.typeface.ai/authorize
description: ''
docs: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Typeface Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Typeface publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Typeface API on a user''s behalf.


  Tokens are issued from https://api-us.typeface.ai/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Typeface
provider_slug: typeface
schemes:
- flows:
  - authorizationUrl: https://auth-us.typeface.ai/authorize
    flow: authorizationCode
    tokenUrl: https://api-us.typeface.ai/mcp/oauth/token
  name: mcpOAuth
  source: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
slug: typeface-scopes
source_filename: typeface-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis\ndocs: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis\nnotes: The core REST API uses bearer JWTs from application credentials (no\n  scope surface documented). The documented scope set below applies to the\n  OAuth 2.1 authorization-code flow (with PKCE) for the Typeface MCP server and\n  MCP APIs; the discovery document at\n  https://api-us.typeface.ai/.well-known/oauth-authorization-server lists\n  supported scopes and grant types.\nschemes:\n  - name: mcpOAuth\n    source: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth-us.typeface.ai/authorize\n        tokenUrl: https://api-us.typeface.ai/mcp/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect\
  \ authentication.\n    flows: [authorizationCode]\n  - scope: profile\n    description: Access to the user's profile claims.\n    flows: [authorizationCode]\n  - scope: email\n    description: Access to the user's email claim.\n    flows: [authorizationCode]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived access.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/scopes/typeface-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Ai
- Artificial Intelligence
- Content Generation
- Marketing
- Agents
- Generative AI
- Brand Management
- Enterprise
token_urls:
- https://api-us.typeface.ai/mcp/oauth/token
---
