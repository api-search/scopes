---
api_specs:
- filename: archbee-public-api-openapi.yml
  format: yaml
  label: Archbee Public API
  slug: archbee-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-public-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.archbee.com/docs/anthropic-claude-connector
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Archbee Scopes
name_suffix: OAuth Scopes
note: These scopes govern the remote MCP endpoint only. The REST Public API does not use OAuth — it authenticates with a bearer value the caller assembles from a space id and an API key, and has no scope concept at all. Archbee publishes no prose scopes reference page; the scope list below comes from the machine-readable metadata documents, which is why the method is probed rather than searched. Descriptions are inferred from the scope names and the tool categories in mcp/archbee-mcp.yml and are marked as such — Archbee states no description for either scope.
overview: 'Archbee uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Archbee
provider_slug: archbee
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: archbee-scopes
source_filename: archbee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://api.archbee.com/.well-known/oauth-authorization-server and\n  https://api.archbee.com/.well-known/oauth-protected-resource/api/public-mcp-ds/sse, both fetched\n  anonymously 2026-09-04 (HTTP 200). Saved verbatim under well-known/.\ndocs: https://www.archbee.com/docs/anthropic-claude-connector\nnote: >-\n  These scopes govern the remote MCP endpoint only. The REST Public API does not use OAuth — it\n  authenticates with a bearer value the caller assembles from a space id and an API key, and has no\n  scope concept at all. Archbee publishes no prose scopes reference page; the scope list below comes\n  from the machine-readable metadata documents, which is why the method is probed rather than\n  searched. Descriptions are inferred from the scope names and the tool categories in\n  mcp/archbee-mcp.yml and are marked as such — Archbee states no description for either scope.\nissuer: https://api.archbee.com\nauthorization_endpoint:\
  \ https://api.archbee.com/oauth/authorize\ntoken_endpoint: https://api.archbee.com/oauth/token\nregistration_endpoint: https://api.archbee.com/oauth/register\nrevocation_endpoint: https://api.archbee.com/oauth/revoke\nflows:\n- authorization_code\n- refresh_token\npkce:\n  required_methods:\n  - S256\ndynamic_client_registration: true\ntoken_endpoint_auth_methods:\n- none\napplies_to:\n- https://api.archbee.com/api/public-mcp-ds/sse\n- https://api.archbee.com\nscopes:\n- name: read:docs\n  description_source: inferred\n  description: >-\n    Read access to documentation content. Covers the read-category MCP tools — get_doc,\n    get_all_docs, search_query, search_title, list_templates, list_content_snippets, list_variables.\n- name: write:docs\n  description_source: inferred\n  description: >-\n    Write and delete access to documentation content. Covers the write and destructive MCP tools —\n    create_doc, update_doc, delete_doc, the space, space-group, category, template, content-snippet\n\
  \    and variable mutations.\ngaps:\n- >-\n    Two scopes cover 26 tools, and one of them covers every destructive operation including\n    delete_doc_space, which permanently removes a space and every document in it. An agent granted\n    write:docs to create a page is granted the ability to delete the workspace. There is no\n    read-only-plus-create scope, no per-resource scope, and no scope reference page in the docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/scopes/archbee-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
- Developer Portal
- Docs as Code
- OpenAPI
- Model Context Protocol
- AI Agents
- Content Management
token_urls: []
---
