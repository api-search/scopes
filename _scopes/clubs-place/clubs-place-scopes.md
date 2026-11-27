---
authorization_urls: []
description: ''
docs: https://clubs.place/.well-known/oauth-protected-resource/api/nippo/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CLUBS Scopes
name_suffix: OAuth Scopes
note: The same three scopes are advertised for both https://clubs.place/api/mcp and https://clubs.place/api/nippo/mcp. CLUBS publishes no scopes reference page.
overview: 'CLUBS publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CLUBS API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CLUBS
provider_slug: clubs-place
schemes: []
scope_count: 3
scope_names:
- nippo:agent:read
- nippo:report:write
- offline_access
scopes:
- description: Listed in scopes_supported of the authorization-server and protected-resource metadata; no published description.
  flows: []
  scope: nippo:agent:read
- description: Listed in scopes_supported; no published description (name indicates daily-report submission).
  flows: []
  scope: nippo:report:write
- description: Listed in scopes_supported; refresh_token is an advertised grant type.
  flows: []
  scope: offline_access
slug: clubs-place-scopes
source_filename: clubs-place-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: CLUBS OAuth scopes\ngenerated: '2026-11-04'\nmethod: probed\nsource: https://clubs.place/.well-known/oauth-authorization-server\ndocs: https://clubs.place/.well-known/oauth-protected-resource/api/nippo/mcp\nscopes:\n- name: nippo:agent:read\n  description: Listed in scopes_supported of the authorization-server and protected-resource metadata; no published description.\n- name: nippo:report:write\n  description: Listed in scopes_supported; no published description (name indicates daily-report submission).\n- name: offline_access\n  description: Listed in scopes_supported; refresh_token is an advertised grant type.\nnote: The same three scopes are advertised for both https://clubs.place/api/mcp and https://clubs.place/api/nippo/mcp. CLUBS publishes no scopes reference page.\n"
source_yaml_url: https://artifacts.apis.io/clubs-place/scopes/clubs-place-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Artificial Intelligence
- MCP
- Productivity
- Notes
- Reporting
- Japan
token_bound: false
token_urls: []
---
