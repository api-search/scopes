---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Xage Scopes
name_suffix: OAuth Scopes
note: The only OAuth scope Xage publishes anywhere is the single `mcp` scope advertised in the RFC 8414 authorization server metadata and echoed in the RFC 9728 protected resource metadata for the WordPress MCP server on xage.com. No scope or permission reference exists for the Xage Fabric Platform product API — that documentation is customer-only. Nothing here was derived from a spec; there is no published OpenAPI.
overview: 'Xage uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xage
provider_slug: xage
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: xage-scopes
source_filename: xage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://xage.com/.well-known/oauth-authorization-server\nnote: >-\n  The only OAuth scope Xage publishes anywhere is the single `mcp` scope advertised in the RFC 8414\n  authorization server metadata and echoed in the RFC 9728 protected resource metadata for the\n  WordPress MCP server on xage.com. No scope or permission reference exists for the Xage Fabric\n  Platform product API — that documentation is customer-only. Nothing here was derived from a spec;\n  there is no published OpenAPI.\nauthorization_server: https://xage.com\nscopes:\n- name: mcp\n  description: >-\n    Access the Model Context Protocol server at https://xage.com/wp-json/mcp/mcp-oauth-server.\n    Advertised verbatim as the sole entry in scopes_supported; no finer-grained description is\n    published, and no per-tool scopes are declared.\n  resource: https://xage.com/wp-json/mcp/mcp-oauth-server\n  evidence: https://xage.com/.well-known/oauth-authorization-server\n\
  scope_count: 1\ndocs: null\ndocs_note: No published scopes or permissions reference page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xage/refs/heads/main/scopes/xage-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Security
- Cybersecurity
- Zero Trust
- Identity and Access Management
- Privileged Access Management
- Operational Technology
- Critical Infrastructure
- Industrial
- Agent Security
token_urls: []
---
