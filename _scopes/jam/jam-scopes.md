---
authorization_urls:
- https://api.jam.dev/oauth/authorize
description: ''
docs: https://jam.dev/docs/personal-access-tokens
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Jam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jam publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jam API on a user''s behalf.


  Tokens are issued from https://api.jam.dev/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jam
provider_slug: jam
schemes:
- flows:
  - authorizationUrl: https://api.jam.dev/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.jam.dev/oauth/token
  name: OAuth2
  source: https://mcp.jam.dev/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access to Jam data (details, console logs, network requests, screenshots, transcripts, members, folders, recording links) via the MCP server and CLI.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access via the MCP server and CLI — create comments, move Jams between folders, create/update/revoke recording links.
  flows:
  - authorizationCode
  scope: mcp:write
slug: jam-scopes
source_filename: jam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.jam.dev/.well-known/oauth-authorization-server\ndocs: https://jam.dev/docs/personal-access-tokens\nschemes:\n  - name: OAuth2\n    source: https://mcp.jam.dev/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.jam.dev/oauth/authorize\n        tokenUrl: https://api.jam.dev/oauth/token\n        pkce: S256\nscopes:\n  - scope: mcp:read\n    description: Read access to Jam data (details, console logs, network requests, screenshots, transcripts, members, folders, recording links) via the MCP server and CLI.\n    flows: [authorizationCode]\n  - scope: mcp:write\n    description: Write access via the MCP server and CLI — create comments, move Jams between folders, create/update/revoke recording links.\n    flows: [authorizationCode]\nnotes: >-\n  Scopes are also selectable when minting Personal Access Tokens\n  (Settings -> MCP). Tokens carry the jam_pat_\
  \ prefix and are used as Bearer\n  credentials for headless/CI MCP clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jam/refs/heads/main/scopes/jam-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Developer Tools
- Bug Reporting
- Debugging
- Quality Assurance
- Observability
- Screen Recording
- Model Context Protocol
token_urls:
- https://api.jam.dev/oauth/token
---
