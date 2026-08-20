---
api_specs:
- filename: opentravel-2020a-hotel-descriptive-content-resource-defs-openapi.json
  format: json
  label: OpenTravel 2020A Hotel Descriptive Content Resource
  slug: opentravel-2020a-hotel-descriptive-content-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2020a-hotel-descriptive-content-resource-defs-openapi.json
- filename: opentravel-2020a-facility-resource-defs-openapi.json
  format: json
  label: OpenTravel 2020A Facility Resource
  slug: opentravel-2020a-facility-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2020a-facility-resource-defs-openapi.json
- filename: opentravel-2018a-hospitality-offers-resource-defs-openapi.json
  format: json
  label: OpenTravel 2018A Hospitality Offers Resource
  slug: opentravel-2018a-hospitality-offers-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2018a-hospitality-offers-resource-defs-openapi.json
- filename: opentravel-2018a-facility-resource-defs-openapi.json
  format: json
  label: OpenTravel 2018A Facility Resource
  slug: opentravel-2018a-facility-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2018a-facility-resource-defs-openapi.json
authorization_urls:
- https://opentravel.org/oauth/authorize
description: ''
docs: https://opentravel.org/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Opentravel Alliance Scopes
name_suffix: OAuth Scopes
note: The published OpenTravel Swagger 2.0 contracts declare no oauth2 security schemes, so derive-oauth-scopes.py returned nothing for this provider. The scope surface below is the real one advertised by the OAuth 2.1 authorization server that opentravel.org runs in front of its Model Context Protocol endpoints. It is a single coarse scope; there is no per-tool or per-resource scope decomposition published, and none is invented here.
overview: 'OpenTravel Alliance publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the OpenTravel Alliance API on a user''s behalf.


  Tokens are issued from https://opentravel.org/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OpenTravel Alliance
provider_slug: opentravel-alliance
schemes:
- flows:
  - authorizationUrl: https://opentravel.org/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://opentravel.org/oauth/token
  name: opentravel-mcp-oauth
  source: well-known/opentravel-alliance-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the OpenTravel Model Context Protocol server at https://opentravel.org/wp-json/mcp/mcp-oauth-server. Advertised as scopes_supported by both the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata.
  flows:
  - authorizationCode
  scope: mcp
slug: opentravel-alliance-scopes
source_filename: opentravel-alliance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://opentravel.org/.well-known/oauth-authorization-server\ndocs: https://opentravel.org/.well-known/oauth-protected-resource\nnote: >-\n  The published OpenTravel Swagger 2.0 contracts declare no oauth2 security schemes, so\n  derive-oauth-scopes.py returned nothing for this provider. The scope surface below is the\n  real one advertised by the OAuth 2.1 authorization server that opentravel.org runs in front\n  of its Model Context Protocol endpoints. It is a single coarse scope; there is no per-tool\n  or per-resource scope decomposition published, and none is invented here.\nschemes:\n- name: opentravel-mcp-oauth\n  source: well-known/opentravel-alliance-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://opentravel.org/oauth/authorize\n    tokenUrl: https://opentravel.org/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n    Access the OpenTravel Model Context Protocol\
  \ server at\n    https://opentravel.org/wp-json/mcp/mcp-oauth-server. Advertised as scopes_supported by\n    both the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource\n    metadata.\n  flows: [authorizationCode]\n  sources:\n  - well-known/opentravel-alliance-oauth-authorization-server.json\n  - well-known/opentravel-alliance-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/scopes/opentravel-alliance-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Travel
- United States
- Standards
- Aviation
- Hospitality
- Hotels
- Car Rental
- Rail
- Cruise
- Distribution
- GDS
- Booking
- Channel
- XML
- JSON-Schema
token_urls:
- https://opentravel.org/oauth/token
---
