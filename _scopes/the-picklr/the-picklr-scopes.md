---
api_specs:
- filename: the-picklr-categories-api-openapi.yml
  format: yaml
  label: The Picklr Categories API
  slug: the-picklr-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-categories-api-openapi.yml
- filename: the-picklr-club-clinics-api-openapi.yml
  format: yaml
  label: The Picklr Club Clinics API
  slug: the-picklr-club-clinics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-club-clinics-api-openapi.yml
- filename: the-picklr-event-api-openapi.yml
  format: yaml
  label: The Picklr Event API
  slug: the-picklr-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-event-api-openapi.yml
- filename: the-picklr-location-api-openapi.yml
  format: yaml
  label: The Picklr Location API
  slug: the-picklr-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-location-api-openapi.yml
- filename: the-picklr-media-api-openapi.yml
  format: yaml
  label: The Picklr Media API
  slug: the-picklr-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-media-api-openapi.yml
- filename: the-picklr-pages-api-openapi.yml
  format: yaml
  label: The Picklr Pages API
  slug: the-picklr-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-pages-api-openapi.yml
- filename: the-picklr-posts-api-openapi.yml
  format: yaml
  label: The Picklr Posts API
  slug: the-picklr-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-posts-api-openapi.yml
- filename: the-picklr-press-api-openapi.yml
  format: yaml
  label: The Picklr Press API
  slug: the-picklr-press-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-press-api-openapi.yml
- filename: the-picklr-search-api-openapi.yml
  format: yaml
  label: The Picklr Search API
  slug: the-picklr-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-search-api-openapi.yml
- filename: the-picklr-tags-api-openapi.yml
  format: yaml
  label: The Picklr Tags API
  slug: the-picklr-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-tags-api-openapi.yml
- filename: the-picklr-taxonomies-api-openapi.yml
  format: yaml
  label: The Picklr Taxonomies API
  slug: the-picklr-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-taxonomies-api-openapi.yml
- filename: the-picklr-types-api-openapi.yml
  format: yaml
  label: The Picklr Types API
  slug: the-picklr-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-types-api-openapi.yml
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
