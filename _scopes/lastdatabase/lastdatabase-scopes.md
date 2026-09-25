---
api_specs:
- filename: lastdatabase-openapi.yml
  format: yaml
  label: LastDatabase Lead Search API
  slug: lead-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lastdatabase/refs/heads/main/openapi/lastdatabase-openapi.yml
authorization_urls: []
description: ''
docs: https://lastdatabase.com/docs/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Lastdatabase Scopes
name_suffix: OAuth Scopes
note: All nine scopes are listed in scopes_supported of both the authorization-server and protected-resource metadata (HTTP 200). Only credits:read, people:search and email:verify are tied to a documented tool; the other six carry no published description.
overview: 'LastDatabase uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LastDatabase
provider_slug: lastdatabase
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: lastdatabase-scopes
source_filename: lastdatabase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-09-23''

  method: searched

  source: https://lastdatabase.com/.well-known/oauth-authorization-server

  docs: https://lastdatabase.com/docs/mcp

  applies_to: LastDatabase MCP Server (https://lastdatabase.com/mcp); the REST Lead Search API uses a Bearer API key, not OAuth.

  scopes:

  - {name: ''profile:read'', description: null, source: scopes_supported}

  - {name: ''credits:read'', description: Read subscription record allowance (get_credits)., source: https://lastdatabase.com/docs/mcp}

  - {name: ''people:search'', description: Search B2B contacts and unlock an eligible contact (search_people, unlock_people)., source: https://lastdatabase.com/docs/mcp}

  - {name: ''companies:search'', description: null, source: scopes_supported}

  - {name: ''email:find'', description: null, source: scopes_supported}

  - {name: ''email:verify'', description: Verify a supplied business email address (verify_email)., source: https://lastdatabase.com/docs/mcp}

  - {name: ''phone:find'', description: null, source: scopes_supported}

  - {name: ''person:enrich'', description: null, source: scopes_supported}

  - {name: ''company:enrich'', description: null, source: scopes_supported}

  note: All nine scopes are listed in scopes_supported of both the authorization-server and protected-resource metadata (HTTP 200). Only credits:read, people:search and email:verify are tied to a documented tool; the other six carry no published description.

  '
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lastdatabase/refs/heads/main/scopes/lastdatabase-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Contact Data
- Lead Generation
- B2B Data
- Email Verification
- Data Enrichment
- Sales Prospecting
- MCP
token_urls: []
---
