---
api_specs:
- filename: paedae-applications-api-openapi.yml
  format: yaml
  label: Paedae Applications API
  slug: paedae-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-applications-api-openapi.yml
- filename: paedae-beacon-configurations-api-openapi.yml
  format: yaml
  label: Paedae Beacon Configurations API
  slug: paedae-beacon-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacon-configurations-api-openapi.yml
- filename: paedae-beacons-api-openapi.yml
  format: yaml
  label: Paedae Beacons API
  slug: paedae-beacons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacons-api-openapi.yml
- filename: paedae-communications-api-openapi.yml
  format: yaml
  label: Paedae Communications API
  slug: paedae-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-communications-api-openapi.yml
- filename: paedae-places-api-openapi.yml
  format: yaml
  label: Paedae Places API
  slug: paedae-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-places-api-openapi.yml
authorization_urls:
- https://manager.gimbal.com/oauth/authorize
- https://mcp.infillion.com/oauth/authorize
description: ''
docs: https://docs.gimbal.com/rest.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Paedae Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Paedae uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://manager.gimbal.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paedae
provider_slug: paedae
schemes:
- description: Transmitter (beacon) Proximity APIs require a user OAuth access token passed as a query parameter — `POST /api/v1/transmitters?access_token={token}`. Access is implicitly limited to transmitters owned by the account behind the token; no scope names are documented.
  flows:
  - authorizationUrl: https://manager.gimbal.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://manager.gimbal.com/oauth/token
  name: ProximityOAuth2
  scopes: []
  scopes_documented: false
  source: openapi/paedae-rest-openapi.yml + https://docs.gimbal.com/rest.html
- description: 'Authorization server fronting the parent''s remote MCP endpoint (https://mcp.infillion.com/mcp). Parent-brand surface: paedae.com and gimbal.com both redirect to infillion.com.'
  flows:
  - authorizationUrl: https://mcp.infillion.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp.infillion.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.infillion.com
  name: InfillionAgentConnector
  note: The metadata document contains no `scopes_supported` member, so a client cannot discover what permissions it may request before registering.
  registration_endpoint: https://mcp.infillion.com/register
  scopes: []
  scopes_documented: false
  source: https://mcp.infillion.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
scope_count: 0
scope_names: []
scopes: []
slug: paedae-scopes
source_filename: paedae-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.gimbal.com/rest.html (transmitter/Proximity OAuth) and live\n  probe of https://mcp.infillion.com/.well-known/oauth-authorization-server\n  (HTTP 200, 2026-08-13). Baseline derived from\n  openapi/paedae-rest-openapi.yml.\ntype: OAuthScopes\nprovider: Paedae (Gimbal proximity platform, operated by Infillion)\nsummary: >-\n  Two OAuth 2.0 authorization servers exist across this company's estate and\n  NEITHER publishes a scope vocabulary. Gimbal's transmitter APIs take an\n  opaque `access_token` query parameter with no documented scopes; the parent's\n  MCP gateway publishes RFC 8414 metadata that omits `scopes_supported`\n  entirely. There is nothing to enumerate — this is a published absence, not an\n  unchecked field.\nschemes:\n  - name: ProximityOAuth2\n    source: openapi/paedae-rest-openapi.yml + https://docs.gimbal.com/rest.html\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://manager.gimbal.com/oauth/authorize\n        tokenUrl: https://manager.gimbal.com/oauth/token\n    description: >-\n      Transmitter (beacon) Proximity APIs require a user OAuth access token\n      passed as a query parameter — `POST /api/v1/transmitters?access_token={token}`.\n      Access is implicitly limited to transmitters owned by the account behind\n      the token; no scope names are documented.\n    scopes: []\n    scopes_documented: false\n  - name: InfillionAgentConnector\n    source: https://mcp.infillion.com/.well-known/oauth-authorization-server\n    issuer: https://mcp.infillion.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.infillion.com/oauth/authorize\n        tokenUrl: https://mcp.infillion.com/oauth/token\n        pkce: S256\n    registration_endpoint: https://mcp.infillion.com/register\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n    token_endpoint_auth_methods_supported:\n      -\
  \ none\n    description: >-\n      Authorization server fronting the parent's remote MCP endpoint\n      (https://mcp.infillion.com/mcp). Parent-brand surface: paedae.com and\n      gimbal.com both redirect to infillion.com.\n    scopes: []\n    scopes_documented: false\n    note: >-\n      The metadata document contains no `scopes_supported` member, so a client\n      cannot discover what permissions it may request before registering.\nscopes: []\ndocs: https://docs.gimbal.com/rest.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/scopes/paedae-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Proximity
- Location
- Beacons
- Geofencing
- Mobile SDK
- Advertising
- Marketing
token_urls:
- https://manager.gimbal.com/oauth/token
- https://mcp.infillion.com/oauth/token
---
