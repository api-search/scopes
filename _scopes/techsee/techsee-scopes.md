---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Techsee Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TechSee publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the TechSee API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TechSee
provider_slug: techsee
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: The only scope the authorization server advertises. It grants access to the protected resource https://techsee.com/wp-json/mcp/mcp-oauth-server — i.e. the whole MCP surface. No finer-grained scopes (read vs write, per-ability, per content type) are published, so an agent holding this scope holds everything the MCP server exposes. No description text is supplied by the provider; this note is API Evangelist's reading of the two metadata documents, not provider prose.
  flows: []
  scope: mcp
slug: techsee-scopes
source_filename: techsee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://techsee.com/.well-known/oauth-authorization-server (200, RFC 8414)\nname: TechSee\nslug: techsee\ndocs: null\ndocs_note: >-\n  TechSee publishes no scopes/permissions reference page. The scope list below is\n  read verbatim from the live OAuth 2.0 Authorization Server Metadata document and\n  is corroborated by the RFC 9728 protected-resource metadata, which advertises the\n  same single scope.\nauthorization_server: https://techsee.com\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The only scope the authorization server advertises. It grants access to the\n    protected resource https://techsee.com/wp-json/mcp/mcp-oauth-server — i.e. the\n    whole MCP surface. No finer-grained scopes (read vs write, per-ability, per\n    content type) are published, so an agent holding this scope holds everything the\n    MCP server exposes. No description text is supplied by the provider; this note\n    is API Evangelist's\
  \ reading of the two metadata documents, not provider prose.\n  source: https://techsee.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/techsee/refs/heads/main/scopes/techsee-scopes.yml
summary_line: 1 scope
tags:
- Company
- Visual Assistance
- Customer Experience
- Customer Service
- Contact Center
- Computer Vision
- Augmented Reality
- Artificial Intelligence
- Field Service
- Remote Support
- Video
- Telecommunications
token_bound: false
token_urls: []
---
