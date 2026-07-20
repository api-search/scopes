---
api_specs:
- filename: archera-openapi-original.json
  format: json
  label: Archera Public API
  slug: archera-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-openapi-original.json
authorization_urls:
- https://api.archera.ai/oauth/authorize
description: OAuth 2.0 scopes advertised by the Archera authorization server (scopes_supported) and echoed by the MCP protected-resource metadata at https://mcp.archera.ai/.well-known/oauth-protected-resource/mcp. The OpenAPI does not enumerate per-operation scope requirements, so scope-to-operation mapping is inferred from the read/write naming convention.
docs: https://docs.archera.ai/api-reference/public-api/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Archera Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Archera publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Archera API on a user''s behalf.


  Tokens are issued from https://api.archera.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Archera
provider_slug: archera
schemes:
- flows:
  - authorizationUrl: https://api.archera.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.archera.ai/oauth/token
  name: oauth2
  source: https://api.archera.ai/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- archera:read
- archera:write
- archera:admin
- archera:analytics
scopes:
- description: Read access to Archera resources (commitment plans, commitments, metrics, resources, orgs).
  flows:
  - authorizationCode
  scope: archera:read
- description: Write access to Archera resources (apply commitment plans, apply exchange recommendations, uploads).
  flows:
  - authorizationCode
  scope: archera:write
- description: Administrative access to the Archera organization.
  flows:
  - authorizationCode
  scope: archera:admin
- description: Access to analytics and reporting data.
  flows:
  - authorizationCode
  scope: archera:analytics
slug: archera-scopes
source_filename: archera-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.archera.ai/.well-known/oauth-authorization-server\ndocs: https://docs.archera.ai/api-reference/public-api/oauth\ndescription: >-\n  OAuth 2.0 scopes advertised by the Archera authorization server\n  (scopes_supported) and echoed by the MCP protected-resource metadata at\n  https://mcp.archera.ai/.well-known/oauth-protected-resource/mcp. The OpenAPI\n  does not enumerate per-operation scope requirements, so scope-to-operation\n  mapping is inferred from the read/write naming convention.\nschemes:\n- name: oauth2\n  source: https://api.archera.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.archera.ai/oauth/authorize\n    tokenUrl: https://api.archera.ai/oauth/token\nscopes:\n- scope: archera:read\n  description: Read access to Archera resources (commitment plans, commitments, metrics, resources, orgs).\n  flows: [authorizationCode]\n  sources: [https://api.archera.ai/.well-known/oauth-authorization-server]\n\
  - scope: archera:write\n  description: Write access to Archera resources (apply commitment plans, apply exchange recommendations, uploads).\n  flows: [authorizationCode]\n  sources: [https://api.archera.ai/.well-known/oauth-authorization-server]\n- scope: archera:admin\n  description: Administrative access to the Archera organization.\n  flows: [authorizationCode]\n  sources: [https://api.archera.ai/.well-known/oauth-authorization-server]\n- scope: archera:analytics\n  description: Access to analytics and reporting data.\n  flows: [authorizationCode]\n  sources: [https://api.archera.ai/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/scopes/archera-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Developer Tools
- FinOps
- Cloud Cost Management
- Cloud Commitments
- Cost Optimization
- MCP
- Azure
- Google Cloud
token_urls:
- https://api.archera.ai/oauth/token
---
