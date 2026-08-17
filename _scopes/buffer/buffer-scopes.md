---
authorization_urls:
- https://auth.buffer.com/auth
description: ''
docs: https://developers.buffer.com/guides/authentication.html#scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Buffer Scopes
name_suffix: OAuth Scopes
note: Two sources disagree in a useful way and both are recorded. Buffer's published Scopes table in the authentication guide lists SEVEN scopes. The live RFC 8414 / OIDC discovery documents advertise TEN — the same seven plus insights:read, engagements:read and engagements:write, which are undocumented in the guide. The MCP server's RFC 9728 protected-resource metadata advertises nine (the ten minus offline_access, which is not a resource permission). Every scope below carries which source names it. Personal API keys have NO scope model at all — Buffer states the key is account-based and reaches everything the account can see — so scopes apply only to the OAuth path.
overview: 'Buffer publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Buffer API on a user''s behalf.


  Tokens are issued from https://auth.buffer.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Buffer
provider_slug: buffer
schemes:
- flows:
  - authorizationUrl: https://auth.buffer.com/auth
    flow: authorizationCode
    pkce: S256 required
    tokenUrl: https://auth.buffer.com/token
  name: OAuth2AuthorizationCodePKCE
  source: https://auth.buffer.com/.well-known/oauth-authorization-server
scope_count: 11
scope_names:
- posts:read
- posts:write
- ideas:read
- ideas:write
- account:read
- account:write
- offline_access
- insights:read
- engagements:read
- engagements:write
- openid
scopes:
- description: View posts and queue.
  flows:
  - authorizationCode
  scope: posts:read
- description: Create and manage posts on the user's behalf.
  flows:
  - authorizationCode
  scope: posts:write
- description: View ideas.
  flows:
  - authorizationCode
  scope: ideas:read
- description: Create and manage ideas on the user's behalf.
  flows:
  - authorizationCode
  scope: ideas:write
- description: View account information.
  flows:
  - authorizationCode
  scope: account:read
- description: Update account settings.
  flows:
  - authorizationCode
  scope: account:write
- description: Receive a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Not described by Buffer. Advertised by the authorization server and by the MCP protected-resource metadata. By name it maps to the analytics surface Buffer ships as Insights (Post.metrics, aggregatedPostMetrics).
  flows:
  - authorizationCode
  scope: insights:read
- description: Not described by Buffer. Advertised by the authorization server and by the MCP protected-resource metadata. By name it maps to Buffer's comments/community engagement product; the roadmap carries a "Community API" item for automating comment replies, still in Exploring.
  flows:
  - authorizationCode
  scope: engagements:read
- description: Not described by Buffer. Advertised by the authorization server and by the MCP protected-resource metadata.
  flows:
  - authorizationCode
  scope: engagements:write
- description: Standard OIDC scope, advertised only by the OpenID discovery document.
  flows:
  - authorizationCode
  scope: openid
slug: buffer-scopes
source_filename: buffer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://auth.buffer.com/.well-known/oauth-authorization-server\ndocs: https://developers.buffer.com/guides/authentication.html#scopes\nnote: >-\n  Two sources disagree in a useful way and both are recorded. Buffer's\n  published Scopes table in the authentication guide lists SEVEN scopes. The\n  live RFC 8414 / OIDC discovery documents advertise TEN — the same seven plus\n  insights:read, engagements:read and engagements:write, which are\n  undocumented in the guide. The MCP server's RFC 9728 protected-resource\n  metadata advertises nine (the ten minus offline_access, which is not a\n  resource permission). Every scope below carries which source names it.\n  Personal API keys have NO scope model at all — Buffer states the key is\n  account-based and reaches everything the account can see — so scopes apply\n  only to the OAuth path.\nschemes:\n  - name: OAuth2AuthorizationCodePKCE\n    source: https://auth.buffer.com/.well-known/oauth-authorization-server\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.buffer.com/auth\n        tokenUrl: https://auth.buffer.com/token\n        pkce: S256 required\nscopes:\n  - scope: posts:read\n    description: View posts and queue.\n    flows: [authorizationCode]\n    sources: [docs, oauth-authorization-server, openid-configuration, oauth-protected-resource]\n    documented: true\n  - scope: posts:write\n    description: Create and manage posts on the user's behalf.\n    flows: [authorizationCode]\n    sources: [docs, oauth-authorization-server, openid-configuration, oauth-protected-resource]\n    documented: true\n  - scope: ideas:read\n    description: View ideas.\n    flows: [authorizationCode]\n    sources: [docs, oauth-authorization-server, openid-configuration, oauth-protected-resource]\n    documented: true\n  - scope: ideas:write\n    description: Create and manage ideas on the user's behalf.\n    flows: [authorizationCode]\n    sources: [docs, oauth-authorization-server,\
  \ openid-configuration, oauth-protected-resource]\n    documented: true\n  - scope: account:read\n    description: View account information.\n    flows: [authorizationCode]\n    sources: [docs, oauth-authorization-server, openid-configuration, oauth-protected-resource]\n    documented: true\n  - scope: account:write\n    description: Update account settings.\n    flows: [authorizationCode]\n    sources: [docs, oauth-authorization-server, openid-configuration, oauth-protected-resource]\n    documented: true\n  - scope: offline_access\n    description: Receive a refresh token for long-lived access.\n    flows: [authorizationCode]\n    sources: [docs, oauth-authorization-server, openid-configuration]\n    documented: true\n    note: >-\n      Not advertised by the MCP protected-resource metadata, which lists only\n      resource permissions.\n  - scope: insights:read\n    description: >-\n      Not described by Buffer. Advertised by the authorization server and by\n      the MCP protected-resource\
  \ metadata. By name it maps to the analytics\n      surface Buffer ships as Insights (Post.metrics, aggregatedPostMetrics).\n    flows: [authorizationCode]\n    sources: [oauth-authorization-server, openid-configuration, oauth-protected-resource]\n    documented: false\n  - scope: engagements:read\n    description: >-\n      Not described by Buffer. Advertised by the authorization server and by\n      the MCP protected-resource metadata. By name it maps to Buffer's\n      comments/community engagement product; the roadmap carries a \"Community\n      API\" item for automating comment replies, still in Exploring.\n    flows: [authorizationCode]\n    sources: [oauth-authorization-server, openid-configuration, oauth-protected-resource]\n    documented: false\n  - scope: engagements:write\n    description: >-\n      Not described by Buffer. Advertised by the authorization server and by\n      the MCP protected-resource metadata.\n    flows: [authorizationCode]\n    sources: [oauth-authorization-server,\
  \ openid-configuration, oauth-protected-resource]\n    documented: false\n  - scope: openid\n    description: Standard OIDC scope, advertised only by the OpenID discovery document.\n    flows: [authorizationCode]\n    sources: [openid-configuration]\n    documented: false\ngaps:\n  - >-\n    There is no scope model for personal API keys. Buffer's roadmap carries\n    \"API permissions / scopes — Create restricted API keys with limited\n    capabilities\" in the Exploring column, which is the provider's own\n    acknowledgement of this gap.\n  - >-\n    insights:read, engagements:read and engagements:write are live on the\n    authorization server but absent from the published Scopes table.\nx-evidence:\n  - {fetched: '2026-08-13', url: 'https://auth.buffer.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {fetched: '2026-08-13', url: 'https://mcp.buffer.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {fetched: '2026-08-13', url: 'https://developers.buffer.com/guides/authentication.html',\
  \ http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buffer/refs/heads/main/scopes/buffer-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Social Media
- Scheduling
- Analytics
- Publishing
- Content Management
- Social Media Management
- Social Media Marketing
- Marketing
- Content Scheduling
- GraphQL
- MCP
- Agents
token_urls:
- https://auth.buffer.com/token
---
