---
api_specs:
- filename: snap-conversion-api-openapi.yml
  format: yaml
  label: Snap Conversion API
  slug: snap-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/openapi/snap-conversion-api-openapi.yml
- filename: snap-events-api-openapi.yml
  format: yaml
  label: Snap Events API
  slug: snap-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/openapi/snap-events-api-openapi.yml
authorization_urls: []
description: ''
docs:
- https://developers.snap.com/api/marketing-api/Ads-API/authentication
- https://developers.snap.com/marketing-api/Ads-MCP/Introduction
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Snap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Snap uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Snap
provider_slug: snap
schemes:
- authorization_endpoint: https://accounts.snapchat.com/login/oauth2/authorize
  delimiter: space
  flow: authorizationCode
  name: Marketing API OAuth
  token_endpoint: https://accounts.snapchat.com/login/oauth2/access_token
- authorization_endpoint: https://mcp.snapchat.com/authorize
  flow: authorizationCode
  issuer: https://mcp.snapchat.com/ads
  metadata: well-known/snap-oauth-authorization-server.json
  name: Snapchat Ads MCP OAuth
  pkce: S256
  token_endpoint: https://mcp.snapchat.com/token
scope_count: 0
scope_names: []
scopes: []
slug: snap-scopes
source_filename: snap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.snap.com/api/marketing-api/Ads-API/authentication\ndocs:\n  - https://developers.snap.com/api/marketing-api/Ads-API/authentication\n  - https://developers.snap.com/marketing-api/Ads-MCP/Introduction\napi: Snap\nschemes:\n  - name: Marketing API OAuth\n    flow: authorizationCode\n    authorization_endpoint: https://accounts.snapchat.com/login/oauth2/authorize\n    token_endpoint: https://accounts.snapchat.com/login/oauth2/access_token\n    delimiter: space\n  - name: Snapchat Ads MCP OAuth\n    flow: authorizationCode\n    issuer: https://mcp.snapchat.com/ads\n    authorization_endpoint: https://mcp.snapchat.com/authorize\n    token_endpoint: https://mcp.snapchat.com/token\n    pkce: S256\n    metadata: well-known/snap-oauth-authorization-server.json\n# legacy single-scheme fields retained for consumers that read them\nflow: authorizationCode\nauthorization_endpoint: https://accounts.snapchat.com/login/oauth2/authorize\n\
  token_endpoint: https://accounts.snapchat.com/login/oauth2/access_token\ndelimiter: space\nscopes:\n  - name: snapchat-marketing-api\n    description: Read and write access to the Snapchat Marketing (Ads) APIs.\n    scheme: Marketing API OAuth\n  - name: snapchat-offline-conversions-api\n    description: Read and write access to the Snapchat Conversions APIs.\n    scheme: Marketing API OAuth\n  - name: snapchat-profile-api\n    description: Read access to the Snapchat Public Profile APIs.\n    scheme: Marketing API OAuth\n  - name: snapads.read\n    description: >-\n      Read-only access to the caller's authorized Snapchat Ads data through the\n      hosted Ads MCP server. The only scope that server accepts — Snap's docs\n      warn that a client requesting its default scope set will be rejected.\n    scheme: Snapchat Ads MCP OAuth\n    added: '2026-08-13'\nnotes: >-\n  Multiple scopes are requested as a space-separated list in the `scope`\n  authorize parameter, e.g.\n  `scope=snapchat-marketing-api\
  \ snapchat-offline-conversions-api`. The granted\n  access token reflects the authorizing user's own permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snap/refs/heads/main/scopes/snap-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- Marketing
- Social-Media
- Augmented Reality
- Camera
- Authentication
- Identity
- Conversions
- Attribution
- SDK
token_urls: []
---
