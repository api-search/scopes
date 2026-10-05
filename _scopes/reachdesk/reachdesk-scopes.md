---
api_specs:
- filename: reachdesk-bulk-sends-api-openapi.yml
  format: yaml
  label: Reachdesk Bulk Sends API
  slug: reachdesk-bulk-sends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-bulk-sends-api-openapi.yml
- filename: reachdesk-campaigns-api-openapi.yml
  format: yaml
  label: Reachdesk Campaigns API
  slug: reachdesk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-campaigns-api-openapi.yml
- filename: reachdesk-contacts-api-openapi.yml
  format: yaml
  label: Reachdesk Contacts API
  slug: reachdesk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-contacts-api-openapi.yml
- filename: reachdesk-gdpr-api-openapi.yml
  format: yaml
  label: Reachdesk Gdpr API
  slug: reachdesk-gdpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-gdpr-api-openapi.yml
- filename: reachdesk-organization-api-openapi.yml
  format: yaml
  label: Reachdesk Organization API
  slug: reachdesk-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-organization-api-openapi.yml
- filename: reachdesk-sends-api-openapi.yml
  format: yaml
  label: Reachdesk Sends API
  slug: reachdesk-sends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-sends-api-openapi.yml
- filename: reachdesk-transactions-api-openapi.yml
  format: yaml
  label: Reachdesk Transactions API
  slug: reachdesk-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-transactions-api-openapi.yml
authorization_urls: []
description: Reachdesk publishes exactly two OAuth scopes, and they belong to its remote MCP server rather than to its REST API. They are read from the provider's own RFC 8414 authorization-server metadata and its RFC 9728 protected-resource metadata, which agree. The REST API has no scope model at all — it authenticates with a single organization-wide API token that carries every permission the organization has.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Reachdesk Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Reachdesk publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Reachdesk API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reachdesk
provider_slug: reachdesk
schemes: []
scope_count: 2
scope_names:
- mcp:tools.user.read
- mcp:tools.user.write
scopes:
- description: Read access to MCP tools acting on behalf of the authenticated Reachdesk user. Description is inferred from the scope name — Reachdesk publishes the scope string with no human-readable description and no scopes reference page. Advertised in both scopes_supported lists.
  flows: []
  scope: mcp:tools.user.read
- description: Write access to MCP tools acting on behalf of the authenticated Reachdesk user. Description inferred from the scope name; not documented by the provider.
  flows: []
  scope: mcp:tools.user.write
slug: reachdesk-scopes
source_filename: reachdesk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.reachdesk.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  Reachdesk publishes exactly two OAuth scopes, and they belong to its remote MCP\n  server rather than to its REST API. They are read from the provider's own RFC\n  8414 authorization-server metadata and its RFC 9728 protected-resource metadata,\n  which agree. The REST API has no scope model at all — it authenticates with a\n  single organization-wide API token that carries every permission the\n  organization has.\nauthorization_server: https://app.reachdesk.com\nresource: https://app.reachdesk.com\nsurface: mcp\nscope_count: 2\nscopes:\n  - name: mcp:tools.user.read\n    description: >-\n      Read access to MCP tools acting on behalf of the authenticated Reachdesk\n      user. Description is inferred from the scope name — Reachdesk publishes the\n      scope string with no human-readable description and no scopes reference page.\n\
  \      Advertised in both scopes_supported lists.\n    access: read\n    documented_description: false\n  - name: mcp:tools.user.write\n    description: >-\n      Write access to MCP tools acting on behalf of the authenticated Reachdesk\n      user. Description inferred from the scope name; not documented by the\n      provider.\n    access: write\n    documented_description: false\ngrant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\npkce: S256\ndynamic_client_registration: true\nnotes:\n  - >-\n    The `user` segment in both scope names indicates tools are scoped to the\n    calling user, which mirrors the REST API's `sender` field (a send is always\n    made on behalf of a platform user).\n  - >-\n    No scopes/permissions reference page exists on reachdesk.readme.io or in the\n    Reachdesk knowledge base. method is `probed` rather than `searched` for exactly\n    that reason: these values come from a machine-readable endpoint, not from docs.\n  - >-\n \
  \   The REST API's OpenAPI declares a single apiKey security scheme with no scopes.\n    Nothing here applies to https://app.reachdesk.com/api/v2.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/scopes/reachdesk-scopes.yml
summary_line: 2 scopes
tags:
- Corporate Gifting
- Direct Mail
- Swag
- B2B
- Sales Enablement
- Customer Success
- Marketing Automation
- Gifting Platform
- Rewards
- MCP
- AI Agents
- OpenAPI
token_bound: false
token_urls: []
---
