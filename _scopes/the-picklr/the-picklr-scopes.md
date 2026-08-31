---
api_specs:
- filename: the-picklr-wordpress-rest-openapi.json
  format: json
  label: The Picklr WordPress REST API
  slug: the-picklr-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-wordpress-rest-openapi.json
authorization_urls: []
description: The authorization server publishes exactly one scope. It is recorded here verbatim from the RFC 8414 metadata document; no additional scopes are inferred, and no scope reference page exists on the site to enrich them from.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: The Picklr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'The Picklr uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Picklr
provider_slug: the-picklr
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: the-picklr-scopes
source_filename: the-picklr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://thepicklr.com/.well-known/oauth-authorization-server\nname: The Picklr — OAuth scopes\ndescription: >-\n  The authorization server publishes exactly one scope. It is recorded here verbatim from the\n  RFC 8414 metadata document; no additional scopes are inferred, and no scope reference page\n  exists on the site to enrich them from.\nauthorization_server: https://thepicklr.com\nmetadata: https://thepicklr.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: The provider publishes no scopes or permissions reference page.\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Access the Model Context Protocol server exposed at\n    https://thepicklr.com/wp-json/mcp/novamira-oauth. The authorization server declares no\n    finer-grained scopes, so this single scope is all-or-nothing for the MCP surface.\n  source: scopes_supported\n  granularity: coarse\nconsent:\n  pkce_required: true\n  code_challenge_methods:\
  \ [S256]\n  token_endpoint_auth_methods: [none]\nx-evidence:\n  fetched: '2026-08-30'\n  url: https://thepicklr.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/scopes/the-picklr-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Sports
- Pickleball
- Fitness
- Franchising
- Recreation
- Health and Wellness
- Consumer
- Content Management
- MCP
token_urls: []
---
