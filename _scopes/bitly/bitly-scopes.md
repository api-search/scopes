---
api_specs:
- filename: bitly-bsds-api-openapi.yml
  format: yaml
  label: Bitly BSDs API
  slug: bitly-bsds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-bsds-api-openapi.yml
- filename: bitly-bitlinks-api-openapi.yml
  format: yaml
  label: Bitly Bitlinks API
  slug: bitly-bitlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-bitlinks-api-openapi.yml
- filename: bitly-campaigns-api-openapi.yml
  format: yaml
  label: Bitly Campaigns API
  slug: bitly-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-campaigns-api-openapi.yml
- filename: bitly-custom-bitlinks-api-openapi.yml
  format: yaml
  label: Bitly Custom Bitlinks API
  slug: bitly-custom-bitlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-custom-bitlinks-api-openapi.yml
- filename: bitly-groups-api-openapi.yml
  format: yaml
  label: Bitly Groups API
  slug: bitly-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-groups-api-openapi.yml
- filename: bitly-oauth-apps-api-openapi.yml
  format: yaml
  label: Bitly OAuth Apps API
  slug: bitly-oauth-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-oauth-apps-api-openapi.yml
- filename: bitly-organizations-api-openapi.yml
  format: yaml
  label: Bitly Organizations API
  slug: bitly-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-organizations-api-openapi.yml
- filename: bitly-qr-codes-api-openapi.yml
  format: yaml
  label: Bitly QR Codes API
  slug: bitly-qr-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-qr-codes-api-openapi.yml
- filename: bitly-user-api-openapi.yml
  format: yaml
  label: Bitly User API
  slug: bitly-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-user-api-openapi.yml
- filename: bitly-webhooks-api-openapi.yml
  format: yaml
  label: Bitly Webhooks API
  slug: bitly-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://dev.bitly.com/docs/getting-started/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bitly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bitly uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bitly
provider_slug: bitly
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: bitly-scopes
source_filename: bitly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://dev.bitly.com/docs/getting-started/authentication,\n  well-known/bitly-oauth-authorization-server.json (live fetch 2026-08-13),\n  openapi/_original/bitly-v4-openapi.json\ndocs: https://dev.bitly.com/docs/getting-started/authentication\nscope_count: 0\nscopes: []\nfinding: >-\n  Bitly runs a real OAuth 2.0 authorization server but publishes NO scopes. This file records\n  that as a measured absence, because a reader would otherwise assume the check was never run.\nevidence:\n- source: well-known/bitly-oauth-authorization-server.json\n  url: https://api-ssl.bitly.com/.well-known/oauth-authorization-server\n  http_status: 200\n  detail: >-\n    RFC 8414 metadata is served and complete on every other axis — issuer, authorization_endpoint,\n    token_endpoint, registration_endpoint, jwks_uri, grant_types_supported,\n    code_challenge_methods_supported — but it omits `scopes_supported` entirely.\n- source: https://dev.bitly.com/docs/getting-started/authentication\n\
  \  http_status: 200\n  detail: >-\n    The authentication guide walks through the web flow, the resource-owner credentials grant and\n    HTTP Basic, and never mentions a `scope` parameter or a permissions reference page. There is\n    no scopes page in the dev.bitly.com sitemap.\n- source: openapi/_original/bitly-v4-openapi.json\n  detail: >-\n    The only securityScheme declared is `bearerAuth` (type http, scheme bearer). No oauth2 scheme,\n    therefore no flows.scopes to derive from. The derive-oauth-scopes pass found 0 oauth2 schemes.\nimplications: >-\n  A Bitly access token is all-or-nothing: it carries the full permissions of the granting user\n  across every group that user can reach, and there is no way to mint a read-only token, a\n  QR-only token, or a token scoped to a single group. That matters most on the MCP surface, where\n  the same undifferentiated bearer token grants an agent delete_short_link alongside get_user —\n  destructive and read operations are indistinguishable\
  \ to the authorization layer. Least-privilege\n  has to be enforced by provisioning a dedicated Bitly user restricted to one group, not by scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/scopes/bitly-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Links
- URL Shortener
- QR Codes
- Analytics
- Marketing
- Link Management
- Webhook
- Attribution
- Agents
- MCP
token_urls: []
---
