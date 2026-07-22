---
api_specs:
- filename: precog-public-http-api-openapi.yaml
  format: yaml
  label: Precog Public HTTP API
  slug: precog-public-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-public-http-api-openapi.yaml
authorization_urls:
- https://studio.precog.cloud/api/mcp/oauth/authorize
description: ''
docs: https://studio.precog.cloud/.well-known/oauth-protected-resource
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Precog Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Precog publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Precog API on a user''s behalf.


  Tokens are issued from https://studio.precog.cloud/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Precog
provider_slug: precog
schemes:
- flows:
  - authorizationUrl: https://studio.precog.cloud/api/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token
  - flow: clientCredentials
    tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token
  name: PrecogMcpOAuth
  source: https://studio.precog.cloud/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 3
scope_names:
- synesis:mcp
- admin:read
- admin:write
scopes:
- description: Access the Precog (Synesis) Model Context Protocol server and its tools.
  flows:
  - authorizationCode
  - clientCredentials
  scope: synesis:mcp
- description: Read access to administrative resources over the MCP surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: admin:read
- description: Write/administrative access over the MCP surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: admin:write
slug: precog-scopes
source_filename: precog-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://studio.precog.cloud/.well-known/oauth-authorization-server\ndocs: https://studio.precog.cloud/.well-known/oauth-protected-resource\nnotes: >-\n  These OAuth 2.0 scopes are advertised by Precog's MCP authorization server\n  (RFC 8414 metadata). They govern the OAuth-secured MCP surface at\n  studio.precog.cloud. The public HTTP REST API (openapi/) itself uses opaque\n  bearer tokens (HTTP Bearer) rather than scoped OAuth, so its scheme carries no\n  scope list.\nschemes:\n- name: PrecogMcpOAuth\n  type: oauth2\n  source: https://studio.precog.cloud/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://studio.precog.cloud/api/mcp/oauth/authorize\n    tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://studio.precog.cloud/api/mcp/oauth/token\nscopes:\n- scope: synesis:mcp\n  description: Access the Precog (Synesis)\
  \ Model Context Protocol server and its tools.\n  flows: [authorizationCode, clientCredentials]\n- scope: admin:read\n  description: Read access to administrative resources over the MCP surface.\n  flows: [authorizationCode, clientCredentials]\n- scope: admin:write\n  description: Write/administrative access over the MCP surface.\n  flows: [authorizationCode, clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/scopes/precog-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Data Integration
- ETL
- Artificial Intelligence
- Semantic Layer
- Model Context Protocol
- Data Pipelines
- Analytics
- Enterprise
token_urls:
- https://studio.precog.cloud/api/mcp/oauth/token
---
