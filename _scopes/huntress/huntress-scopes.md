---
api_specs:
- filename: huntress-rest-openapi.json
  format: json
  label: Huntress REST API
  slug: huntress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/openapi/huntress-rest-openapi.json
authorization_urls:
- https://api.huntress.io/v1/mcp/authorize
description: ''
docs: https://api.huntress.io/.well-known/oauth-protected-resource
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Huntress Scopes
name_suffix: OAuth Scopes
note: The Huntress REST API uses HTTP Basic auth (no OAuth scopes). OAuth 2.1 applies only to the remote MCP server, whose authorization-server metadata advertises a single coarse-grained scope.
overview: 'Huntress publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Huntress API on a user''s behalf.


  Tokens are issued from https://api.huntress.io/v1/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Huntress
provider_slug: huntress
schemes:
- flows:
  - authorizationUrl: https://api.huntress.io/v1/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://api.huntress.io/v1/mcp/token
  - flow: clientCredentials
    tokenUrl: https://api.huntress.io/v1/mcp/token
  name: MCP OAuth
  source: https://api.huntress.io/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants an OAuth client access to the Huntress remote MCP server.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp
slug: huntress-scopes
source_filename: huntress-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.huntress.io/.well-known/oauth-authorization-server\ndocs: https://api.huntress.io/.well-known/oauth-protected-resource\nnote: >-\n  The Huntress REST API uses HTTP Basic auth (no OAuth scopes). OAuth 2.1 applies\n  only to the remote MCP server, whose authorization-server metadata advertises a\n  single coarse-grained scope.\nschemes:\n  - name: MCP OAuth\n    source: https://api.huntress.io/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.huntress.io/v1/mcp/authorize\n        tokenUrl: https://api.huntress.io/v1/mcp/token\n      - flow: clientCredentials\n        tokenUrl: https://api.huntress.io/v1/mcp/token\nscopes:\n  - scope: mcp\n    description: Grants an OAuth client access to the Huntress remote MCP server.\n    flows: [authorizationCode, clientCredentials]\n    sources: [https://api.huntress.io/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huntress/refs/heads/main/scopes/huntress-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Endpoint Security
- SOC
- SIEM
- Identity Threat Detection
- MSP
- Webhooks
token_urls:
- https://api.huntress.io/v1/mcp/token
---
