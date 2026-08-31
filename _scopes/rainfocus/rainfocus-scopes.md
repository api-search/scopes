---
authorization_urls: []
description: The only OAuth scope RainFocus advertises anywhere machine-readable is "openid", read from its own OIDC discovery document. RainFocus describes "short-lived, scoped access tokens" and "per-event scoping" for MCP Profiles, so a scope or permission vocabulary demonstrably exists inside the product - it is simply not published. No scope names are invented here.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Rainfocus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RainFocus uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RainFocus
provider_slug: rainfocus
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rainfocus-scopes
source_filename: rainfocus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://api.rainfocus.com/.well-known/openid-configuration\ndocs: null\ndocs_note: >-\n  RainFocus publishes no scopes or permissions reference page. Searching the public site and the\n  API and MCP Tools terms turned up no scope names.\ndescription: >-\n  The only OAuth scope RainFocus advertises anywhere machine-readable is \"openid\", read from its\n  own OIDC discovery document. RainFocus describes \"short-lived, scoped access tokens\" and\n  \"per-event scoping\" for MCP Profiles, so a scope or permission vocabulary demonstrably exists\n  inside the product - it is simply not published. No scope names are invented here.\nauthorization_server: https://events.rainfocus.com/oidc\nscopes:\n- name: openid\n  description: >-\n    Standard OpenID Connect scope requesting an ID token. Advertised in scopes_supported.\n  source: '.well-known/openid-configuration scopes_supported'\nscope_count: 1\nundocumented_scoping_mechanisms:\n\
  - mechanism: API Profile\n  description: >-\n    Each RainFocus API Profile declares which endpoints are enabled (for example Attendee Store),\n    which is the effective authorization boundary for the REST API. Profile names and the endpoint\n    catalog are customer-specific and not published.\n  source: https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/marketing-automation/rainfocus\n- mechanism: MCP Profile per-event scoping\n  description: >-\n    Planners activate and control MCP tool access event by event, layered on per-user\n    authentication and role-based access control.\n  source: https://www.rainfocus.com/company/news-press/rainfocus-launches-ai-agent-connectivity-for-event-data-with-mcp-profiles/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainfocus/refs/heads/main/scopes/rainfocus-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Event
- Event Management
- Event Marketing
- Registration
- Conferences
- Webinars
- Marketing Technology
- Attendee Data
- MCP
- Agents
- Enterprise Software
- Software-as-a-Service
token_urls: []
---
