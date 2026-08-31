---
api_specs:
- filename: browser-use-api-v4-openapi.json
  format: json
  label: Browser Use Public API v4
  slug: browser-use-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v4-openapi.json
- filename: browser-use-api-v3-openapi.json
  format: json
  label: Browser Use Public API v3
  slug: browser-use-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v3-openapi.json
- filename: browser-use-api-v2-openapi.json
  format: json
  label: Browser Use Public API v2
  slug: browser-use-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-api-v2-openapi.json
authorization_urls: []
description: ''
docs: https://browser-use.com/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Browser Use Scopes
name_suffix: OAuth Scopes
note: Derived from the live OAuth 2.0 authorization-server metadata, not from an OpenAPI oauth2 securityScheme — none of the three published OpenAPI documents declares an oauth2 flow. The authorization server exists to protect the hosted MCP resource, and it advertises exactly one scope.
overview: 'Browser Use uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Browser Use
provider_slug: browser-use
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: browser-use-scopes
source_filename: browser-use-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://browser-use.com/.well-known/oauth-authorization-server\ndocs: https://browser-use.com/auth.md\nnote: >-\n  Derived from the live OAuth 2.0 authorization-server metadata, not from an OpenAPI oauth2\n  securityScheme — none of the three published OpenAPI documents declares an oauth2 flow. The\n  authorization server exists to protect the hosted MCP resource, and it advertises exactly one scope.\nauthorization_server:\n  issuer: https://api.browser-use.com\n  metadata_url: https://browser-use.com/.well-known/oauth-authorization-server\n  http_status: 200\n  protected_resource: https://api.browser-use.com/mcp\n  protected_resource_metadata_url: https://api.browser-use.com/.well-known/oauth-protected-resource\n  http_status_protected_resource: 200\n  dynamic_client_registration: true\n  grant_types:\n  - authorization_code\n  - urn:ietf:params:oauth:grant-type:device_code\n  code_challenge_methods:\n  - S256\nscope_count:\
  \ 1\nscopes:\n- name: mcp\n  description: >-\n    Access the Browser Use hosted MCP resource at https://api.browser-use.com/mcp. This is the only\n    permission published in the authorization-server metadata.\n  resource: https://api.browser-use.com/mcp\n  source: https://browser-use.com/.well-known/oauth-authorization-server\ngaps:\n- >-\n  No per-operation or per-resource scopes are published for the v2/v3/v4 REST APIs. An API key is\n  all-or-nothing against a project, which is a real constraint for agent delegation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/scopes/browser-use-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI Automation
- Browser Automation
- Web Agents
- Web Scraping
- Headless Browsers
- Agent Infrastructure
- Model Context Protocol
- Cloud Browsers
token_urls: []
---
