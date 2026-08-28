---
api_specs:
- filename: sharethis-ai-summary-api-openapi.yml
  format: yaml
  label: ShareThis AI Summary API
  slug: sharethis-ai-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-ai-summary-api-openapi.yml
- filename: sharethis-apps-api-openapi.yml
  format: yaml
  label: ShareThis Apps API
  slug: sharethis-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-apps-api-openapi.yml
- filename: sharethis-audience-api-openapi.yml
  format: yaml
  label: ShareThis Audience API
  slug: sharethis-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-audience-api-openapi.yml
- filename: sharethis-authentication-api-openapi.yml
  format: yaml
  label: ShareThis Authentication API
  slug: sharethis-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-authentication-api-openapi.yml
- filename: sharethis-oauth-clients-api-openapi.yml
  format: yaml
  label: ShareThis OAuth Clients API
  slug: sharethis-oauth-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-oauth-clients-api-openapi.yml
- filename: sharethis-properties-api-openapi.yml
  format: yaml
  label: ShareThis Properties API
  slug: sharethis-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/openapi/sharethis-properties-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sharethis Scopes
name_suffix: OAuth Scopes
note: The OpenAPI document declares no oauth2 securityScheme, so derive-oauth-scopes.py correctly found nothing to derive from the spec. The scope surface here belongs to the MCP server instead, and was read directly from its live RFC 8414 / RFC 9728 discovery documents rather than from the contract.
overview: 'ShareThis uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ShareThis
provider_slug: sharethis
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: sharethis-scopes
source_filename: sharethis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://mcp.sharethis.com/.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource (2026-08-27)\nnote: >-\n  The OpenAPI document declares no oauth2 securityScheme, so derive-oauth-scopes.py correctly found\n  nothing to derive from the spec. The scope surface here belongs to the MCP server instead, and was\n  read directly from its live RFC 8414 / RFC 9728 discovery documents rather than from the contract.\nsurface: ShareThis MCP Server\nresource: https://mcp.sharethis.com\nauthorization_servers:\n- https://mcp.sharethis.com\nscopes:\n- name: mcp:tools\n  description: >-\n    Authorizes invocation of the ShareThis MCP tool set — property create/list/get/validate and app\n    upsert/list/get/delete/liveview.\n  source: scopes_supported in the authorization-server and protected-resource metadata\ngranularity:\n  level: coarse\n  assessment: >-\n    A single scope covers all nine tools, including the one\
  \ destructive operation\n    (sharethis_apps_delete). There is no read-only scope, so an agent granted access to list\n    properties is necessarily also granted the ability to delete an app configuration. Least\n    privilege is not expressible against this authorization server today.\nrest_api_scopes:\n  present: false\n  note: >-\n    The Platform API's bearer JWT carries no scopes — authorization is all-or-nothing on the\n    account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharethis/refs/heads/main/scopes/sharethis-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Social Sharing
- Website Tools
- Audience Data
- Advertising Technology
- Analytics
- Consent Management
- Publishing
- Model Context Protocol
token_urls: []
---
