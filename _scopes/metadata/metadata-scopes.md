---
api_specs:
- filename: metadata-mcp-server-openapi.json
  format: json
  label: Metadata MCP Server (MetadataONE)
  slug: metadata-mcp-server-metadataone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metadata/refs/heads/main/openapi/metadata-mcp-server-openapi.json
authorization_urls: []
description: ''
docs: https://metadata.io/developers/authentication.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Metadata Scopes
name_suffix: OAuth Scopes
note: Two distinct scope vocabularies. The seven PRODUCT scopes below are attached to API keys at mint time and gate MCP tool access. The OAuth authorization server separately advertises only the transport scopes openid and offline_access.
overview: 'Metadata uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Metadata
provider_slug: metadata
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: metadata-scopes
source_filename: metadata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://metadata.io/developers/authentication.html\ndocs: https://metadata.io/developers/authentication.html\nnote: Two distinct scope vocabularies. The seven PRODUCT scopes below are attached to API keys at mint\n  time and gate MCP tool access. The OAuth authorization server separately advertises only the transport\n  scopes openid and offline_access.\nscope_count: 7\nscopes:\n- name: read:all\n  description: All get_*, search_*, list_*, *_stats and *_insights tools\n  destructive: false\n- name: write:audiences\n  description: Create, update, archive audiences and target groups\n  destructive: false\n  note: documented as reversible\n- name: write:creatives\n  description: Generate or upload creatives, build ads\n  destructive: false\n- name: write:campaigns\n  description: Create and edit campaigns in Draft, excluding launch\n  destructive: false\n- name: launch:campaigns\n  description: launch_campaign, manage_campaign\
  \ — real spend begins\n  destructive: true\n- name: write:integrations\n  description: Connect and disconnect ad channels and CRMs\n  destructive: true\n- name: admin:*\n  description: Account impersonation, billing, user management\n  destructive: true\noauth_scopes:\n- name: openid\n  source: https://mcp-server.metadata.io/.well-known/oauth-authorization-server\n- name: offline_access\n  source: https://mcp-server.metadata.io/.well-known/oauth-authorization-server\nleast_privilege_guidance: 'Docs: \"If a key only needs analytics, do not grant launch permissions.\" The\n  Hermes config example ships with launch = false to gate launches behind human approval.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metadata/refs/heads/main/scopes/metadata-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Marketing Automation
- Demand Generation
- Advertising
- B2B
- Artificial Intelligence
- MCP
- Model Context Protocol
- AI Agents
- Paid Media
- Account Based Marketing
token_urls: []
---
