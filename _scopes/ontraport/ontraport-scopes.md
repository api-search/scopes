---
api_specs:
- filename: ontraport-metadata-api-openapi.yml
  format: yaml
  label: Ontraport Metadata API
  slug: ontraport-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/openapi/ontraport-metadata-api-openapi.yml
- filename: ontraport-objects-api-openapi.yml
  format: yaml
  label: Ontraport Objects API
  slug: ontraport-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/openapi/ontraport-objects-api-openapi.yml
authorization_urls: []
description: 'Ontraport publishes exactly one OAuth scope, and it exists only on the MCP surface. The REST API has no OAuth at all — it authenticates with a pair of static account-level headers and has no scope concept, which means an Ontraport API key is unscoped and carries whatever the owning user can do. The single mcp:tools scope is coarse: it grants the whole 47-tool surface, including the commerce tools that charge and refund cards. Ontraport''s compensating control is client-side, not server-side — a per-connection configure panel where the account holder enables or disables individual tools after connecting.'
docs: https://ontraport.com/support/My-account/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ontraport Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ontraport uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ontraport
provider_slug: ontraport
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ontraport-scopes
source_filename: ontraport-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mcp.ontraport.com/.well-known/oauth-protected-resource and\n  https://app.ontraport.com/.well-known/oauth-authorization-server, both fetched 2026-08-13\n  with HTTP 200; corroborated by https://ontraport.com/support/My-account/mcp-server\ndocs: https://ontraport.com/support/My-account/mcp-server\ndescription: >-\n  Ontraport publishes exactly one OAuth scope, and it exists only on the MCP surface. The\n  REST API has no OAuth at all — it authenticates with a pair of static account-level\n  headers and has no scope concept, which means an Ontraport API key is unscoped and carries\n  whatever the owning user can do. The single mcp:tools scope is coarse: it grants the whole\n  47-tool surface, including the commerce tools that charge and refund cards. Ontraport's\n  compensating control is client-side, not server-side — a per-connection configure panel\n  where the account holder enables or disables individual tools\
  \ after connecting.\nscheme: oauth2\ngrant_types:\n- authorization_code\n- refresh_token\npkce: S256\ndynamic_client_registration: true\nresource: https://mcp.ontraport.com\nauthorization_server: https://app.ontraport.com\nendpoints:\n  authorization: https://app.ontraport.com/oauth/authorize\n  token: https://app.ontraport.com/oauth/token\n  registration: https://app.ontraport.com/oauth/register\n  revocation: https://app.ontraport.com/oauth/revoke\nscope_count: 1\nscopes:\n- name: mcp:tools\n  description: >-\n    Access to the tools exposed by the Ontraport MCP server. The only scope advertised in\n    both the protected-resource metadata and the authorization-server metadata, and the\n    scope named in the WWW-Authenticate challenge returned by an unauthenticated tools/list.\n  grants: >-\n    The full published MCP tool surface — CRUD, Query, Manage and Commerce. Not\n    read/write-separated and not resource-separated.\n  source: >-\n    scopes_supported in https://mcp.ontraport.com/.well-known/oauth-protected-resource\n\
  rest_api:\n  oauth: false\n  scopes: false\n  note: >-\n    The REST API at https://api.ontraport.com/1 uses Api-Key + Api-Appid headers with no\n    scope parameter. Authorization is bounded instead by Ontraport package-level and\n    user-level permissions, which have applied to API requests since 2019-02-01, and by the\n    per-object Access column (many object types are GET-only) published in the Accessible\n    Objects table.\ngaps:\n- >-\n  One scope for a surface that includes process_transaction, refund_transaction and\n  cancel_subscription. There is no way to grant an agent read-only access at the\n  authorization layer.\n- >-\n  No scope separates the schema-mutating surface from the data surface, though in practice\n  Ontraport has kept field editing off the MCP server entirely.\n- >-\n  REST API keys have no scopes and no expiry, so key-based MCP connections bypass the scope\n  model altogether.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/scopes/ontraport-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CRM
- Marketing Automation
- Email Marketing
- Ecommerce
- Landing Pages
- Membership Sites
- MCP
- AI Agents
- Payments
- Sales Automation
token_urls: []
---
