---
api_specs:
- filename: ipstack
  format: yaml
  label: ipstack REST API
  slug: ipstack-rest-api
  spec_type: Postman
  url: https://www.postman.com/apilayer/apilayer/collection/1jn3xlj/ipstack
authorization_urls: []
description: The APILayer authorization server publishes its scope list in discovery. Two of the five scopes are product scopes and one of them names IPstack explicitly — api:ipstack — which is also the ownership proof that mcp.apilayer.com is IPstack's own agent surface and not a sibling product's.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ipstack Scopes
name_suffix: OAuth Scopes
note: APILayer publishes no human-readable scopes/permissions reference page; the scope list exists only in the machine-readable discovery documents. That is recorded as an honest gap rather than filled in.
overview: 'IPstack uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IPstack
provider_slug: ipstack
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ipstack-scopes
source_filename: ipstack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://auth.apilayer.com/.well-known/oauth-authorization-server (HTTP 200) and\n  https://mcp.apilayer.com/.well-known/oauth-protected-resource (HTTP 200). Both fetched\n  anonymously on 2026-09-04 and saved verbatim under well-known/. derive-oauth-scopes.py\n  produced nothing because no OpenAPI with oauth2 securitySchemes is published.\nname: IPstack / APILayer OAuth scopes\ndescription: >-\n  The APILayer authorization server publishes its scope list in discovery. Two of the five\n  scopes are product scopes and one of them names IPstack explicitly — api:ipstack — which\n  is also the ownership proof that mcp.apilayer.com is IPstack's own agent surface and not\n  a sibling product's.\nissuer: https://auth.apilayer.com\nresource: https://mcp.apilayer.com/mcp\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n    source: authorization-server metadata scopes_supported\n \
  \ - name: offline\n    description: Requests a refresh token (Ory/Hydra-style alias of offline_access).\n    source: authorization-server metadata scopes_supported\n  - name: offline_access\n    description: Standard OIDC scope requesting a refresh token for long-lived agent sessions.\n    source: authorization-server metadata scopes_supported\n  - name: mcp:read\n    description: >-\n      Read access through the APILayer MCP server. Advertised by the protected-resource\n      document at mcp.apilayer.com as one of the two scopes that endpoint accepts.\n    source: both authorization-server and protected-resource metadata\n  - name: api:ipstack\n    description: >-\n      Access to the IPstack product surface through an APILayer token. The only\n      product-named scope in the discovery document.\n    source: both authorization-server and protected-resource metadata\ndocs: null\nnote: >-\n  APILayer publishes no human-readable scopes/permissions reference page; the scope list\n  exists\
  \ only in the machine-readable discovery documents. That is recorded as an honest\n  gap rather than filled in.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipstack/refs/heads/main/scopes/ipstack-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Geocoding
- IP Geolocation
- Location
- Threat Intelligence
- Networking
- MCP
- Public APIs
token_urls: []
---
