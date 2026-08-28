---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Simspace Scopes
name_suffix: OAuth Scopes
note: The only OAuth scope surface SimSpace publishes anonymously is the one declared in its RFC 8414 authorization-server metadata and echoed in its RFC 9728 protected-resource metadata. It carries a single scope. SimSpace publishes no scopes or permissions reference page for the platform API; if the platform API uses scopes, they are documented only inside the authenticated portal.
overview: 'SimSpace uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SimSpace
provider_slug: simspace
schemes:
- authorization_url: https://simspace.com/oauth/authorize
  name: oauth2-mcp
  source: https://simspace.com/.well-known/oauth-authorization-server
  token_url: https://simspace.com/oauth/token
scope_count: 0
scope_names: []
scopes: []
slug: simspace-scopes
source_filename: simspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://simspace.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  The only OAuth scope surface SimSpace publishes anonymously is the one declared in\n  its RFC 8414 authorization-server metadata and echoed in its RFC 9728\n  protected-resource metadata. It carries a single scope. SimSpace publishes no scopes\n  or permissions reference page for the platform API; if the platform API uses scopes,\n  they are documented only inside the authenticated portal.\nschemes:\n- name: oauth2-mcp\n  source: https://simspace.com/.well-known/oauth-authorization-server\n  authorization_url: https://simspace.com/oauth/authorize\n  token_url: https://simspace.com/oauth/token\nscopes:\n- name: mcp\n  description: Access the MCP server surface at https://simspace.com/wp-json/mcp/mcp-oauth-server\n  source: scopes_supported in RFC 8414 authorization-server metadata and RFC 9728\n    protected-resource metadata\n  applies_to: https://simspace.com/wp-json/mcp/mcp-oauth-server\n\
  scope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simspace/refs/heads/main/scopes/simspace-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cybersecurity
- Cyber Range
- Security Training
- Simulation
- AI Agents
- Security Operations
- Critical Infrastructure
- Government
- Compliance
token_urls: []
---
