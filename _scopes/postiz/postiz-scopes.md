---
api_specs:
- filename: postiz-analytics-api-openapi.yml
  format: yaml
  label: Postiz Analytics API
  slug: postiz-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-analytics-api-openapi.yml
- filename: postiz-integrations-api-openapi.yml
  format: yaml
  label: Postiz Integrations API
  slug: postiz-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-integrations-api-openapi.yml
- filename: postiz-notifications-api-openapi.yml
  format: yaml
  label: Postiz Notifications API
  slug: postiz-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-notifications-api-openapi.yml
- filename: postiz-posts-api-openapi.yml
  format: yaml
  label: Postiz Posts API
  slug: postiz-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-posts-api-openapi.yml
- filename: postiz-uploads-api-openapi.yml
  format: yaml
  label: Postiz Uploads API
  slug: postiz-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-uploads-api-openapi.yml
- filename: postiz-public-api-openapi.json
  format: json
  label: Postiz Public API
  slug: postiz-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-public-api-openapi.json
- filename: postiz-platform-swagger-openapi.json
  format: json
  label: Postiz Platform API
  slug: postiz-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-platform-swagger-openapi.json
authorization_urls:
- https://platform.postiz.com/oauth/authorize
description: ''
docs: https://docs.postiz.com/public-api/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Postiz Scopes
name_suffix: OAuth Scopes
note: 'The Postiz OpenAPI documents apiKey auth only and declares no oauth2 securityScheme, so derive-oauth-scopes.py found nothing. Postiz nevertheless runs a real OAuth 2.0 authorization-code flow, and its MCP resource publishes RFC 8414 and RFC 9728 discovery documents that name the scopes. Those two documents — fetched live and saved verbatim under well-known/ — are the authoritative scope source, not the spec. The Public API OAuth docs page describes the same flow for third-party apps but does not document a scope parameter: consent is app-wide, tokens are prefixed pos_ and do not expire, and users revoke them from Settings > Approved Apps.'
overview: 'Postiz publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Postiz API on a user''s behalf.


  Tokens are issued from https://api.postiz.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Postiz
provider_slug: postiz
schemes:
- flows:
  - authorizationUrl: https://platform.postiz.com/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    pkce:
    - S256
    response_types:
    - code
    tokenUrl: https://api.postiz.com/oauth/token
  issuer: https://api.postiz.com/mcp-oauth
  name: PostizOAuth2
  source: https://api.postiz.com/.well-known/oauth-authorization-server/mcp-oauth
  type: oauth2
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access through the Postiz MCP resource — listing channels, groups, platform settings schemas and scheduled posts.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access through the Postiz MCP resource — scheduling, drafting and publishing posts, updating post settings, and generating images and video.
  flows:
  - authorizationCode
  scope: mcp:write
slug: postiz-scopes
source_filename: postiz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.postiz.com/.well-known/oauth-protected-resource/mcp-oauth\ndocs: https://docs.postiz.com/public-api/oauth\nnote: >-\n  The Postiz OpenAPI documents apiKey auth only and declares no oauth2 securityScheme,\n  so derive-oauth-scopes.py found nothing. Postiz nevertheless runs a real OAuth 2.0\n  authorization-code flow, and its MCP resource publishes RFC 8414 and RFC 9728\n  discovery documents that name the scopes. Those two documents — fetched live and\n  saved verbatim under well-known/ — are the authoritative scope source, not the spec.\n  The Public API OAuth docs page describes the same flow for third-party apps but does\n  not document a scope parameter: consent is app-wide, tokens are prefixed pos_ and\n  do not expire, and users revoke them from Settings > Approved Apps.\nschemes:\n- name: PostizOAuth2\n  type: oauth2\n  source: https://api.postiz.com/.well-known/oauth-authorization-server/mcp-oauth\n  issuer:\
  \ https://api.postiz.com/mcp-oauth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.postiz.com/oauth/authorize\n    tokenUrl: https://api.postiz.com/oauth/token\n    pkce: [S256]\n    response_types: [code]\n    grant_types: [authorization_code]\nscopes:\n- scope: mcp:read\n  description: >-\n    Read access through the Postiz MCP resource — listing channels, groups, platform\n    settings schemas and scheduled posts.\n  flows: [authorizationCode]\n  resource: https://api.postiz.com/mcp-oauth\n  sources: [well-known/postiz-oauth-protected-resource-mcp-oauth.json, well-known/postiz-oauth-authorization-server-mcp-oauth.json]\n- scope: mcp:write\n  description: >-\n    Write access through the Postiz MCP resource — scheduling, drafting and publishing\n    posts, updating post settings, and generating images and video.\n  flows: [authorizationCode]\n  resource: https://api.postiz.com/mcp-oauth\n  sources: [well-known/postiz-oauth-protected-resource-mcp-oauth.json,\
  \ well-known/postiz-oauth-authorization-server-mcp-oauth.json]\npublic_api_scopes:\n  documented: false\n  note: >-\n    The two scopes above govern the MCP resource. For the Public API itself, Postiz\n    documents no scope parameter on /oauth/authorize — an approved app receives a\n    pos_ token that works against every Public API endpoint. Recorded as an honest\n    absence rather than inferred scopes.\nx-evidence:\n- {url: 'https://api.postiz.com/.well-known/oauth-protected-resource/mcp-oauth', status: 200, fetched: '2026-08-13'}\n- {url: 'https://api.postiz.com/.well-known/oauth-authorization-server/mcp-oauth', status: 200, fetched: '2026-08-13'}\n- {url: 'https://docs.postiz.com/public-api/oauth', status: 200, fetched: '2026-08-13'}\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/scopes/postiz-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Social-Media
- Scheduling
- Open-Source
- Content
- Marketing
- Agents
- MCP
- Automation
- Publishing
- Analytics
token_urls:
- https://api.postiz.com/oauth/token
---
