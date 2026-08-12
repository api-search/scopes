---
authorization_urls:
- https://tweetapi.com/dashboard/mcp/authorize
description: ''
docs: https://tweetapi.com/docs/getting-started/agents
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Tweetapi Scopes
name_suffix: OAuth Scopes
note: Read from live RFC 8414 / RFC 9728 discovery documents, not from an OpenAPI oauth2 securityScheme — TweetAPI publishes no OpenAPI. The REST API is API-key authenticated and has no scope surface at all; scopes exist only on the MCP OAuth boundary.
overview: 'TweetAPI publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TweetAPI API on a user''s behalf.


  Tokens are issued from https://tweetapi.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TweetAPI
provider_slug: tweetapi
schemes:
- flows:
  - authorizationUrl: https://tweetapi.com/dashboard/mcp/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://tweetapi.com/api/oauth/token
  issuer: https://tweetapi.com
  name: TweetAPIOAuth
  source: https://tweetapi.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- tweetapi:read
- offline_access
scopes:
- description: Read-only access through the hosted MCP server — TweetAPI documentation tools and live public-data lookups. Excludes posting, engagement, account-secret, DM, billing and administration operations.
  flows:
  - authorizationCode
  scope: tweetapi:read
- description: Issue a refresh token so an agent client can maintain the authorization across sessions without re-running the dashboard flow.
  flows:
  - authorizationCode
  scope: offline_access
slug: tweetapi-scopes
source_filename: tweetapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://tweetapi.com/.well-known/oauth-authorization-server\ncorroborating_source: https://mcp.tweetapi.com/.well-known/oauth-protected-resource/mcp\ndocs: https://tweetapi.com/docs/getting-started/agents\napplies_to: TweetAPI Hosted MCP Server (https://mcp.tweetapi.com/mcp)\nnote: >-\n  Read from live RFC 8414 / RFC 9728 discovery documents, not from an OpenAPI oauth2 securityScheme —\n  TweetAPI publishes no OpenAPI. The REST API is API-key authenticated and has no scope surface at\n  all; scopes exist only on the MCP OAuth boundary.\nschemes:\n  - name: TweetAPIOAuth\n    issuer: https://tweetapi.com\n    source: https://tweetapi.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://tweetapi.com/dashboard/mcp/authorize\n        tokenUrl: https://tweetapi.com/api/oauth/token\n        code_challenge_methods: [S256]\nscopes:\n  - scope: tweetapi:read\n    description:\
  \ >-\n      Read-only access through the hosted MCP server — TweetAPI documentation tools and live\n      public-data lookups. Excludes posting, engagement, account-secret, DM, billing and\n      administration operations.\n    flows: [authorizationCode]\n    sources: [https://tweetapi.com/.well-known/oauth-authorization-server, https://mcp.tweetapi.com/.well-known/oauth-protected-resource/mcp]\n  - scope: offline_access\n    description: >-\n      Issue a refresh token so an agent client can maintain the authorization across sessions\n      without re-running the dashboard flow.\n    flows: [authorizationCode]\n    sources: [https://tweetapi.com/.well-known/oauth-authorization-server, https://mcp.tweetapi.com/.well-known/oauth-protected-resource/mcp]\nscope_count: 2\ngranularity: coarse\ngaps:\n  - >-\n    A single read scope covers the entire read surface — an agent authorized for a user lookup is\n    equally authorized for search, lists, communities and Spaces. There is no per-resource\
  \ or\n    per-category scope, and no write scope exists because writes are excluded from MCP entirely.\n  - No published scopes reference page; the scope strings are discoverable only from the metadata documents.\nx-evidence:\n  - {url: 'https://tweetapi.com/.well-known/oauth-authorization-server', http_status: 200, fetched: '2026-08-11'}\n  - {url: 'https://mcp.tweetapi.com/.well-known/oauth-protected-resource/mcp', http_status: 200, fetched: '2026-08-11'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tweetapi/refs/heads/main/scopes/tweetapi-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- twitter
- x
- social-media
- social-data
- search
- analytics
- research
- developer-tools
- mcp
- agent-native
- llms-txt
- rest-api
token_urls:
- https://tweetapi.com/api/oauth/token
---
