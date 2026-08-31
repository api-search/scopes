---
authorization_urls:
- https://api.descope.com/oauth2/v1/apps/authorize
description: ''
docs: https://result.dev/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Result Scopes
name_suffix: OAuth Scopes
note: 'Result declares exactly one OAuth scope. Both the RFC 9728 protected-resource metadata for the MCP server and the RFC 8414 authorization-server metadata it delegates to publish scopes_supported: ["full-access"] and nothing else. There is no scope-reference or permissions page in the documentation, and no finer-grained scope exists to enrich this with — that coarseness IS the finding, and it is recorded rather than padded. Result''s own /mcp page describes the compensating controls in prose: authorization grants read and write, every call re-checks that the business belongs to the authenticated account, and sensitive actions (publishing, filing, outreach) are pushed to a client-side approval prompt rather than being separated by scope. 0-working/derive-oauth-scopes.py was not the source here — it reads OpenAPI oauth2 securitySchemes, and Result publishes no OpenAPI.'
overview: 'Result publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Result API on a user''s behalf.


  Tokens are issued from https://api.descope.com/oauth2/v1/apps/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Result
provider_slug: result
schemes:
- authorization_server: https://api.descope.com/v1/apps/P3HVe6On8gLt3t2puHvHToMFQit2
  flows:
  - authorizationUrl: https://api.descope.com/oauth2/v1/apps/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://api.descope.com/oauth2/v1/apps/token
  name: result-mcp-oauth
  resource: https://api.result.dev/mcp
  source: https://api.result.dev/.well-known/oauth-protected-resource
scope_count: 1
scope_names:
- full-access
scopes:
- description: Read and write access to the Result businesses owned by the authenticated account, across all 74 MCP tools. The only scope Result publishes.
  flows:
  - authorizationCode
  scope: full-access
slug: result-scopes
source_filename: result-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.result.dev/.well-known/oauth-protected-resource\ndocs: https://result.dev/mcp\nnote: >-\n  Result declares exactly one OAuth scope. Both the RFC 9728 protected-resource metadata for\n  the MCP server and the RFC 8414 authorization-server metadata it delegates to publish\n  scopes_supported: [\"full-access\"] and nothing else. There is no scope-reference or\n  permissions page in the documentation, and no finer-grained scope exists to enrich this\n  with — that coarseness IS the finding, and it is recorded rather than padded. Result's\n  own /mcp page describes the compensating controls in prose: authorization grants read and\n  write, every call re-checks that the business belongs to the authenticated account, and\n  sensitive actions (publishing, filing, outreach) are pushed to a client-side approval\n  prompt rather than being separated by scope.\n  0-working/derive-oauth-scopes.py was not the source here — it reads\
  \ OpenAPI oauth2\n  securitySchemes, and Result publishes no OpenAPI.\nschemes:\n- name: result-mcp-oauth\n  source: https://api.result.dev/.well-known/oauth-protected-resource\n  resource: https://api.result.dev/mcp\n  authorization_server: https://api.descope.com/v1/apps/P3HVe6On8gLt3t2puHvHToMFQit2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.descope.com/oauth2/v1/apps/authorize\n    tokenUrl: https://api.descope.com/oauth2/v1/apps/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: full-access\n  description: >-\n    Read and write access to the Result businesses owned by the authenticated account,\n    across all 74 MCP tools. The only scope Result publishes.\n  flows: [authorizationCode]\n  sources:\n  - well-known/result-oauth-protected-resource.json\n  - well-known/result-oauth-authorization-server.json\nclaims_supported:\n- iss\n- aud\n- iat\n- exp\n- sub\n- name\n- email\n- email_verified\n- phone_number\n- phone_number_verified\n- picture\n\
  - family_name\n- given_name\nassessment:\n  granularity: single-scope\n  least_privilege: false\n  note: >-\n    An agent connecting to the Result MCP server cannot be granted anything narrower than\n    full read-write access to every business on the account. There is no read-only grant, no\n    per-category scope matching the six published tool categories, and no per-business\n    scope. Delegation is all-or-nothing at the token layer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/result/refs/heads/main/scopes/result-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Business Operations
- Software-as-a-Service
- Entrepreneurship
- Payments
- Marketing
- No-Code
- Startups
- Artificial Intelligence
- Backend as a Service
- MCP
- Agents
- Database
- Authentication
- Storage
- Serverless
- Real-Time
token_urls:
- https://api.descope.com/oauth2/v1/apps/token
---
