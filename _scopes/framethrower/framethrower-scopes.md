---
api_specs:
- filename: framethrower-openapi.yml
  format: yaml
  label: FrameThrower API
  slug: framethrower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/openapi/framethrower-openapi.yml
authorization_urls: []
description: ''
docs: https://github.com/framethrower-ai/framethrower-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Framethrower Scopes
name_suffix: OAuth Scopes
note: Scopes are the OpenID Connect standard set advertised by the MCP authorization server; the REST API uses personal bearer tokens with no scopes.
overview: 'FrameThrower uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FrameThrower
provider_slug: framethrower
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: framethrower-scopes
source_filename: framethrower-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: https://framethrower.ai/.well-known/oauth-authorization-server\ndocs: https://github.com/framethrower-ai/framethrower-mcp\nnote: Scopes are the OpenID Connect standard set advertised by the MCP authorization server; the REST API uses personal bearer tokens with no scopes.\nscopes:\n- name: openid\n  surface: mcp\n- name: profile\n  surface: mcp\n- name: email\n  surface: mcp\n- name: offline_access\n  surface: mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/scopes/framethrower-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Film
- Cinematography
- Visual Reference
- Image Search
- Media
- Creative Tools
- MCP
- Agent-Native
token_urls: []
---
