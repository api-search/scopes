---
api_specs:
- filename: semrush-hermes-partner-api-api-openapi.yml
  format: yaml
  label: Semrush Hermes Partner API API
  slug: semrush-hermes-partner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-hermes-partner-api-api-openapi.yml
- filename: semrush-jwt-issuer-api-openapi.yml
  format: yaml
  label: Semrush JWT Issuer API
  slug: semrush-jwt-issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-jwt-issuer-api-openapi.yml
- filename: semrush-partner-service-api-openapi.yml
  format: yaml
  label: Semrush Partner Service API
  slug: semrush-partner-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-partner-service-api-openapi.yml
authorization_urls: []
description: OAuth 2.0 scope inventory for Semrush. The authorization server advertises exactly one scope. Semrush publishes no scopes reference page and no permission catalogue for its OAuth APIs; the only scope in existence is the one the MCP resource declares, and the device-authorization documentation treats scope as optional ("if the API requires scopes").
docs: https://developer.semrush.com/api/v4/get-started/authorization/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Semrush Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Semrush uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Semrush
provider_slug: semrush
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: semrush-scopes
source_filename: semrush-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mcp.semrush.com/.well-known/oauth-authorization-server +\n  https://mcp.semrush.com/.well-known/oauth-protected-resource/v2/mcp +\n  https://developer.semrush.com/api/v4/get-started/authorization/\ndocs: https://developer.semrush.com/api/v4/get-started/authorization/\nprovider: Semrush\nproviderId: semrush\ndescription: >-\n  OAuth 2.0 scope inventory for Semrush. The authorization server advertises exactly one\n  scope. Semrush publishes no scopes reference page and no permission catalogue for its\n  OAuth APIs; the only scope in existence is the one the MCP resource declares, and the\n  device-authorization documentation treats scope as optional (\"if the API requires scopes\").\n\nauthorization_server:\n  issuer: https://api.semrush.com/apis/v4/auth/v1/oauth/access_token\n  metadata_url: https://mcp.semrush.com/.well-known/oauth-authorization-server\n  authorization_endpoint: https://api.semrush.com/apis/v4/auth/v0/oauth2/auth\n\
  \  token_endpoint: https://api.semrush.com/apis/v4-raw/auth/v1/oauth2/access_token\n  registration_endpoint: https://api.semrush.com/apis/v4-raw/auth/v1/oauth2/register\n  revocation_endpoint: https://api.semrush.com/apis/v4/auth/v1/oauth2/revoke\n  device_authorization_endpoint: https://oauth.semrush.com/dag/device/code\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  device_grant_note: >-\n    The device grant is documented in the developer portal (RFC 8628, \"recommended\") but is\n    not advertised in the RFC 8414 metadata document, which lists only authorization_code\n    and refresh_token. The metadata and the docs disagree.\n  pkce: [S256, plain]\n  token_endpoint_auth_methods: [none]\n\nscopes:\n- name: mcp.access\n  description: >-\n    Grants an MCP client access to the Semrush MCP server, and through it to the Trends API,\n    the whole SEO API, and the read-only methods of the Projects API v3. A single coarse\n\
  \    scope — there is no per-API, per-report or read/write split at the OAuth layer.\n  resources:\n  - https://mcp.semrush.com/v1/mcp\n  - https://mcp.semrush.com/v2/mcp\n  source: RFC 8414 + RFC 9728 metadata documents, fetched 2026-08-13\n\nscope_count: 1\n\nnon_oauth_permissions:\n  note: >-\n    Semrush's real authorization granularity lives on the API key, not on OAuth scopes. A v4\n    API key carries one of two permission settings, plus a TTL.\n  model:\n  - permission: Read-only\n    grants: GET requests\n    example: Get Location\n  - permission: Read and write\n    grants: GET, POST, PUT, PATCH, DELETE\n    example: Create Location\n  key_limits:\n    max_v4_keys_per_account: 100\n    revocable: true\n    ttl_configurable: true\n\ngaps:\n- No scopes or permissions reference page is published in the developer portal.\n- >-\n  The OAuth-authorized REST APIs (Map Rank Tracker, deprecated Projects, deprecated Listing\n  Management) document no scope values at all — only \"include\
  \ an optional scope parameter\n  if the API requires scopes\".\n- >-\n  mcp.access is all-or-nothing: an agent granted it can read every report the subscription\n  entitles, with no way for a user to narrow the grant.\n\nx-evidence:\n- url: https://mcp.semrush.com/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://mcp.semrush.com/.well-known/oauth-protected-resource/v2/mcp\n  http_status: 200\n- url: https://developer.semrush.com/api/v4/get-started/authorization/\n  http_status: 200\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/scopes/semrush-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Data
- Search Engines
- SEO
- Marketing
- Marketing Intelligence
- Content Marketing
- Advertising
- Competitive Intelligence
- Keyword Research
- Backlinks
- Rank Tracking
- AI Search Visibility
- Local SEO
- MCP
token_urls: []
---
