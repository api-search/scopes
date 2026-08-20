---
authorization_urls: []
description: ''
docs: https://help.mutinyhq.com/articles/5003451538-connecting-mutiny-to-claude
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Mutiny Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mutiny uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mutiny
provider_slug: mutiny
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: mutiny-scopes
source_filename: mutiny-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.mutinyhq.com/.well-known/oauth-authorization-server\ndocs: https://help.mutinyhq.com/articles/5003451538-connecting-mutiny-to-claude\napi: Mutiny MCP Server\nauthorization_server: https://mcp.mutinyhq.com\nprotected_resource: https://mcp.mutinyhq.com\nflows:\n- type: authorization_code\n  authorization_endpoint: https://mcp.mutinyhq.com/oauth/authorize\n  token_endpoint: https://mcp.mutinyhq.com/oauth/token\n  pkce: S256\nscope_count: 5\nscopes:\n- name: read_asset_groups\n  description: >-\n    Read the caller's Mutiny asset groups — the deal rooms, landing pages, decks, proposals and other\n    customer-facing assets in the workspace. Mutiny's own connector consent screen renders this as\n    \"Read assets\".\n  consent_label: Read assets\n  access: read\n- name: create_asset_groups\n  description: >-\n    Create new Mutiny asset groups and iterate on them (generate a page/deck/proposal from a template\n    plus\
  \ conversation context, then revise sections or headlines). Consent screen: \"Create assets\".\n  consent_label: Create assets\n  access: write\n- name: publish_asset_groups\n  description: >-\n    Publish an asset group to production and return a live, shareable URL. This is the scope that makes\n    an agent's output externally visible to a prospect, so it is the highest-consequence scope in the\n    set. Consent screen: \"Publish assets\".\n  consent_label: Publish assets\n  access: write\n- name: read_library_content\n  description: >-\n    Search and list the workspace content library — logos, images, case studies and other reusable brand\n    assets, including filtering by tag. Consent screen: \"Read library content\".\n  consent_label: Read library content\n  access: read\n- name: manage_library_content\n  description: >-\n    Upload items into the content library from a URL and manage their organisation, including tagging\n    library items. Consent screen: \"Manage library content\"\
  .\n  consent_label: Manage library content\n  access: write\nnotes: >-\n  The five scope strings are read verbatim from Mutiny's RFC 8414 authorization-server metadata and are\n  repeated identically in its RFC 9728 protected-resource metadata (both saved under well-known/). The\n  human-readable consent labels are quoted from the Mutiny help-centre article on connecting Mutiny to\n  Claude. Mutiny publishes no separate scopes/permissions reference page, so the descriptions above\n  restate what each scope name plus the documented MCP capabilities cover; no scope is invented, and no\n  scope beyond these five is claimed. There is no default/implicit scope and no refresh_token grant\n  advertised — the metadata declares grant_types_supported: [authorization_code] only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutiny/refs/heads/main/scopes/mutiny-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Enterprise
- Sales
- Marketing
- Go-To-Market
- Artificial Intelligence
- AI Agents
- Sales Enablement
- Account Based Marketing
- Workflow-Automation
- MCP
token_urls: []
---
