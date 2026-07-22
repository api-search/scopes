---
authorization_urls:
- https://mcp.pointfive.co/authorize
description: ''
docs: https://www.pointfive.co/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Pointfive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pointfive publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pointfive API on a user''s behalf.


  Tokens are issued from https://mcp.pointfive.co/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pointfive
provider_slug: pointfive
schemes:
- flows:
  - authorizationUrl: https://mcp.pointfive.co/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.pointfive.co/token
  name: OAuth2
  source: well-known/pointfive-oauth-authorization-server.json
scope_count: 2
scope_names:
- api:read
- api:write
scopes:
- description: Read access to PointFive data (opportunities, resources, anomalies, commitments).
  flows:
  - authorizationCode
  scope: api:read
- description: Write access to PointFive data.
  flows:
  - authorizationCode
  scope: api:write
slug: pointfive-scopes
source_filename: pointfive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mcp.pointfive.co/.well-known/oauth-authorization-server\ndocs: https://www.pointfive.co/mcp\nschemes:\n- name: OAuth2\n  source: well-known/pointfive-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.pointfive.co/authorize\n    tokenUrl: https://mcp.pointfive.co/token\nscopes:\n- scope: api:read\n  description: Read access to PointFive data (opportunities, resources, anomalies, commitments).\n  flows: [authorizationCode]\n  sources: [well-known/pointfive-oauth-authorization-server.json]\n- scope: api:write\n  description: Write access to PointFive data.\n  flows: [authorizationCode]\n  sources: [well-known/pointfive-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointfive/refs/heads/main/scopes/pointfive-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Cloud Saas
- FinOps
- Cloud Cost Optimization
- Cloud Infrastructure
- Kubernetes
- AI Infrastructure
- MCP
token_urls:
- https://mcp.pointfive.co/token
---
