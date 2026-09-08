---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Listings API
  slug: listings-api
  spec_type: OpenAPI
  url: https://listingsapi.com/openapi.yaml
authorization_urls: []
description: ''
docs: https://docs.listingsapi.com/docs/authentication
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Listings Api Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Listings API uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Listings API
provider_slug: listings-api
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: listings-api-scopes
source_filename: listings-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: https://listingsapi.com/.well-known/oauth-authorization-server, https://listingsapi.com/.well-known/oauth-protected-resource, https://docs.listingsapi.com/docs/authentication, https://github.com/listings-api/listingsapi-mcp (README)\ndocs: https://docs.listingsapi.com/docs/authentication\noauth:\n  applies_to: MCP server (https://listingsapi.com/mcp) only; the REST API authenticates with static API keys.\n  issuer: https://listingsapi.com\n  authorization_endpoint: https://listingsapi.com/oauth/authorize\n  token_endpoint: https://listingsapi.com/oauth/token\n  registration_endpoint: https://listingsapi.com/oauth/register\n  revocation_endpoint: https://listingsapi.com/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  pkce: S256\n  token_endpoint_auth: none\nscopes:\n  - name: read\n    description: >-\n      Read access - every lookup and report: locations, listings and citations, reviews,\n      posts, analytics.\
  \ Mirrors the \"Read\" access level on API keys.\n  - name: write\n    description: >-\n      Write access - create/update locations, reply to reviews, publish posts, connect\n      accounts. Mirrors the \"Write\" access level on API keys.\nnotes: >-\n  scopes_supported [read, write] comes from the provider's own RFC 8414 discovery document.\n  API keys carry the same two access levels (Read or Write), chosen at key creation in the\n  dashboard; OAuth consent on the MCP server materialises as an API key named after the client.\n  A key with Read access covers every lookup; writes need Write access (403 on a write means a\n  Read-only key).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/scopes/listings-api-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Business Listings
- Local SEO
- Locations
- Reviews
- Google Business Profile
- Analytics
- citation-management
- Local Marketing
- social-publishing
- MCP
- agent-native
token_urls: []
---
