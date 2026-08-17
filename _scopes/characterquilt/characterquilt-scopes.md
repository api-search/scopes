---
api_specs:
- filename: characterquilt-branding-api-openapi.yml
  format: yaml
  label: CharacterQuilt Branding API
  slug: characterquilt-branding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/characterquilt/refs/heads/main/openapi/characterquilt-branding-api-openapi.yml
- filename: characterquilt-discovery-api-openapi.yml
  format: yaml
  label: CharacterQuilt Discovery API
  slug: characterquilt-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/characterquilt/refs/heads/main/openapi/characterquilt-discovery-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Characterquilt Scopes
name_suffix: OAuth Scopes
note: 'Scopes read verbatim from CharacterQuilt''s own RFC 9728 OAuth Protected Resource Metadata document, served at the MCP host and returned HTTP 200 with content-type application/json. CharacterQuilt publishes no scope reference page, so the descriptions below are read from the scope names themselves and are marked as such — nothing here is invented beyond naming what a read:/write:/publish: verb on a named resource means. The scopes are NOT declared in any OpenAPI securityScheme; the protected-resource metadata is the only place they appear.'
overview: 'CharacterQuilt uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CharacterQuilt
provider_slug: characterquilt
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: characterquilt-scopes
source_filename: characterquilt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.characterquilt.com/.well-known/oauth-protected-resource\ndocs: null\nnote: >-\n  Scopes read verbatim from CharacterQuilt's own RFC 9728 OAuth Protected Resource\n  Metadata document, served at the MCP host and returned HTTP 200 with\n  content-type application/json. CharacterQuilt publishes no scope reference page,\n  so the descriptions below are read from the scope names themselves and are marked\n  as such — nothing here is invented beyond naming what a read:/write:/publish: verb\n  on a named resource means. The scopes are NOT declared in any OpenAPI\n  securityScheme; the protected-resource metadata is the only place they appear.\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://mcp.characterquilt.com/.well-known/oauth-protected-resource\n  http_status: 200\n  content_type: application/json\n  raw_file: well-known/characterquilt-oauth-protected-resource.json\nresource: https://mcp.characterquilt.com/api/mcp\n\
  authorization_servers:\n- https://characterquilt-review-beta.vercel.app\nbearer_methods_supported:\n- header\nscope_count: 5\nscopes:\n- name: read:design_brain\n  access: read\n  resource: design_brain\n  description: >-\n    Read access to the \"design brain\" — CharacterQuilt's per-customer brand model\n    (the brand/creative knowledge its Design Agent operates from). Scope name is\n    published; CharacterQuilt documents no per-scope reference.\n- name: write:generated_artifacts\n  access: write\n  resource: generated_artifacts\n  description: >-\n    Write access to generated artifacts — the creative output the agents produce\n    (emails, ads, landing pages, one-pagers, decks).\n- name: publish:public_file\n  access: publish\n  resource: public_file\n  description: >-\n    Publish a file to a public location. The only scope whose verb is neither read\n    nor write, and the one with an externally visible consequence.\n- name: read:agent_work\n  access: read\n  resource: agent_work\n\
  \  description: Read access to agent work — the runs/tasks the agents execute.\n- name: write:agent_work\n  access: write\n  resource: agent_work\n  description: Write access to agent work — creating or modifying agent runs/tasks.\ngaps:\n- issue: no-scope-reference-page\n  detail: >-\n    No public documentation maps these scopes to operations, so a client cannot\n    determine least privilege for a given task. The scope strings are only\n    discoverable by reading the protected-resource metadata.\n- issue: authorization-server-metadata-missing\n  detail: >-\n    authorization_servers names https://characterquilt-review-beta.vercel.app — a\n    Vercel preview deployment — and that host does NOT serve RFC 8414\n    authorization-server metadata: both /.well-known/oauth-authorization-server and\n    /.well-known/openid-configuration return HTTP 200 with the Next.js HTML app\n    shell, not JSON. The OAuth discovery chain therefore terminates: an MCP client\n    that follows the WWW-Authenticate\
  \ resource_metadata pointer correctly cannot\n    reach an authorization endpoint. Probed 2026-08-13.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/characterquilt/refs/heads/main/scopes/characterquilt-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Artificial Intelligence
- AI Agents
- Marketing Automation
- Campaign Management
- Brand Identity
- Computer Use Agents
- Y Combinator
- Data
- MCP
token_urls: []
---
