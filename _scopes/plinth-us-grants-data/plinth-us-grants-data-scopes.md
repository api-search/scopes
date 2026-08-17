---
api_specs:
- filename: plinth-us-grants-data-analyze-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Analyze API
  slug: plinth-us-grants-data-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-analyze-api-openapi.yml
- filename: plinth-us-grants-data-grants-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Grants API
  slug: plinth-us-grants-data-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-grants-api-openapi.yml
- filename: plinth-us-grants-data-organizations-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Organizations API
  slug: plinth-us-grants-data-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-organizations-api-openapi.yml
- filename: plinth-us-grants-data-resolve-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Resolve API
  slug: plinth-us-grants-data-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-resolve-api-openapi.yml
- filename: plinth-us-grants-data-sql-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data SQL API
  slug: plinth-us-grants-data-sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-sql-api-openapi.yml
authorization_urls: []
description: ''
docs: https://data.useplinth.com/connect
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Plinth Us Grants Data Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Plinth US Grants Data uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Plinth US Grants Data
provider_slug: plinth-us-grants-data
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: plinth-us-grants-data-scopes
source_filename: plinth-us-grants-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://data.useplinth.com/.well-known/oauth-authorization-server\ncorroboration:\n  - https://data.useplinth.com/.well-known/oauth-protected-resource\n  - https://data.useplinth.com/.well-known/api-onboarding\ndocs: https://data.useplinth.com/connect\nchecked: '2026-08-14'\nderivation_note: >-\n  derive-oauth-scopes.py found zero oauth2 securitySchemes and wrote nothing — correctly, because\n  the REST OpenAPI declares only the X-API-Key apiKey scheme. The OAuth surface belongs to the MCP\n  connector, not to REST, and is discoverable only from the RFC 8414 metadata document. This file\n  was therefore written from the live metadata rather than from the spec.\n\nsummary: >-\n  ONE scope, `plinth:read`, covering the entire MCP connector. There is no scope decomposition —\n  no per-tool, per-dataset or read/write split — because the whole product is read-only. What\n  looks like authorization granularity at Plinth is actually\
  \ PLAN granularity: the boundary between\n  what an agent may reach is drawn by the subscription tier, enforced at 402/403, not by scopes.\n\nmodel: single-scope\nauthorization_server: https://data.useplinth.com\nprotected_resource: https://data.useplinth.com/api/connector/mcp\nscope_count: 1\n\nscopes:\n  - name: plinth:read\n    description: >-\n      Read access to the Plinth grants warehouse through the MCP connector. Advertised in both the\n      RFC 8414 authorization-server metadata (scopes_supported) and the RFC 9728 protected-resource\n      metadata (scopes_supported) — the two agree.\n    grants:\n      - Search organizations (name -> EIN resolution)\n      - Foundation dossiers (giving, causes, grantee network, look-alikes)\n      - Natural-language questions grounded in a foundation's IRS filings\n    write_access: false\n    source: https://data.useplinth.com/.well-known/oauth-authorization-server\n    verbatim: '\"scopes_supported\":[\"plinth:read\"]'\n\nflow:\n  grant_types:\
  \ [authorization_code, refresh_token]\n  pkce: S256\n  pkce_required: true\n  client_registration: dynamic (RFC 7591) at https://data.useplinth.com/oauth/register\n  token_endpoint_auth_methods: [none]\n  response_types: [code]\n  bearer_methods: [header]\n  consent: >-\n    Browser sign-in required once. The provider's own onboarding descriptor lists \"No programmatic\n    signup\" as a gap: dynamic registration and PKCE are fully automatable, but the human consent\n    step and the plan check are not.\n\nauthorization_is_plan_shaped:\n  model: product-tiers\n  vocabulary_url: https://data.useplinth.com/pricing\n  provider_wording: >-\n    \"Plan-gated rather than scoped. The free tier reads /grants/* and the organization endpoints;\n    POST /api/sql, the people/board and asset tables and the MCP connector require a paid plan. A\n    request outside the plan answers 402 with a message naming the reason.\"\n    — /.well-known/api-onboarding, scopes.notes\n  effective_boundaries:\n   \
  \ - boundary: unauthenticated\n      reaches: GET /api/search only (security [] in the spec; unmetered)\n    - boundary: free key\n      reaches: /grants/* and the three organization endpoints, 50 calls/month\n    - boundary: paid key\n      reaches: '+ POST /api/sql, + the people/board and asset warehouse tables'\n    - boundary: For consultants ($250/mo)\n      reaches: '+ the MCP connector (plinth:read), 10,000 calls/month'\n  enforcement: 402 (plan/allowance) and 403 (gated warehouse table named in SQL)\n  see:\n    - errors/plinth-us-grants-data-problem-types.yml\n    - plans/plinth-us-grants-data-plans-pricing.yml\n\nrest_api_scopes:\n  applicable: false\n  note: >-\n    The REST API uses a static API key with no scope surface at all. One key per account, rotatable\n    at /account, prefixed `plinth_sk_`, shown once. See\n    authentication/plinth-us-grants-data-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/scopes/plinth-us-grants-data-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Philanthropy
- Grants
- Nonprofits
- Foundations
- IRS 990
- Open Data
- Government Spending
- Research
- Agents
- REST
- JSON
- MCP
- SQL
token_urls: []
---
