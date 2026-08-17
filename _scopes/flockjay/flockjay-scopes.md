---
authorization_urls: []
description: Flockjay's authorization server advertises exactly two scopes. There is no scopes or permissions reference page anywhere on flockjay.com — these are read from the server's own RFC 8414 metadata, which is the only place they are published.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Flockjay Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flockjay uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flockjay
provider_slug: flockjay
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: flockjay-scopes
source_filename: flockjay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://api.flockjay.com/.well-known/oauth-authorization-server and\n  https://api.flockjay.com/.well-known/oauth-protected-resource (fetched 2026-08-14)\nname: Flockjay OAuth scopes\ndescription: >-\n  Flockjay's authorization server advertises exactly two scopes. There is no scopes\n  or permissions reference page anywhere on flockjay.com — these are read from the\n  server's own RFC 8414 metadata, which is the only place they are published.\ndocs: null\ndocs_note: >-\n  No public scopes/permissions documentation exists. The authoritative list is the\n  machine-readable metadata document itself.\n\nauthorization_server: https://api.flockjay.com\nprotected_resource: https://api.flockjay.com/mcp\n\nscopes:\n- name: read\n  description: >-\n    Read access to the caller's Flockjay enablement data. Required by the MCP\n    server — the WWW-Authenticate challenge on POST /mcp names scope=\"read\"\n    explicitly.\n  required_by:\n\
  \  - https://api.flockjay.com/mcp\n  source: oauth-authorization-server metadata + WWW-Authenticate challenge\n- name: offline_access\n  description: >-\n    Issues a refresh token so an agent can keep calling after the access token\n    expires. Backed by grant_types_supported including refresh_token.\n  source: oauth-authorization-server metadata\n\nscope_count: 2\n\nfindings:\n- >-\n  The scope model is read-only. No write, admin, or resource-specific scope is\n  advertised, so an OAuth client — including the MCP server — cannot mutate\n  enablement data through this path. That is a deliberate and defensible posture\n  for an agent surface, and worth saying plainly.\n- >-\n  Scopes are coarse. There is no per-resource decomposition (no courses:read,\n  no scorecards:read), so a customer granting an AI assistant access grants it\n  everything readable at once. There is no way to consent to less.\n- >-\n  Because token_endpoint_auth_methods_supported is [\"none\"] and registration is\n\
  \  dynamic, any client can register and request these scopes; the control point is\n  the user's authorization decision at https://flockjay.com/oauth/authorize, not\n  client vetting.\n\nrelated:\n  authentication: authentication/flockjay-authentication.yml\n  mcp: mcp/flockjay-mcp.yml\n  well_known: well-known/flockjay-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flockjay/refs/heads/main/scopes/flockjay-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Sales Enablement
- Sales Training
- Learning Management
- Revenue Operations
- AI Coaching
- Content Management
- SaaS
- MCP
- Agent Native
- OAuth
token_urls: []
---
