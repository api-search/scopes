---
api_specs:
- filename: channel99-pulsar-openapi.json
  format: json
  label: Channel99 Pulsar Reporting API
  slug: channel99-pulsar-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-pulsar-openapi.json
authorization_urls: []
description: ''
docs: https://support.channel99.com/hc/en-us/articles/47105598392475-MCP-Server-General-FAQ
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Channel99 Scopes
name_suffix: OAuth Scopes
note: 'Channel99 publishes no scopes reference page. These scopes are read verbatim from the two RFC 8414 authorization-server metadata documents Channel99 serves - the resource-scoped list advertised by the MCP server, and the wider list advertised by the Stytch authorization server that backs the web application. The Pulsar Reporting API does NOT use OAuth scopes: it uses an M2M client_credentials exchange whose authorization is carried entirely by the tenant binding of the client_id, so there is nothing scope-shaped to record for it.'
overview: 'Channel99 uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Channel99
provider_slug: channel99
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: channel99-scopes
source_filename: channel99-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://mcp.channel99.com/.well-known/oauth-authorization-server\ndocs: https://support.channel99.com/hc/en-us/articles/47105598392475-MCP-Server-General-FAQ\nnote: >-\n  Channel99 publishes no scopes reference page. These scopes are read verbatim from the two\n  RFC 8414 authorization-server metadata documents Channel99 serves - the resource-scoped list\n  advertised by the MCP server, and the wider list advertised by the Stytch authorization server\n  that backs the web application. The Pulsar Reporting API does NOT use OAuth scopes: it uses an\n  M2M client_credentials exchange whose authorization is carried entirely by the tenant binding\n  of the client_id, so there is nothing scope-shaped to record for it.\n\nauthorization_servers:\n- issuer: https://api.stytch.app.channel99.com\n  metadata: https://mcp.channel99.com/.well-known/oauth-authorization-server\n  protected_resource: https://mcp.channel99.com\n  applies_to: Channel99\
  \ MCP Server\n  scopes:\n  - name: openid\n    description: Authenticate the user and issue an OpenID Connect ID token.\n  - name: email\n    description: Read the authenticated user's email address.\n  - name: profile\n    description: Read the authenticated user's basic profile.\n\n- issuer: https://api.stytch.app.channel99.com\n  metadata: https://api.stytch.app.channel99.com/.well-known/openid-configuration\n  applies_to: Channel99 web application (app.channel99.com)\n  scopes:\n  - name: openid\n    description: Authenticate the user and issue an OpenID Connect ID token.\n  - name: profile\n    description: Read the authenticated user's basic profile.\n  - name: email\n    description: Read the authenticated user's email address.\n  - name: phone\n    description: Read the authenticated user's phone number.\n  - name: offline_access\n    description: Issue a refresh token so the client can act after the session token expires.\n  - name: full_access\n    description: >-\n      Stytch's\
  \ catch-all scope granting the full set of session permissions for the\n      organization member. No Channel99 documentation describes narrower resource scopes.\n\ngranularity:\n  resource_scopes_published: false\n  assessment: >-\n    Neither authorization server publishes resource-level scopes (nothing of the form\n    visits:read or audiences:write). Authorization on the MCP surface is coarse - the FAQ states\n    the connection is read-only across the tenant's data, enforced server-side rather than\n    expressed as scopes a client can request or a user can review at consent time.\n\nscope_count: 6\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/scopes/channel99-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Analytics
- Attribution
- B2B
- Advertising
- Marketing Technology
- Artificial Intelligence
- Account Based Marketing
- Reporting
- MCP
- Agent Ready
- Intent Data
- Account Identification
- Data Export
token_urls: []
---
