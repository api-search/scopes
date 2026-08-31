---
api_specs:
- filename: textql-v2-openapi.yml
  format: yaml
  label: TextQL v2 API
  slug: textql-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-v2-openapi.yml
- filename: textql-chat-v1-openapi.yml
  format: yaml
  label: TextQL Platform API (v1)
  slug: textql-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-chat-v1-openapi.yml
- filename: textql-platform-api-openapi.yml
  format: yaml
  label: TextQL Public RPC API
  slug: textql-public-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-platform-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.textql.com/core/how-it-works/mcp/client-setup
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Textql Scopes
name_suffix: OAuth Scopes
note: Read verbatim from TextQL's live OAuth 2.1 authorization-server metadata document, not derived from an OpenAPI securityScheme — the published OpenAPIs declare only bearer/apiKey schemes and carry no oauth2 flows, so derive-oauth-scopes.py found nothing. The scope list below is what the provider actually advertises at the discovery endpoint. Scope DESCRIPTIONS are not published; the resource each scope governs is stated from the matching platform surface and is marked as inferred where it is not spelled out in the docs.
overview: 'TextQL uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TextQL
provider_slug: textql
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: textql-scopes
source_filename: textql-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://app.textql.com/.well-known/oauth-authorization-server\ndocs: https://docs.textql.com/core/how-it-works/mcp/client-setup\nnote: >-\n  Read verbatim from TextQL's live OAuth 2.1 authorization-server metadata document, not derived from\n  an OpenAPI securityScheme — the published OpenAPIs declare only bearer/apiKey schemes and carry no\n  oauth2 flows, so derive-oauth-scopes.py found nothing. The scope list below is what the provider\n  actually advertises at the discovery endpoint. Scope DESCRIPTIONS are not published; the resource\n  each scope governs is stated from the matching platform surface and is marked as inferred where it\n  is not spelled out in the docs.\nauthorization_server: https://app.textql.com\nscope_count: 34\nscopes:\n- name: openid\n  category: identity\n  description: OpenID Connect — request an ID token.\n- name: profile\n  category: identity\n  description: Basic profile claims (name, given_name,\
  \ family_name, picture).\n- name: email\n  category: identity\n  description: Email address and verification status.\n- name: api:read\n  category: platform\n  description: Read access to the platform API.\n- name: api:write\n  category: platform\n  description: Write access to the platform API.\n- name: mcp:tools\n  category: mcp\n  description: >-\n    Call Ana's MCP tools. This is the only scope declared by the /mcp protected-resource metadata\n    document, so it is the scope an MCP client actually needs.\n- name: mcp:read\n  category: mcp\n  description: Read registered external MCP server configuration.\n- name: mcp:write\n  category: mcp\n  description: Register, toggle and delete external MCP servers in Ana's context.\n- name: agent:read\n  category: agents\n  description: Read agents (long-running monitors that watch data and post to the feed).\n- name: agent:write\n  category: agents\n  description: Create, edit and trigger agents.\n- name: chat:read\n  category: chat\n  description:\
  \ Read chats/threads, messages, cells and generated assets.\n- name: chat:write\n  category: chat\n  description: Create chats, ask questions, stream and cancel runs.\n- name: connector:read\n  category: connectors\n  description: List connectors and connector types.\n- name: connector:write\n  category: connectors\n  description: Create, test, update and delete connectors, and manage connector access grants.\n- name: connector:raw_sql\n  category: connectors\n  description: >-\n    Execute raw SQL against a connector. Broken out as its own scope because organizations can turn\n    raw SQL off entirely and query only through TQL and the Ontology.\n- name: context:read\n  category: context\n  description: Read the organization/role/personal context stack.\n- name: context:write\n  category: context\n  description: Author and edit context files.\n- name: context_policy:read\n  category: context\n  description: Read context policies.\n- name: context_policy:write\n  category: context\n  description:\
  \ Write context policies.\n- name: dashboard:read\n  category: dashboards\n  description: Read dashboards and data apps.\n- name: dashboard:write\n  category: dashboards\n  description: Create, update and publish dashboards and data apps.\n- name: dataset:read\n  category: datasets\n  description: Read datasets.\n- name: dataset:write\n  category: datasets\n  description: Create and modify datasets.\n- name: feed:read\n  category: feed\n  description: Read the shared activity feed agents and teams publish insights to.\n- name: feed:write\n  category: feed\n  description: Post to the feed.\n- name: observability:read\n  category: observability\n  description: Read observability data for the platform.\n- name: observability:write\n  category: observability\n  description: Configure observability.\n- name: ontology:read\n  category: ontology\n  description: Read the Ontology semantic layer and its pending changes.\n- name: ontology:write\n  category: ontology\n  description: Propose, approve,\
  \ deny and restore Ontology changes.\n- name: playbook:read\n  category: playbooks\n  description: Read playbooks (scheduled automated analyses).\n- name: playbook:write\n  category: playbooks\n  description: Create, update, run, deploy and delete playbooks.\n- name: sandbox:read\n  category: sandbox\n  description: Read sandcastle status, files and execution history.\n- name: sandbox:write\n  category: sandbox\n  description: Start and stop sandcastles, execute code, load data and upload files.\n- name: usage:read\n  category: billing\n  description: Read usage/consumption (ACU) data.\ninferred_descriptions: true\ninferred_note: >-\n  TextQL publishes scope NAMES at the discovery endpoint but no scope reference page with\n  descriptions. Each description above states the platform surface the scope name maps to, read from\n  the matching API reference section. The names, the count and the grouping are provider-published\n  fact; the one-line descriptions are ours.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/scopes/textql-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Artificial Intelligence
- Analytics
- Business Intelligence
- Data
- Agents
- MCP
- Semantic Layer
- Text-to-SQL
- Data Warehouse
- Enterprise
token_urls: []
---
