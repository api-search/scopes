---
authorization_urls:
- https://app.crayon.co/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Crayon Scopes
name_suffix: OAuth Scopes
note: Read from Crayon's RFC 8414 authorization-server metadata, which is served anonymously. Crayon publishes no scopes/permissions reference page, so the metadata is the only scope surface. Note that the RFC 9728 protected-resource document for the MCP endpoint declares an EMPTY scopes_supported array while the authorization server declares mcp:read — the two disagree, and that disagreement is recorded rather than reconciled. The earlier version of this file described the "CustomerApi" scope of Crayon Group ASA's Cloud-iQ platform (crayon.com), a different company; it is quarantined in _wrong-company/.
overview: 'Crayon publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Crayon API on a user''s behalf.


  Tokens are issued from https://app.crayon.co/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Crayon
provider_slug: crayon
schemes:
- flows:
  - authorizationUrl: https://app.crayon.co/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://app.crayon.co/oauth/token/
  name: CrayonOAuth2
  source: well-known/crayon-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: Read access to the Crayon competitive-intelligence MCP server at https://mcp.crayon.co/mcp/. The only scope Crayon's authorization server advertises; no write or admin scope is published.
  flows:
  - authorizationCode
  scope: mcp:read
slug: crayon-scopes
source_filename: crayon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.crayon.co/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Read from Crayon's RFC 8414 authorization-server metadata, which is served anonymously. Crayon\n  publishes no scopes/permissions reference page, so the metadata is the only scope surface. Note\n  that the RFC 9728 protected-resource document for the MCP endpoint declares an EMPTY\n  scopes_supported array while the authorization server declares mcp:read — the two disagree, and\n  that disagreement is recorded rather than reconciled. The earlier version of this file described\n  the \"CustomerApi\" scope of Crayon Group ASA's Cloud-iQ platform (crayon.com), a different\n  company; it is quarantined in _wrong-company/.\n\nschemes:\n- name: CrayonOAuth2\n  source: well-known/crayon-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.crayon.co/oauth/authorize/\n    tokenUrl: https://app.crayon.co/oauth/token/\n\
  \nscopes:\n- scope: mcp:read\n  description: >-\n    Read access to the Crayon competitive-intelligence MCP server at\n    https://mcp.crayon.co/mcp/. The only scope Crayon's authorization server advertises; no\n    write or admin scope is published.\n  flows:\n  - authorizationCode\n  sources:\n  - https://mcp.crayon.co/.well-known/oauth-authorization-server\n  - https://app.crayon.co/.well-known/oauth-authorization-server\n\ndiscrepancies:\n- resource: https://mcp.crayon.co/mcp/\n  document: https://mcp.crayon.co/.well-known/oauth-protected-resource/mcp/\n  issue: scopes_supported is [] on the protected resource but [\"mcp:read\"] on the authorization server\n  observed: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/scopes/crayon-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Competitive Intelligence
- Market Intelligence
- Sales Enablement
- Battlecards
- Win-Loss Analysis
- Product Marketing
- Artificial Intelligence
- MCP
token_urls:
- https://app.crayon.co/oauth/token/
---
