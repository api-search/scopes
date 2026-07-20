---
api_specs:
- filename: kernel-openapi-original.yml
  format: yaml
  label: Kernel API
  slug: kernel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-openapi-original.yml
authorization_urls: []
description: ''
docs: https://kernel.sh/docs/reference/mcp-server/authentication.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kernel Scopes
name_suffix: OAuth Scopes
note: The Kernel REST API OpenAPI declares a single bearer (API key) scheme without oauth2 flows, but the RFC 8414 authorization-server metadata advertises OAuth 2.1 (used by the hosted MCP server, with dynamic client registration) and two coarse scopes. Scopes are captured from the well-known document verbatim.
overview: 'Kernel publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kernel API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kernel
provider_slug: kernel
schemes:
- bearer_methods_supported:
  - header
  dynamic_client_registration: true
  flows:
  - flow: authorizationCode
    note: OAuth 2.1 with dynamic client registration; used by the hosted MCP server.
  issuer: https://api.onkernel.com/
  name: OAuth2.1
  source: https://api.onkernel.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- api.read
- api.write
scopes:
- description: Read access to Kernel API resources.
  flows: []
  scope: api.read
- description: Write access to Kernel API resources.
  flows: []
  scope: api.write
slug: kernel-scopes
source_filename: kernel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.onkernel.com/.well-known/oauth-authorization-server\ndocs: https://kernel.sh/docs/reference/mcp-server/authentication.md\nnote: >-\n  The Kernel REST API OpenAPI declares a single bearer (API key) scheme without\n  oauth2 flows, but the RFC 8414 authorization-server metadata advertises OAuth 2.1\n  (used by the hosted MCP server, with dynamic client registration) and two coarse\n  scopes. Scopes are captured from the well-known document verbatim.\nschemes:\n  - name: OAuth2.1\n    source: https://api.onkernel.com/.well-known/oauth-authorization-server\n    issuer: https://api.onkernel.com/\n    bearer_methods_supported: [header]\n    dynamic_client_registration: true\n    flows:\n      - flow: authorizationCode\n        note: OAuth 2.1 with dynamic client registration; used by the hosted MCP server.\nscopes:\n  - scope: api.read\n    description: Read access to Kernel API resources.\n    sources: [https://api.onkernel.com/.well-known/oauth-authorization-server]\n\
  \  - scope: api.write\n    description: Write access to Kernel API resources.\n    sources: [https://api.onkernel.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/scopes/kernel-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Browser Automation
- Web Agents
- Browser Infrastructure
- AI Agents
- Playwright
- Cloud Browsers
- Computer Use
- MCP
- Managed Auth
token_urls: []
---
