---
authorization_urls:
- https://klarys.app/api/public/o/authorize/
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Klarys Scopes
name_suffix: OAuth Scopes
note: Klarys publishes its OAuth 2.0 scope list anonymously in the RFC 8414 authorization-server metadata document, but publishes no scopes/permissions reference page, so descriptions below are recorded as unpublished rather than guessed. Six scopes are advertised. Two of them — mcp:read and mcp:write — are the only public evidence that Klarys operates a Model Context Protocol surface; no MCP endpoint was reachable anonymously (see mcp/klarys-mcp.yml).
overview: 'Klarys publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Klarys API on a user''s behalf.


  Tokens are issued from https://klarys.app/api/public/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Klarys
provider_slug: klarys
schemes:
- flows:
  - authorizationUrl: https://klarys.app/api/public/o/authorize/
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://klarys.app/api/public/o/token/
  - flow: clientCredentials
    tokenUrl: https://klarys.app/api/public/o/token/
  issuer: https://klarys.app/api/public/o
  name: OAuth2
  source: well-known/klarys-oauth-authorization-server.json
scope_count: 6
scope_names:
- read
- write
- groups
- introspection
- mcp:read
- mcp:write
scopes:
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: write
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: groups
- description: ''
  flows:
  - clientCredentials
  scope: introspection
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:write
slug: klarys-scopes
source_filename: klarys-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://klarys.app/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Klarys publishes its OAuth 2.0 scope list anonymously in the RFC 8414 authorization-server metadata\n  document, but publishes no scopes/permissions reference page, so descriptions below are recorded as\n  unpublished rather than guessed. Six scopes are advertised. Two of them — mcp:read and mcp:write — are\n  the only public evidence that Klarys operates a Model Context Protocol surface; no MCP endpoint was\n  reachable anonymously (see mcp/klarys-mcp.yml).\nschemes:\n- name: OAuth2\n  source: well-known/klarys-oauth-authorization-server.json\n  issuer: https://klarys.app/api/public/o\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://klarys.app/api/public/o/authorize/\n    tokenUrl: https://klarys.app/api/public/o/token/\n    code_challenge_methods:\n    - S256\n  - flow: clientCredentials\n    tokenUrl: https://klarys.app/api/public/o/token/\n\
  scopes:\n- scope: read\n  description: null\n  description_published: false\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - well-known/klarys-oauth-authorization-server.json\n- scope: write\n  description: null\n  description_published: false\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - well-known/klarys-oauth-authorization-server.json\n- scope: groups\n  description: null\n  description_published: false\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - well-known/klarys-oauth-authorization-server.json\n- scope: introspection\n  description: null\n  description_published: false\n  note: >-\n    Django OAuth Toolkit convention — grants a client the right to call the token introspection endpoint\n    at https://klarys.app/api/public/o/introspect/.\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/klarys-oauth-authorization-server.json\n- scope: mcp:read\n  description: null\n  description_published: false\n\
  \  note: Read scope for a Model Context Protocol surface; no MCP endpoint is anonymously discoverable.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - well-known/klarys-oauth-authorization-server.json\n- scope: mcp:write\n  description: null\n  description_published: false\n  note: Write scope for a Model Context Protocol surface; no MCP endpoint is anonymously discoverable.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - well-known/klarys-oauth-authorization-server.json\nsummary:\n  scope_count: 6\n  descriptions_published: 0\n  mcp_scopes: 2\ngaps:\n- No scopes/permissions reference page is published, so no scope carries a documented meaning.\n- The metadata does not bind scopes to individual flows; the flow lists above reflect the grant types\n  the server advertises, not a per-scope restriction Klarys publishes.\nx-evidence:\n  fetched: '2026-08-17'\n  url: https://klarys.app/.well-known/oauth-authorization-server\n  http_status: 200\n\
  \  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarys/refs/heads/main/scopes/klarys-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Company
- SaaS
- eProcurement
- Procurement
- Supply Chain
- Food and Beverage
- Seafood
- Fresh Food
- Retail
- EDI
- Invoicing
- France
token_urls:
- https://klarys.app/api/public/o/token/
---
