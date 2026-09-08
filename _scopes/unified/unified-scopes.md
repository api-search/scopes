---
api_specs:
- filename: unified-mcp-service-openapi.json
  format: json
  label: Unified MCP Service
  slug: unified-mcp-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified/refs/heads/main/openapi/unified-mcp-service-openapi.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Unified Scopes
name_suffix: OAuth Scopes
note: Unified's authorization server advertises exactly one scope. Both the RFC 8414 authorization server metadata and the RFC 9728 protected-resource descriptor for the MCP endpoint list scopes_supported as ["openid"] and nothing else. There is no anonymous permissions or scope reference page to enrich from — docs.unified.com is behind SSO — so this is the complete published scope surface, not a partial read. Fine-grained authorization, if any, is expressed inside the customer's Unified connection rather than in OAuth scope strings.
overview: 'Unified uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unified
provider_slug: unified
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: unified-scopes
source_filename: unified-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://mcp.unified.com/.well-known/oauth-authorization-server (scopes_supported) and\n  https://mcp.unified.com/.well-known/oauth-protected-resource/mcp (scopes_supported).\n  Probed 2026-09-02.\nnote: >-\n  Unified's authorization server advertises exactly one scope. Both the RFC 8414 authorization\n  server metadata and the RFC 9728 protected-resource descriptor for the MCP endpoint list\n  scopes_supported as [\"openid\"] and nothing else. There is no anonymous permissions or scope\n  reference page to enrich from — docs.unified.com is behind SSO — so this is the complete\n  published scope surface, not a partial read. Fine-grained authorization, if any, is expressed\n  inside the customer's Unified connection rather than in OAuth scope strings.\nauthorization_server: https://mcp.unified.com/\nresource: https://mcp.unified.com/mcp\ndocs: null\nscope_count: 1\nscopes:\n- name: openid\n  description: >-\n    Advertised\
  \ verbatim in scopes_supported by both discovery documents. No description is\n    published by the provider; the OIDC-standard meaning is assumed by the name only and is not\n    asserted here.\n  source: https://mcp.unified.com/.well-known/oauth-authorization-server\n  required_for:\n  - https://mcp.unified.com/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unified/refs/heads/main/scopes/unified-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- Social Media
- Digital Advertising
- Marketing
- Analytics
- Media
- Agents
- MCP
token_urls: []
---
