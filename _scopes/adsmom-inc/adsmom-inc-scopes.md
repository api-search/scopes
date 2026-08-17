---
api_specs:
- filename: adsmom-inc-openapi.json
  format: json
  label: Adsmom REST API
  slug: adsmom-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsmom-inc/refs/heads/main/openapi/adsmom-inc-openapi.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Adsmom Inc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adsmom Inc. uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adsmom Inc.
provider_slug: adsmom-inc
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: adsmom-inc-scopes
source_filename: adsmom-inc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://app.adsmom.com/.well-known/oauth-authorization-server (RFC 8414, HTTP 200,\n  scopes_supported) + https://app.adsmom.com/.well-known/oauth-protected-resource\n  and .../oauth-protected-resource/mcp (RFC 9728, HTTP 200)\ndocs: null\ndocs_note: >-\n  Adsmom publishes no scope-reference page. https://adsmom.com/product/api describes\n  the auth model in prose only and sends the reader to the Integrations section of a\n  logged-in account. Every scope string below is read verbatim from the provider's own\n  anonymous OAuth discovery documents — not from documentation, and not inferred.\nprovider: Adsmom\nissuer: https://app.adsmom.com\nauthorization_endpoint: https://app.adsmom.com/oauth/authorize\ntoken_endpoint: https://app.adsmom.com/oauth/token\nscope_count: 4\n\nscopes:\n- name: mcp:invoke\n  description: >-\n    Invoke tools on the Adsmom MCP server. The only scope advertised by either\n    protected-resource\
  \ document, and the scope an MCP client (Claude, Codex,\n    Cursor, Gemini) requests when connecting.\n  surfaces:\n  - mcp\n  advertised_by:\n  - /.well-known/oauth-authorization-server\n  - /.well-known/oauth-protected-resource\n  - /.well-known/oauth-protected-resource/mcp\n- name: api:read\n  description: >-\n    Read access to the REST API. Maps to the 66 GET operations in the OpenAPI —\n    Explore (ad listing, hydration, detail, reach/impression timeseries,\n    snapshots), Insights reads (tracked advertisers/accounts, AI summaries,\n    weekly reports) and all of Analytics.\n  surfaces:\n  - rest\n  advertised_by:\n  - /.well-known/oauth-authorization-server\n- name: api:write\n  description: >-\n    Write access to the REST API. Maps to the 12 mutating operations — the six\n    POST track* operations (trackMetaAdvertiser, trackTiktokAdvertiser,\n    trackGoogleAdvertiser, trackLinkedinAdvertiser, trackTiktokSocialAccount,\n    trackInstagramSocialAccount) and the six DELETE untrack*\
  \ operations.\n  surfaces:\n  - rest\n  advertised_by:\n  - /.well-known/oauth-authorization-server\n- name: billing:read\n  description: >-\n    Read access to billing/entitlement state. No REST operation in the published\n    OpenAPI is billing-specific; the closest is getUsage (GET /api/v1/usage),\n    which returns plan, credits and rate limit.\n  surfaces:\n  - rest\n  advertised_by:\n  - /.well-known/oauth-authorization-server\n\nmapping_note: >-\n  The OpenAPI declares its security scheme as an HTTP bearer scheme rather than an\n  oauth2 scheme with a flows/scopes map, so no operation in the spec names a scope.\n  The surface/operation mapping above is an honest derivation from the scope names\n  and the operation verbs; Adsmom does not publish a per-operation scope table.\n\ncross_links:\n  authentication: authentication/adsmom-inc-authentication.yml\n  well_known: well-known/adsmom-inc-well-known.yml\n  openapi: openapi/adsmom-inc-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adsmom-inc/refs/heads/main/scopes/adsmom-inc-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- Ad Intelligence
- Competitive Intelligence
- Marketing
- AI
- MCP
- SaaS
- OpenAPI
- REST
- Analytics
- Social Media
- Agent Native
token_urls: []
---
