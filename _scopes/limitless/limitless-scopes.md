---
api_specs:
- filename: limitless-developer-openapi-original.yml
  format: yaml
  label: Limitless Developer API
  slug: developer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limitless/refs/heads/main/openapi/limitless-developer-openapi-original.yml
authorization_urls:
- https://api.limitless.ai/api/auth/authorize
description: ''
docs: https://www.limitless.ai/developers
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Limitless Scopes
name_suffix: OAuth Scopes
note: Scopes are NOT declared in the published Swagger 2.0 document (it has no securityDefinitions). They come from the live RFC 8414 / OIDC Discovery documents on api.limitless.ai, which back the hosted MCP server. Limitless publishes no separate scopes/permissions reference page.
overview: 'Limitless publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Limitless API on a user''s behalf.


  Tokens are issued from https://api.limitless.ai/api/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Limitless
provider_slug: limitless
schemes:
- flows:
  - authorizationUrl: https://api.limitless.ai/api/auth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.limitless.ai/api/auth/token
  name: LimitlessOAuth
  source: well-known/limitless-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- lifelogs:read
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the Limitless user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to basic profile claims (name, preferred_username, updated_at).
  flows:
  - authorizationCode
  scope: profile
- description: Access to the email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Read access to the authenticated user's lifelogs - the Pendant recordings, transcripts, and structured contents exposed by GET /v1/lifelogs and GET /v1/lifelogs/{id}. This is the only resource-level scope Limitless advertises; note that the REST API's DELETE operations have no corresponding write/delete scope, which implies deletion is only reachable with an X-API-Key, not an OAuth token.
  flows:
  - authorizationCode
  scope: lifelogs:read
slug: limitless-scopes
source_filename: limitless-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/limitless-oauth-authorization-server.json\ndocs: https://www.limitless.ai/developers\nnote: >-\n  Scopes are NOT declared in the published Swagger 2.0 document (it has no\n  securityDefinitions). They come from the live RFC 8414 / OIDC Discovery documents on\n  api.limitless.ai, which back the hosted MCP server. Limitless publishes no separate\n  scopes/permissions reference page.\nschemes:\n- name: LimitlessOAuth\n  source: well-known/limitless-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.limitless.ai/api/auth/authorize\n    tokenUrl: https://api.limitless.ai/api/auth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the Limitless user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/limitless-openid-configuration.json\n- scope: profile\n  description: Access to\
  \ basic profile claims (name, preferred_username, updated_at).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/limitless-openid-configuration.json\n- scope: email\n  description: Access to the email and email_verified claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/limitless-openid-configuration.json\n- scope: lifelogs:read\n  description: >-\n    Read access to the authenticated user's lifelogs - the Pendant recordings,\n    transcripts, and structured contents exposed by GET /v1/lifelogs and\n    GET /v1/lifelogs/{id}. This is the only resource-level scope Limitless advertises;\n    note that the REST API's DELETE operations have no corresponding write/delete scope,\n    which implies deletion is only reachable with an X-API-Key, not an OAuth token.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/limitless-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limitless/refs/heads/main/scopes/limitless-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Artificial Intelligence
- Wearables
- Voice
- Transcription
- Personal Data
- Consumer Hardware
- Search
- Productivity
- Meeting Notes
- Model Context Protocol
token_urls:
- https://api.limitless.ai/api/auth/token
---
