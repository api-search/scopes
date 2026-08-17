---
authorization_urls:
- https://app.ringdna.com/mcp/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Revenue Io Scopes
name_suffix: OAuth Scopes
note: Derived from live RFC 8414 authorization-server metadata, not from an OpenAPI — Revenue.io publishes no machine-readable spec. Revenue.io publishes no scopes or permissions reference page in its knowledge center; the single scope below is everything the provider advertises. A granular scope model, if one exists behind the OAuth flow, is not published.
overview: 'Revenue.io publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Revenue.io API on a user''s behalf.


  Tokens are issued from https://app.ringdna.com/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Revenue.io
provider_slug: revenue-io
schemes:
- flows:
  - authorizationUrl: https://app.ringdna.com/mcp/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://app.ringdna.com/mcp/oauth/token
  issuer: https://app.ringdna.com
  name: mcp-oauth2
  source: well-known/revenue-io-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: 'The only value in scopes_supported. Advertised by both the authorization server metadata and the protected-resource metadata for https://app.ringdna.com/mcp. Coarse-grained: one scope covers the entire MCP tool surface, with no read/write or per-resource separation published.'
  flows:
  - authorizationCode
  scope: mcp
slug: revenue-io-scopes
source_filename: revenue-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.revenue.io/.well-known/oauth-authorization-server\nnote: >-\n  Derived from live RFC 8414 authorization-server metadata, not from an OpenAPI —\n  Revenue.io publishes no machine-readable spec. Revenue.io publishes no scopes\n  or permissions reference page in its knowledge center; the single scope below\n  is everything the provider advertises. A granular scope model, if one exists\n  behind the OAuth flow, is not published.\nschemes:\n  - name: mcp-oauth2\n    source: well-known/revenue-io-oauth-authorization-server.json\n    issuer: https://app.ringdna.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.ringdna.com/mcp/oauth/authorize\n        tokenUrl: https://app.ringdna.com/mcp/oauth/token\n        pkce: S256\nscopes:\n  - scope: mcp\n    description: >-\n      The only value in scopes_supported. Advertised by both the authorization\n      server metadata and the protected-resource\
  \ metadata for\n      https://app.ringdna.com/mcp. Coarse-grained: one scope covers the entire\n      MCP tool surface, with no read/write or per-resource separation published.\n    flows: [authorizationCode]\n    sources:\n      - well-known/revenue-io-oauth-authorization-server.json\n      - well-known/revenue-io-oauth-protected-resource.json\nsummary:\n  scope_count: 1\n  granularity: coarse\n  docs_page: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revenue-io/refs/heads/main/scopes/revenue-io-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Revenue Intelligence
- Sales Engagement
- Conversation Intelligence
- RevOps
- Call Analytics
- Real-Time Guidance
- CRM Integration
- Salesforce
token_urls:
- https://app.ringdna.com/mcp/oauth/token
---
