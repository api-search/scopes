---
authorization_urls: []
description: ''
docs: https://mcp.globaldata.com/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Globaldata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GlobalData uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GlobalData
provider_slug: globaldata
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: globaldata-scopes
source_filename: globaldata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://mcp.globaldata.com/.well-known/oauth-authorization-server\ndocs: https://mcp.globaldata.com/\nsummary: >-\n  The four scopes GlobalData's OAuth 2.1 server advertises are OIDC identity scopes, nothing more.\n  They govern what claims a token carries and whether a refresh token is issued — they do NOT\n  express data permissions. What a caller can read is decided by subscription entitlement,\n  evaluated server-side per credential, and GlobalData publishes no scope names for it.\nderivation_note: >-\n  NOT derived from an OpenAPI oauth2 securityScheme — no OpenAPI exists for this provider. The list\n  below was read directly from the scopes_supported array of the fetched RFC 8414 document, and the\n  request-time scope string was read from GlobalData's own credentials-grant example.\nscopes:\n  - name: openid\n    description: OIDC — requests an ID token identifying the signed-in GlobalData user.\n    standard: true\n \
  \ - name: profile\n    description: OIDC — standard profile claims for the signed-in user.\n    standard: true\n  - name: email\n    description: OIDC — email claim for the signed-in user.\n    standard: true\n  - name: offline_access\n    description: OIDC — requests a refresh token so a long-running agent can renew without re-auth.\n    standard: true\nscope_count: 4\nrequested_in_docs: 'openid profile email offline_access'\ndata_permission_model:\n  expressed_as_scopes: false\n  mechanism: subscription entitlement\n  note: >-\n    A domain outside the caller's subscription returns not_entitled from discover_capabilities /\n    reveal_advanced. contacts, market_data, fdi_projects and ict_contracts each carry a separate\n    entitlement. None of these is addressable as an OAuth scope, so an agent cannot request or\n    inspect its own data permissions ahead of a call — it discovers them by calling list_domains.\nchecked: '2026-09-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globaldata/refs/heads/main/scopes/globaldata-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Market Intelligence
- Business Intelligence
- Data
- Analytics
- MCP
- Agents
- Company Data
- Deals
- News
- Patents
- Research
- Financial-Services
- Energy
- Mining
token_urls: []
---
