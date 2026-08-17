---
api_specs:
- filename: taboola-accounts-api-openapi.yml
  format: yaml
  label: Taboola Accounts API
  slug: taboola-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-accounts-api-openapi.yml
- filename: taboola-audience-targeting-api-openapi.yml
  format: yaml
  label: Taboola Audience Targeting API
  slug: taboola-audience-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-audience-targeting-api-openapi.yml
- filename: taboola-bulk-items-api-openapi.yml
  format: yaml
  label: Taboola Bulk Items API
  slug: taboola-bulk-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-bulk-items-api-openapi.yml
- filename: taboola-bulk-operations-api-openapi.yml
  format: yaml
  label: Taboola Bulk Operations API
  slug: taboola-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-bulk-operations-api-openapi.yml
- filename: taboola-campaign-items-api-openapi.yml
  format: yaml
  label: Taboola Campaign Items API
  slug: taboola-campaign-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-campaign-items-api-openapi.yml
- filename: taboola-campaigns-api-openapi.yml
  format: yaml
  label: Taboola Campaigns API
  slug: taboola-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-campaigns-api-openapi.yml
- filename: taboola-combined-audiences-api-openapi.yml
  format: yaml
  label: Taboola Combined Audiences API
  slug: taboola-combined-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-combined-audiences-api-openapi.yml
- filename: taboola-conversion-rules-api-openapi.yml
  format: yaml
  label: Taboola Conversion Rules API
  slug: taboola-conversion-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-conversion-rules-api-openapi.yml
- filename: taboola-custom-audiences-api-openapi.yml
  format: yaml
  label: Taboola Custom Audiences API
  slug: taboola-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-custom-audiences-api-openapi.yml
- filename: taboola-dictionary-api-openapi.yml
  format: yaml
  label: Taboola Dictionary API
  slug: taboola-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-dictionary-api-openapi.yml
- filename: taboola-first-party-audiences-api-openapi.yml
  format: yaml
  label: Taboola First Party Audiences API
  slug: taboola-first-party-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-first-party-audiences-api-openapi.yml
- filename: taboola-lookalike-audiences-api-openapi.yml
  format: yaml
  label: Taboola Lookalike Audiences API
  slug: taboola-lookalike-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-lookalike-audiences-api-openapi.yml
- filename: taboola-marketplace-audiences-api-openapi.yml
  format: yaml
  label: Taboola Marketplace Audiences API
  slug: taboola-marketplace-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-marketplace-audiences-api-openapi.yml
- filename: taboola-reach-estimator-api-openapi.yml
  format: yaml
  label: Taboola Reach Estimator API
  slug: taboola-reach-estimator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-reach-estimator-api-openapi.yml
- filename: taboola-reports-api-openapi.yml
  format: yaml
  label: Taboola Reports API
  slug: taboola-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-reports-api-openapi.yml
- filename: taboola-video-items-api-openapi.yml
  format: yaml
  label: Taboola Video Items API
  slug: taboola-video-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-video-items-api-openapi.yml
authorization_urls: []
description: 'Taboola runs OAuth on both of its API surfaces but publishes almost no scope vocabulary.

  derive-oauth-scopes.py found zero oauth2 securitySchemes in openapi/ (the captured specs

  model auth as an http bearer scheme, which is what the Backstage docs describe at the

  request level), so nothing could be derived. Everything below was probed or read from

  the provider''s own documentation.


  The finding: authorization on both surfaces is coarse. The Backstage API issues a token

  whose permissions are those of the account behind the client_id — there are no scopes at

  all in the token request. The Realize MCP server advertises exactly one scope, `all`.

  An agent cannot be granted read-only access to Realize; the same token that lists

  campaigns can create and update them.'
docs:
- https://developers.taboola.com/backstage-api/reference/authentication-basics
- https://developers.taboola.com/backstage-api/reference/client-credentials-flow
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Taboola Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Taboola uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Taboola
provider_slug: taboola
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: taboola-scopes
source_filename: taboola-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mcp.realize.com/.well-known/oauth-authorization-server,\n  https://mcp.realize.com/.well-known/oauth-protected-resource,\n  https://developers.taboola.com/backstage-api/reference/authentication-basics,\n  https://developers.taboola.com/backstage-api/reference/client-credentials-flow\nprovider: Taboola\nproviderId: taboola\ndescription: |-\n  Taboola runs OAuth on both of its API surfaces but publishes almost no scope vocabulary.\n  derive-oauth-scopes.py found zero oauth2 securitySchemes in openapi/ (the captured specs\n  model auth as an http bearer scheme, which is what the Backstage docs describe at the\n  request level), so nothing could be derived. Everything below was probed or read from\n  the provider's own documentation.\n\n  The finding: authorization on both surfaces is coarse. The Backstage API issues a token\n  whose permissions are those of the account behind the client_id — there are no scopes at\n\
  \  all in the token request. The Realize MCP server advertises exactly one scope, `all`.\n  An agent cannot be granted read-only access to Realize; the same token that lists\n  campaigns can create and update them.\n\ndocs:\n  - https://developers.taboola.com/backstage-api/reference/authentication-basics\n  - https://developers.taboola.com/backstage-api/reference/client-credentials-flow\n\nsurfaces:\n  - name: Backstage API\n    base: https://backstage.taboola.com/backstage/api/1.0\n    token_endpoint: https://backstage.taboola.com/backstage/oauth/token\n    grant: client_credentials\n    scope_parameter: not used\n    scopes_published: 0\n    note: >-\n      The documented token request body carries only client_id, client_secret and\n      grant_type. The embedded OpenAPI fragment on the client-credentials-flow docs page\n      declares the oauth2 scheme with an EMPTY scopes object (\"scopes\": {}) for both the\n      clientCredentials and password flows — the provider's own machine-readable\
  \ statement\n      that there is no scope vocabulary. Permissions are attached to the account the\n      credentials identify (\"The Access Token identifies who you are - and your set of\n      permissions\").\n\n  - name: Realize MCP\n    base: https://mcp.realize.com/mcp\n    issuer: https://mcp.realize.com\n    authorization_endpoint: https://authentication.taboola.com/authentication/oauth2.1/authorize\n    token_endpoint: https://authentication.taboola.com/authentication/oauth2.1/token\n    grant: [authorization_code, refresh_token, client_credentials]\n    pkce: S256\n    scopes_published: 1\n    scopes:\n      - name: all\n        description: >-\n          The only scope the Realize authorization server advertises. Declared in both\n          RFC 8414 authorization-server metadata (scopes_supported) and RFC 9728\n          protected-resource metadata (scopes_supported). No description is published by\n          the provider; the name is self-describing and there is no narrower alternative.\n\
  \        source: https://mcp.realize.com/.well-known/oauth-authorization-server\n        http_status: 200\n        read_only_alternative: none\n    note: >-\n      Coarse-grained by construction. The MCP server exposes 25 tools including six write\n      tools (create_campaign, update_campaign, create/update native and display items) and\n      they are all reachable under the same single scope. Least-privilege for an agent has\n      to be enforced client-side — which is exactly what Taboola's own realize-claude-plugin\n      does, splitting reads and writes across separate skills and gating every write behind\n      a preview-and-confirm step (see ../skills/taboola-manage-campaigns.md).\n\nx-evidence:\n  - fetched: '2026-08-13'\n    url: https://mcp.realize.com/.well-known/oauth-authorization-server\n    http_status: 200\n    file: ../well-known/taboola-mcp-oauth-authorization-server.json\n  - fetched: '2026-08-13'\n    url: https://mcp.realize.com/.well-known/oauth-protected-resource\n\
  \    http_status: 200\n    file: ../well-known/taboola-mcp-oauth-protected-resource.json\n\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/scopes/taboola-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Advertising
- Native Advertising
- Discovery
- Performance Marketing
- AdTech
- Realize
- Backstage
- Recommendation
- Publisher
- Programmatic
token_urls: []
---
