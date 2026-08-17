---
authorization_urls: []
description: OAuth 2.1 scopes Highspot advertises for its remote MCP server. Read directly from the two machine-readable discovery documents Highspot serves — RFC 8414 authorization server metadata on app.highspot.com and RFC 9728 protected resource metadata on mcp.highspot.com — not from prose. Both documents agree on the same three scopes. Highspot's REST API (api-{instance}.highspot.com/v1.0) does NOT use OAuth scopes; it authenticates with an API client key and secret pair, so no scope vocabulary exists for it.
docs: https://www.highspot.com/product/mcp-server/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Highspot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Highspot publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Highspot API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Highspot
provider_slug: highspot
schemes: []
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- offline_access
scopes:
- description: Read access through the Highspot MCP server — search content, retrieve items, request instant answers and analytics-backed responses.
  flows: []
  scope: mcp:read
- description: Write access through the Highspot MCP server — create linked pitches, generate Digital Rooms, and invoke Highspot Agents that take action.
  flows: []
  scope: mcp:write
- description: Issue a refresh token so an agent can keep operating without a fresh interactive authorization.
  flows: []
  scope: offline_access
slug: highspot-scopes
source_filename: highspot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Highspot OAuth Scopes\ndescription: >-\n  OAuth 2.1 scopes Highspot advertises for its remote MCP server. Read directly from\n  the two machine-readable discovery documents Highspot serves — RFC 8414\n  authorization server metadata on app.highspot.com and RFC 9728 protected resource\n  metadata on mcp.highspot.com — not from prose. Both documents agree on the same\n  three scopes. Highspot's REST API (api-{instance}.highspot.com/v1.0) does NOT use\n  OAuth scopes; it authenticates with an API client key and secret pair, so no scope\n  vocabulary exists for it.\ngenerated: '2026-08-14'\nmethod: probed\nsource: https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp\ndocs: https://www.highspot.com/product/mcp-server/\nchecked: '2026-08-14'\n\nauthorization_server:\n  issuer: https://app.highspot.com\n  metadata_url: https://app.highspot.com/.well-known/oauth-authorization-server\n  authorization_endpoint: https://app.highspot.com/oauth2/v1/authorize\n  token_endpoint:\
  \ https://app.highspot.com/auth/oauth2/v1/token\n  registration_endpoint: https://app.highspot.com/auth/oauth2/v1/register\n  grant_types_supported:\n    - authorization_code\n    - refresh_token\n  response_types_supported:\n    - code\n  token_endpoint_auth_methods_supported:\n    - client_secret_post\n    - none\n  code_challenge_methods_supported:\n    - S256\n    - plain\n\nprotected_resource:\n  resource: https://mcp.highspot.com/mcp\n  metadata_url: https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp\n  authorization_servers:\n    - https://app.highspot.com/auth/\n\nscopes:\n  - scope: mcp:read\n    description: >-\n      Read access through the Highspot MCP server — search content, retrieve items,\n      request instant answers and analytics-backed responses.\n    type: read\n    source: https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp\n  - scope: mcp:write\n    description: >-\n      Write access through the Highspot MCP server — create linked pitches,\
  \ generate\n      Digital Rooms, and invoke Highspot Agents that take action.\n    type: write\n    source: https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp\n  - scope: offline_access\n    description: >-\n      Issue a refresh token so an agent can keep operating without a fresh interactive\n      authorization.\n    type: session\n    source: https://mcp.highspot.com/.well-known/oauth-protected-resource/mcp\n\nscope_count: 3\n\nnotes:\n  - >-\n    Scope granularity is coarse: two scopes cover every read and every write across\n    content, pitches, Digital Rooms and agent invocation. There is no per-resource or\n    per-spot scope, so an agent granted mcp:write can create pitches and rooms on the\n    user's behalf with no narrower consent step.\n  - >-\n    plain is advertised alongside S256 in code_challenge_methods_supported. S256 is\n    the only method MCP clients should use.\n  - >-\n    No corresponding scope vocabulary exists for the REST API; see\n    authentication/highspot-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highspot/refs/heads/main/scopes/highspot-scopes.yml
summary_line: 3 scopes
tags:
- Sales Enablement
- Content Management
- Pitch Analytics
- CRM Integration
- Buyer Engagement
- Training
- Coaching
- AI
- MCP Server
token_urls: []
---
