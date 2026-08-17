---
authorization_urls: []
description: The complete published scope vocabulary for SocialBee's OAuth 2.1 authorization server. Both the RFC 8414 authorization server metadata and the RFC 9728 protected resource metadata declare a single scope, "mcp". There is no scopes or permissions reference page — SocialBee does not document this authorization server at all, so the metadata document is the only source.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Socialbee Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SocialBee uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SocialBee
provider_slug: socialbee
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: socialbee-scopes
source_filename: socialbee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://socialbee.com/.well-known/oauth-authorization-server\nname: SocialBee OAuth Scopes\ndescription: >-\n  The complete published scope vocabulary for SocialBee's OAuth 2.1 authorization\n  server. Both the RFC 8414 authorization server metadata and the RFC 9728\n  protected resource metadata declare a single scope, \"mcp\". There is no scopes\n  or permissions reference page — SocialBee does not document this authorization\n  server at all, so the metadata document is the only source.\ndocs: null\n\nscopes:\n  - name: mcp\n    description: >-\n      The only scope advertised by the authorization server. Grants access to the\n      Model Context Protocol server at\n      https://socialbee.com/wp-json/mcp/mcp-oauth-server. No finer-grained\n      scope vocabulary is published, so this is an all-or-nothing grant for the\n      MCP resource.\n    source: metadata\n    resource: https://socialbee.com/wp-json/mcp/mcp-oauth-server\n\
  \ngranularity:\n  level: coarse\n  read_write_split: false\n  resource_scoped: false\n  note: >-\n    A single opaque scope with no read/write or per-resource separation. An agent\n    cannot request least privilege: consenting to \"mcp\" consents to whatever the\n    server's full tool set does. Whether that set is read-only cannot be\n    determined without an authenticated tools/list.\n\nsummary:\n  scope_count: 1\n  source_of_truth: RFC 8414 authorization server metadata\n  documented_by_provider: false\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n    - url: https://socialbee.com/.well-known/oauth-authorization-server\n      http_status: 200\n      field: scopes_supported\n      value: [\"mcp\"]\n    - url: https://socialbee.com/.well-known/oauth-protected-resource\n      http_status: 200\n      field: scopes_supported\n      value: [\"mcp\"]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socialbee/refs/heads/main/scopes/socialbee-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Social Media Management
- Content Scheduling
- Content Recycling
- Social Media Analytics
- AI Caption Generation
- Social Media Publishing
- Model Context Protocol
- Marketing Automation
- SaaS
token_urls: []
---
