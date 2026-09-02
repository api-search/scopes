---
authorization_urls:
- https://apstal.com/api/auth/callback
description: ''
docs: https://apstal.com/auth.md
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Apstal Scopes
name_suffix: OAuth Scopes
note: 'Apstal publishes no OpenAPI, so derive-oauth-scopes.py has no spec to read. The scope list below is taken from the provider''s live RFC 8414 authorization-server metadata and its RFC 9728 protected-resource metadata, cross-checked against auth.md. Apstal publishes NO per-scope descriptions and NO scope-to-permission mapping; the descriptions below are the provider''s own wording from auth.md ("Scopes: read, write, admin") and nothing more has been inferred.'
overview: 'Apstal publishes 3 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apstal API on a user''s behalf.


  Tokens are issued from https://apstal.com/api/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apstal
provider_slug: apstal
schemes:
- flows:
  - authorizationUrl: https://apstal.com/api/auth/callback
    flow: authorizationCode
    tokenUrl: https://apstal.com/api/auth/token
  - flow: refreshToken
  issuer: https://apstal.com
  name: oauth2
  source: https://apstal.com/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- read
- write
- admin
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: read
- description: ''
  flows:
  - authorizationCode
  scope: write
- description: ''
  flows:
  - authorizationCode
  scope: admin
slug: apstal-scopes
source_filename: apstal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://apstal.com/.well-known/oauth-authorization-server\ndocs: https://apstal.com/auth.md\nnote: >-\n  Apstal publishes no OpenAPI, so derive-oauth-scopes.py has no spec to read. The scope list\n  below is taken from the provider's live RFC 8414 authorization-server metadata and its\n  RFC 9728 protected-resource metadata, cross-checked against auth.md. Apstal publishes NO\n  per-scope descriptions and NO scope-to-permission mapping; the descriptions below are the\n  provider's own wording from auth.md (\"Scopes: read, write, admin\") and nothing more has been\n  inferred.\nschemes:\n- name: oauth2\n  source: https://apstal.com/.well-known/oauth-authorization-server\n  issuer: https://apstal.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://apstal.com/api/auth/callback\n    tokenUrl: https://apstal.com/api/auth/token\n  - flow: refreshToken\nscopes:\n- scope: read\n  description: null\n  flows: [authorizationCode]\n\
  \  sources:\n  - https://apstal.com/.well-known/oauth-authorization-server\n  - https://apstal.com/.well-known/oauth-protected-resource\n- scope: write\n  description: null\n  flows: [authorizationCode]\n  sources:\n  - https://apstal.com/.well-known/oauth-authorization-server\n  - https://apstal.com/.well-known/oauth-protected-resource\n- scope: admin\n  description: null\n  flows: [authorizationCode]\n  sources:\n  - https://apstal.com/.well-known/oauth-authorization-server\n  - https://apstal.com/.well-known/oauth-protected-resource\ngaps:\n- No published scopes/permissions reference page.\n- No per-scope descriptions anywhere in the provider's public material.\n- >-\n  API keys (the credential the MCP server and the documented REST endpoints actually use) carry\n  no scope model at all; auth.md says only that \"API keys grant access to analytics query\n  endpoints (/api/analytics/*)\" while \"OAuth tokens grant access to the full API surface\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apstal/refs/heads/main/scopes/apstal-scopes.yml
summary_line: 3 scopes · authorizationCode/refreshToken
tags:
- Analytics
- Web Analytics
- Privacy
- Session Replay
- Heatmaps
- MCP
- agent-native
- Cookieless
- llms-txt
- BigQuery
- GDPR
- A2A
- Agent Skills
- Bot Detection
- Core Web Vitals
token_urls:
- https://apstal.com/api/auth/token
---
