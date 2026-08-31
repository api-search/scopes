---
api_specs:
- filename: seamless-ai-public-api-openapi-original.json
  format: json
  label: Seamless.AI Public API
  slug: seamless-ai-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/_original/seamless-ai-public-api-openapi-original.json
- filename: seamless-ai-mcp-api-openapi.yml
  format: yaml
  label: Seamless.AI MCP API
  slug: seamless-ai-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/seamless-ai-mcp-api-openapi.yml
authorization_urls:
- https://login.seamless.ai/oauth/authorize
description: ''
docs: https://docs.seamless.ai/authentication/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Seamless Ai Scopes
name_suffix: OAuth Scopes
note: 'The derived pass found the oauth2 scheme but ZERO scopes, because the published OpenAPI declares `scopes: {}` on its authorizationCode flow — the scope vocabulary is absent from the machine- readable contract. Both real scopes below were recovered from the documentation and from the MCP authorization-server metadata, so this file is upgraded to `searched`. Seamless.AI operates two separate OAuth surfaces with two separate authorization servers and two disjoint scope vocabularies; they are not interchangeable.'
overview: 'Seamless.AI publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Seamless.AI API on a user''s behalf.


  Tokens are issued from https://api.seamless.ai/api/client/v1/oauth/accessToken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Seamless.AI
provider_slug: seamless-ai
schemes:
- flows:
  - authorizationUrl: https://login.seamless.ai/oauth/authorize
    flow: authorizationCode
    scopes_declared: 0
    tokenUrl: https://api.seamless.ai/api/client/v1/oauth/accessToken
  name: OAuth2
  source: openapi/_original/seamless-ai-public-api-openapi-original.json
scope_count: 2
scope_names:
- publicAPI.v1.all
- mcp.all
scopes:
- description: Full access to the Seamless.AI Public API v1 — search, research, polling and org-data reads. The only REST scope published.
  flows:
  - authorizationCode
  scope: publicAPI.v1.all
- description: Full MCP access — all 54 tools and all seamless:// resources the org is licensed for.
  flows:
  - authorizationCode
  scope: mcp.all
slug: seamless-ai-scopes
source_filename: seamless-ai-scopes.yml
source_heading: OAuth Scopes
source_url: https://docs.seamless.ai/authentication/oauth
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/_original/seamless-ai-public-api-openapi-original.json\ndocs: https://docs.seamless.ai/authentication/oauth\nsources:\n  - https://docs.seamless.ai/authentication/oauth\n  - https://docs.seamless.ai/api-http-status-codes\n  - https://mcp.seamless.ai/.well-known/oauth-protected-resource\n  - openapi/_original/seamless-ai-public-api-openapi-original.json\nnote: >-\n  The derived pass found the oauth2 scheme but ZERO scopes, because the published OpenAPI declares\n  `scopes: {}` on its authorizationCode flow — the scope vocabulary is absent from the machine-\n  readable contract. Both real scopes below were recovered from the documentation and from the MCP\n  authorization-server metadata, so this file is upgraded to `searched`. Seamless.AI operates two\n  separate OAuth surfaces with two separate authorization servers and two disjoint scope\n  vocabularies; they are not interchangeable.\n\nscope_count: 2\ngranularity:\
  \ coarse\ngranularity_note: >-\n  Both surfaces expose exactly ONE all-or-nothing scope. There is no read/write split, no\n  per-resource scope, and no way to grant an agent search access without also granting enrichment\n  (which spends credits) or, on MCP, campaign and bulk-email send. Least-privilege delegation is\n  not expressible against this API today.\n\nsurfaces:\n  - name: REST Public API v1\n    authorization_server: https://login.seamless.ai\n    authorization_url: https://login.seamless.ai/oauth/authorize\n    token_url: https://api.seamless.ai/api/client/v1/oauth/accessToken\n    flow: authorizationCode\n    client_authentication: client_secret\n    pkce: false\n    dynamic_client_registration: false\n    scopes_in_spec: 0\n    registration: Settings -> Public API -> OAuth Connections, at https://login.seamless.ai/settings/public-api\n  - name: MCP server\n    authorization_server: https://mcp.seamless.ai\n    authorization_url: https://mcp.seamless.ai/mcp/authorize\n   \
  \ token_url: https://mcp.seamless.ai/mcp/token\n    registration_endpoint: https://mcp.seamless.ai/mcp/register\n    revocation_endpoint: https://mcp.seamless.ai/mcp/revoke\n    flow: authorizationCode\n    client_authentication: none\n    pkce: [S256]\n    dynamic_client_registration: true\n\nschemes:\n  - name: OAuth2\n    source: openapi/_original/seamless-ai-public-api-openapi-original.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.seamless.ai/oauth/authorize\n        tokenUrl: https://api.seamless.ai/api/client/v1/oauth/accessToken\n        scopes_declared: 0\n\nscopes:\n  - scope: publicAPI.v1.all\n    surface: rest\n    description: >-\n      Full access to the Seamless.AI Public API v1 — search, research, polling and org-data reads.\n      The only REST scope published.\n    flows: [authorizationCode]\n    sources: [https://docs.seamless.ai/authentication/oauth]\n    in_spec: false\n    enforcement: >-\n      A connection lacking it receives\
  \ HTTP 403 with `code: insufficientScope`. The documented\n      remedy is to re-authorize with this scope.\n  - scope: mcp.all\n    surface: mcp\n    description: Full MCP access — all 54 tools and all seamless:// resources the org is licensed for.\n    flows: [authorizationCode]\n    sources:\n      - https://mcp.seamless.ai/.well-known/oauth-protected-resource\n      - https://mcp.seamless.ai/.well-known/oauth-authorization-server\n    in_spec: true\n    in_spec_source: https://docs.seamless.ai/mcp-openapi.yaml\n    enforcement: >-\n      Advertised as the required scope in the WWW-Authenticate challenge returned by an\n      unauthenticated POST to https://mcp.seamless.ai/mcp (HTTP 401, verified 2026-08-14).\n\nsecondary_authorization:\n  mechanism: license entitlement\n  note: >-\n    Scope is not the only gate. Tool visibility on MCP is filtered per request by the org's\n    license — \"Connect\" for templates/email/calls/activity, \"Connect (full)\" for campaigns and\n    tasks\
  \ — and the REST API requires an active Public API license or returns HTTP 422\n    `missingLicense`. An access token carrying mcp.all still sees a smaller tool list on an\n    unlicensed org, so a client must not assume a fixed tool set.\n  see_also: mcp/seamless-ai-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/scopes/seamless-ai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- B2B
- Contact Data
- Sales Intelligence
- Prospecting
- Lead Generation
- CRM Enrichment
- Data Enrichment
- MCP
- Agents
- Sales Automation
token_urls:
- https://api.seamless.ai/api/client/v1/oauth/accessToken
---
