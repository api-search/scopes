---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Acelab Scopes
name_suffix: OAuth Scopes
note: 'The only OAuth scope Acelab publishes anywhere is the single scope advertised by the authorization server backing the documentation MCP server on docs.acelabusa.com. There is no scope or permissions reference page for the Acelab product API — that API answers WWW-Authenticate: Bearer with no published authorization model at all. This file deliberately records one scope rather than inventing a product-API scope surface.'
overview: 'Acelab uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Acelab
provider_slug: acelab
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: acelab-scopes
source_filename: acelab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://docs.acelabusa.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  The only OAuth scope Acelab publishes anywhere is the single scope advertised by the\n  authorization server backing the documentation MCP server on docs.acelabusa.com. There is no\n  scope or permissions reference page for the Acelab product API — that API answers\n  WWW-Authenticate: Bearer with no published authorization model at all. This file deliberately\n  records one scope rather than inventing a product-API scope surface.\nauthorization_server: https://docs.acelabusa.com/mcp/oauth\ngrant_types:\n- authorization_code\n- client_credentials\n- refresh_token\ncode_challenge_methods:\n- S256\ndynamic_client_registration: true\nscope_count: 1\nscopes:\n- name: mcp:search\n  description: >-\n    Search and retrieve Acelab documentation content through the MCP server at\n    https://docs.acelabusa.com/mcp. Anonymous callers can already\
  \ list and call the read-only\n    tools; this scope gates authenticated/private documentation content.\n  resource: https://docs.acelabusa.com\nx-evidence:\n  fetched: '2026-09-06'\n  url: https://docs.acelabusa.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acelab/refs/heads/main/scopes/acelab-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Construction
- Architecture
- Building Materials
- Design
- Sustainability
- Product Data
- AECO
- Revit
- Specification
token_urls: []
---
