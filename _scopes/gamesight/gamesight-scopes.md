---
api_specs:
- filename: gamesight-measurement-api-openapi.yml
  format: yaml
  label: Gamesight Measurement API
  slug: gamesight-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-measurement-api-openapi.yml
- filename: gamesight-reporting-api-openapi.yml
  format: yaml
  label: Gamesight Reporting API
  slug: gamesight-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-reporting-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.gamesight.io/reference/authorization
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Gamesight Scopes
name_suffix: OAuth Scopes
note: Gamesight has TWO distinct authorization models and this artifact records both, because neither alone describes the provider. (1) OAuth 2.0 — discovered by probe, not by documentation. The RFC 8414 Authorization Server Metadata served on both api.marketing.gamesight.io and console.gamesight.io declares exactly one supported scope, "mcp", which gates the hosted MCP server at https://console.gamesight.io/mcp. This OAuth surface is undocumented in the public developer docs. (2) API key scopes — the documented model for both REST APIs. These are NOT OAuth scopes; they are permission roles selected at key-creation time in the console, and they are carried by the opaque key in the Authorization header. They are recorded here because they are the real authorization vocabulary a consumer must reason about.
overview: 'Gamesight uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gamesight
provider_slug: gamesight
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: gamesight-scopes
source_filename: gamesight-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://api.marketing.gamesight.io/.well-known/oauth-authorization-server,\n  https://console.gamesight.io/.well-known/oauth-protected-resource/mcp\ndocs: https://docs.gamesight.io/reference/authorization\nnote: >-\n  Gamesight has TWO distinct authorization models and this artifact records\n  both, because neither alone describes the provider.\n  (1) OAuth 2.0 — discovered by probe, not by documentation. The RFC 8414\n  Authorization Server Metadata served on both api.marketing.gamesight.io and\n  console.gamesight.io declares exactly one supported scope, \"mcp\", which gates\n  the hosted MCP server at https://console.gamesight.io/mcp. This OAuth surface\n  is undocumented in the public developer docs.\n  (2) API key scopes — the documented model for both REST APIs. These are NOT\n  OAuth scopes; they are permission roles selected at key-creation time in the\n  console, and they are carried by the opaque key in the Authorization\
  \ header.\n  They are recorded here because they are the real authorization vocabulary a\n  consumer must reason about.\noauth:\n  discovered_by: probe\n  documented: false\n  schemes:\n    - name: GamesightOAuth2\n      type: oauth2\n      issuer: https://console.gamesight.io\n      flows:\n        - flow: authorizationCode\n          authorizationUrl: https://console.gamesight.io/authorize\n          tokenUrl: https://console.gamesight.io/api/app/oauth/token\n          refreshUrl: https://console.gamesight.io/api/app/oauth/token\n          pkce: S256\n      registration_endpoint: https://console.gamesight.io/api/app/oauth/register\n      revocation_endpoint: https://console.gamesight.io/api/app/oauth/revoke\n  scopes:\n    - scope: mcp\n      description: >-\n        Grants a bearer token access to the Gamesight MCP Server\n        (https://console.gamesight.io/mcp). The only scope the authorization\n        server advertises. The set of tools this scope unlocks is not published.\n \
  \     flows: [authorizationCode]\n      resource: https://console.gamesight.io/mcp\n      sources:\n        - well-known/gamesight-oauth-authorization-server.json\n        - well-known/gamesight-oauth-protected-resource-mcp.json\napi_key_scopes:\n  documented: true\n  mechanism: Opaque API key in the Authorization request header; scope is fixed at key creation.\n  docs: https://docs.gamesight.io/docs/api-key-management\n  scopes:\n    - scope: Reporting\n      description: >-\n        Fully permissioned reporting key — marketing analytics reporting, game\n        analytics, user-level reporting, and unattributed goals. Intended for\n        internal use by the game developer/publisher.\n    - scope: Aggregate Reporting\n      description: >-\n        Restricted reporting key scoped to a specific set of teams. No access to\n        game analytics, user-level reporting, or unattributed goals. Intended for\n        external parties such as agencies who need campaign performance only.\n  \
  \  - scope: GDPR\n      description: >-\n        Permits Data Access, Right-to-Forget, and Opt-Out requests for user data.\n    - scope: Audit\n      description: Permits calls to the Audit Log API (/audit_logs).\n    - scope: Event Measurement\n      description: >-\n        Separate in-game/website ingest key, provisioned under Management >\n        In-Game Integration rather than the API Keys settings page. Used only by\n        the Measurement API and the Web SDK.\nx-evidence:\n  - url: https://api.marketing.gamesight.io/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://console.gamesight.io/.well-known/oauth-protected-resource/mcp\n    status: 200\n  - url: https://docs.gamesight.io/reference/authorization\n    status: 200\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/scopes/gamesight-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Gaming
- Marketing
- Analytics
- Attribution
- Measurement
- Advertising
- Creators
- Game Development
token_urls: []
---
