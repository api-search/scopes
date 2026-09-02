---
api_specs:
- filename: closedloop-public-api-openapi.yaml
  format: yaml
  label: ClosedLoop AI REST API
  slug: closedloop-ai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-public-api-openapi.yaml
authorization_urls: []
description: ''
docs: https://closedloop.sh/docs/account/mcp-service-clients
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Closedloop Scopes
name_suffix: OAuth Scopes
note: 'derive-oauth-scopes.py returned nothing for this provider, correctly: the published OpenAPI declares only an apiKey securityScheme and no oauth2 flows, so there is nothing in the REST contract to derive from. The scopes below are NOT derived -- they were read from the live OAuth metadata the MCP servers actually serve. The provider publishes the scope NAMES in that metadata but publishes no per-scope description or permission matrix anywhere in its documentation, so the descriptions below say what the metadata establishes and no more.'
overview: 'ClosedLoop AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClosedLoop AI
provider_slug: closedloop
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: closedloop-scopes
source_filename: closedloop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://mcp.closedloop.sh/.well-known/oauth-authorization-server and\n  https://mcp.closedloop.sh/.well-known/oauth-protected-resource\ndocs: https://closedloop.sh/docs/account/mcp-service-clients\nnote: >-\n  derive-oauth-scopes.py returned nothing for this provider, correctly: the published OpenAPI\n  declares only an apiKey securityScheme and no oauth2 flows, so there is nothing in the REST\n  contract to derive from. The scopes below are NOT derived -- they were read from the live OAuth\n  metadata the MCP servers actually serve. The provider publishes the scope NAMES in that metadata\n  but publishes no per-scope description or permission matrix anywhere in its documentation, so the\n  descriptions below say what the metadata establishes and no more.\napplies_to: MCP surface only\nrest_api_scopes:\n  model: none\n  detail: >-\n    The /v1 REST API has no scope model at all. A key is team-scoped and region-scoped and grants\n\
  \    read access to everything that team can see; there is no way to issue a narrower key. Since\n    every operation is a GET, the blast radius of a leaked key is disclosure, not modification.\nauthorization_servers:\n- issuer: https://mcp.closedloop.sh\n  region: us\n  documented: true\n  scopes_supported: [mcp:tools, mcp:read]\n- issuer: https://eu.mcp.closedloop.sh\n  region: eu\n  documented: true\n  scopes_supported: [mcp:tools, mcp:read]\n- issuer: https://api.closedloop.sh/mcp\n  region: us\n  documented: false\n  scopes_supported: [mcp:tools, mcp:read]\n- issuer: https://eu.api.closedloop.sh/mcp\n  region: eu\n  documented: false\n  scopes_supported: [mcp:tools, mcp:read]\nscopes:\n- name: mcp:tools\n  description: >-\n    Invoke MCP tools. Advertised in both scopes_supported (authorization-server metadata) and the\n    protected-resource metadata on every ClosedLoop AI MCP host.\n  published_description: null\n  published_description_note: The provider publishes no description\
  \ for this scope. Recorded as\n    null rather than guessed.\n  covers: >-\n    Presumed to gate the 12 documented tools (get_overview, get_facets, get_trends,\n    search_customers, get_customer, search_insights, get_insight, search_signals, get_signal,\n    get_competitors, search_opportunities, get_opportunity). NOT CONFIRMED -- tools/list is\n    OAuth-gated so the per-tool scope requirement could not be observed.\n- name: mcp:read\n  description: >-\n    Read access over the MCP surface. Advertised alongside mcp:tools on every host.\n  published_description: null\n  published_description_note: The provider publishes no description for this scope.\n  covers: >-\n    Relationship to mcp:tools is not documented. Since every MCP tool is itself a read, the two\n    scopes may overlap substantially. NOT CONFIRMED.\nscope_count: 2\nbearer_methods_supported: [header]\ngrant_types_supported: [authorization_code, refresh_token, client_credentials]\ngaps:\n- id: no-scope-reference-page\n  detail:\
  \ >-\n    There is no scopes or permissions reference page anywhere under https://closedloop.sh/docs. The\n    MCP service-clients guide explains how to obtain a credential but never states what each scope\n    grants or which scope a given tool requires. A security reviewer cannot answer \"what can this\n    token do\" from published material -- only from the two scope names in the metadata.\n- id: rest-has-no-scopes\n  detail: >-\n    A ClosedLoop AI REST key cannot be narrowed. There is no read-only-subset key, no per-resource\n    key, and no way to issue a key that can see insights but not customer CRM context and deal\n    values. For a product whose data includes named customers, ARR and deal values, that is the\n    most consequential authorization gap in the surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/scopes/closedloop-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Product Intelligence
- Customer Feedback
- Voice of Customer
- Product Management
- Agentic AI
- MCP
- SaaS analytics
- A2A
- SCIM
- Product Discovery
token_urls: []
---
