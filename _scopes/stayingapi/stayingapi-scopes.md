---
api_specs:
- filename: stayingapi-account-api-openapi.yml
  format: yaml
  label: StayingAPI Account API
  slug: stayingapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-account-api-openapi.yml
- filename: stayingapi-data-api-openapi.yml
  format: yaml
  label: StayingAPI Data API
  slug: stayingapi-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-data-api-openapi.yml
- filename: stayingapi-jobs-api-openapi.yml
  format: yaml
  label: StayingAPI Jobs API
  slug: stayingapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-jobs-api-openapi.yml
authorization_urls:
- https://mcp.stayingapi.com/mcp/oauth/authorize
description: StayingAPI's OAuth surface belongs to the hosted MCP server, not the REST API (REST uses a Bearer API key with no scopes). A single read scope is advertised by both the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata, which matches the server's posture of seven read-only tools.
docs: https://stayingapi.com/docs/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Stayingapi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'StayingAPI publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the StayingAPI API on a user''s behalf.


  Tokens are issued from https://mcp.stayingapi.com/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: StayingAPI
provider_slug: stayingapi
schemes:
- authorization_servers:
  - https://mcp.stayingapi.com/mcp/oauth
  flows:
  - authorizationUrl: https://mcp.stayingapi.com/mcp/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://mcp.stayingapi.com/mcp/oauth/register
    tokenUrl: https://mcp.stayingapi.com/mcp/oauth/token
  name: mcpOAuth
  resource: https://mcp.stayingapi.com/mcp
  source: well-known/stayingapi-oauth-authorization-server.json
scope_count: 1
scope_names:
- stays.read
scopes:
- description: Read-only access to StayingAPI accommodation data through the MCP server — search, availability, listing detail, price, cross-OTA price comparison, reviews and job polling. No write scope is published; every MCP tool is read-only.
  flows:
  - authorizationCode
  scope: stays.read
slug: stayingapi-scopes
source_filename: stayingapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://mcp.stayingapi.com/.well-known/oauth-authorization-server\ndocs: https://stayingapi.com/docs/mcp\ndescription: >-\n  StayingAPI's OAuth surface belongs to the hosted MCP server, not the REST API (REST uses a\n  Bearer API key with no scopes). A single read scope is advertised by both the RFC 8414\n  authorization-server metadata and the RFC 9728 protected-resource metadata, which matches\n  the server's posture of seven read-only tools.\nschemes:\n  - name: mcpOAuth\n    source: well-known/stayingapi-oauth-authorization-server.json\n    resource: https://mcp.stayingapi.com/mcp\n    authorization_servers:\n      - https://mcp.stayingapi.com/mcp/oauth\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.stayingapi.com/mcp/oauth/authorize\n        tokenUrl: https://mcp.stayingapi.com/mcp/oauth/token\n        registrationUrl: https://mcp.stayingapi.com/mcp/oauth/register\n        code_challenge_methods:\n\
  \          - S256\nscopes:\n  - scope: stays.read\n    description: >-\n      Read-only access to StayingAPI accommodation data through the MCP server — search,\n      availability, listing detail, price, cross-OTA price comparison, reviews and job\n      polling. No write scope is published; every MCP tool is read-only.\n    flows:\n      - authorizationCode\n    sources:\n      - well-known/stayingapi-oauth-authorization-server.json\n      - well-known/stayingapi-oauth-protected-resource.json\nnotes:\n  - The REST OpenAPI declares only http/bearer; it has no oauth2 securityScheme and therefore\n    no spec-derived scopes.\n  - >-\n    An insufficient-scope condition is present in the REST error catalog as sub-code\n    scope_insufficient (403 permission_denied).\nx-evidence:\n  - url: https://mcp.stayingapi.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.stayingapi.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/scopes/stayingapi-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- travel
- hospitality
- accommodation-data
- hotel-api
- vacation-rental
- short-term-rental
- airbnb
- booking.com
- vrbo
- google-hotels
- cross-ota-price-comparison
- availability
- reviews
- rest
- mcp
- agent-native
- openapi
token_urls:
- https://mcp.stayingapi.com/mcp/oauth/token
---
