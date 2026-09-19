---
api_specs:
- filename: rubiconnect-campaigns-api-openapi.yml
  format: yaml
  label: RubiConnect Campaigns API
  slug: rubiconnect-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-campaigns-api-openapi.yml
- filename: rubiconnect-capabilities-api-openapi.yml
  format: yaml
  label: RubiConnect Capabilities API
  slug: rubiconnect-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-capabilities-api-openapi.yml
- filename: rubiconnect-messages-api-openapi.yml
  format: yaml
  label: RubiConnect Messages API
  slug: rubiconnect-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-messages-api-openapi.yml
- filename: rubiconnect-webhooks-api-openapi.yml
  format: yaml
  label: RubiConnect Webhooks API
  slug: rubiconnect-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Rubiconnect Scopes
name_suffix: OAuth Scopes
note: The REST OpenAPI declares only apiKey + http bearer security schemes (no oauth2 block), so no scopes are derivable from the spec. OAuth 2.0 is used by the hosted MCP server and is described only in the served authorization-server metadata, which advertises a single scope.
overview: 'RubiConnect uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RubiConnect
provider_slug: rubiconnect
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rubiconnect-scopes
source_filename: rubiconnect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: probed\nsource: https://console.rubiconnect.com/.well-known/oauth-authorization-server\nnote: >-\n  The REST OpenAPI declares only apiKey + http bearer security schemes (no oauth2 block), so no\n  scopes are derivable from the spec. OAuth 2.0 is used by the hosted MCP server and is described\n  only in the served authorization-server metadata, which advertises a single scope.\nauthorization_endpoint: https://console.rubiconnect.com/en/authorize\ntoken_endpoint: https://console.rubiconnect.com/api/oauth/token\nscopes:\n  - name: mcp\n    description: >-\n      Grants an OAuth client access to the RubiConnect hosted MCP server and its 18 messaging /\n      campaign / analytics tools, scoped to the authenticated account.\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/scopes/rubiconnect-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CPaaS
- Communications APIs
- Business Messaging
- RCS
- WhatsApp Business
- SMS
- Marketing & Campaigns
- Conversational AI
- MCP
- AI Agents
token_urls: []
---
