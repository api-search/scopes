---
api_specs:
- filename: chirpie-ai-openapi-generated.yml
  format: yaml
  label: Chirpie API
  slug: chirpie-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chirpie-ai/openapi/_ae-authored/chirpie-ai-openapi-generated.yml
authorization_urls: []
description: ''
docs: https://chirpie.ai/docs/authentication#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Chirpie Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Chirpie publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Chirpie API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chirpie
provider_slug: chirpie-ai
schemes: []
scope_count: 9
scope_names:
- posts:read
- posts:write
- accounts:read
- accounts:write
- analytics:read
- comments:read
- comments:write
- media:write
- keys:write
scopes:
- description: Read posts, threads and drafts
  flows: []
  scope: posts:read
- description: Create, edit, schedule, delete, hide and unhide posts and threads
  flows: []
  scope: posts:write
- description: List connected social accounts
  flows: []
  scope: accounts:read
- description: Connect, reconnect, deactivate and disconnect social accounts
  flows: []
  scope: accounts:write
- description: Read post metrics
  flows: []
  scope: analytics:read
- description: Read comments on posts
  flows: []
  scope: comments:read
- description: Reply to, hide and delete comments
  flows: []
  scope: comments:write
- description: Upload media
  flows: []
  scope: media:write
- description: Create, list and revoke API keys
  flows: []
  scope: keys:write
slug: chirpie-ai-scopes
source_filename: chirpie-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chirpie.ai/docs/authentication.md\ndocs: https://chirpie.ai/docs/authentication#scopes\nmechanism: 'API-key scopes (not OAuth2): a key created without scopes (scopes: null) has full access; named scopes\n  narrow it. A key can never grant a scope it does not hold (403 insufficient_scope). There is no keys:read.'\nscopes:\n- name: posts:read\n  description: Read posts, threads and drafts\n- name: posts:write\n  description: Create, edit, schedule, delete, hide and unhide posts and threads\n- name: accounts:read\n  description: List connected social accounts\n- name: accounts:write\n  description: Connect, reconnect, deactivate and disconnect social accounts\n- name: analytics:read\n  description: Read post metrics\n- name: comments:read\n  description: Read comments on posts\n- name: comments:write\n  description: Reply to, hide and delete comments\n- name: media:write\n  description: Upload media\n- name: keys:write\n\
  \  description: Create, list and revoke API keys\n"
source_yaml_url: https://artifacts.apis.io/chirpie-ai/scopes/chirpie-ai-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Social Media
- Social Media Posting
- Scheduling
- MCP
- AI Agents
- Analytics
token_bound: false
token_urls: []
---
