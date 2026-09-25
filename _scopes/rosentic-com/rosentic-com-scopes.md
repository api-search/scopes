---
authorization_urls:
- https://api.rosentic.com/oauth/authorize
description: ''
docs:
- https://rosentic.com/mcp/
- well-known/rosentic-com-oauth-authorization-server.json
- well-known/rosentic-com-oauth-protected-resource.json
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Rosentic Com Scopes
name_suffix: OAuth Scopes
note: No OpenAPI declares an oauth2 scheme, so derive-oauth-scopes.py has nothing to read; this file is written from the provider's live RFC 8414 and RFC 9728 discovery documents on api.rosentic.com and the 401 challenge the MCP endpoint returns. Exactly one scope is published, for one resource. The provider's human docs do not publish a scopes reference page.
overview: 'Rosentic publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rosentic API on a user''s behalf.


  Tokens are issued from https://api.rosentic.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rosentic
provider_slug: rosentic-com
schemes:
- dcr_probe:
    body: '{}'
    fetched: '2026-09-19'
    http_status: 400
    method: POST
    note: RFC 7591-shaped error for an empty registration request; no client was registered. GET returns 405 method not allowed.
    response: '{"error":"invalid_client_metadata","error_description":"redirect_uris must contain 1 to 10 HTTPS or loopback HTTP URIs without fragments"}'
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://api.rosentic.com/oauth/authorize
    client_type: public (token_endpoint_auth_methods_supported [none])
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256 (code_challenge_methods_supported)
    refreshUrl: https://api.rosentic.com/oauth/token
    response_types:
    - code
    tokenUrl: https://api.rosentic.com/oauth/token
  issuer: https://api.rosentic.com
  name: Rosentic Remote OAuth 2.1
  protected_resources:
  - https://api.rosentic.com/mcp
  registration_endpoint: https://api.rosentic.com/oauth/register
  source: well-known/rosentic-com-oauth-authorization-server.json
  type: oauth2
scope_count: 1
scope_names:
- rosentic:remote:read
scopes:
- description: Read access to Rosentic Remote — the hosted MCP tools run_status, which_lane and get_verdict, which answer from stored scan snapshots scoped to the caller's workspace. The only scope the authorization server advertises and the scope the MCP endpoint's WWW-Authenticate challenge demands.
  flows:
  - authorizationCode
  scope: rosentic:remote:read
slug: rosentic-com-scopes
source_filename: rosentic-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.rosentic.com/.well-known/oauth-authorization-server\ndocs:\n- https://rosentic.com/mcp/\n- well-known/rosentic-com-oauth-authorization-server.json\n- well-known/rosentic-com-oauth-protected-resource.json\nnote: >-\n  No OpenAPI declares an oauth2 scheme, so derive-oauth-scopes.py has nothing to read; this file is written\n  from the provider's live RFC 8414 and RFC 9728 discovery documents on api.rosentic.com and the 401\n  challenge the MCP endpoint returns. Exactly one scope is published, for one resource. The provider's\n  human docs do not publish a scopes reference page.\nschemes:\n- name: Rosentic Remote OAuth 2.1\n  type: oauth2\n  source: well-known/rosentic-com-oauth-authorization-server.json\n  issuer: https://api.rosentic.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.rosentic.com/oauth/authorize\n    tokenUrl: https://api.rosentic.com/oauth/token\n    refreshUrl: https://api.rosentic.com/oauth/token\n\
  \    pkce: S256 (code_challenge_methods_supported)\n    client_type: public (token_endpoint_auth_methods_supported [none])\n    grant_types: [authorization_code, refresh_token]\n    response_types: [code]\n  registration_endpoint: https://api.rosentic.com/oauth/register\n  dynamic_client_registration: true\n  dcr_probe:\n    fetched: '2026-09-19'\n    method: POST\n    body: '{}'\n    http_status: 400\n    response: '{\"error\":\"invalid_client_metadata\",\"error_description\":\"redirect_uris must contain 1 to 10 HTTPS or loopback HTTP URIs without fragments\"}'\n    note: RFC 7591-shaped error for an empty registration request; no client was registered. GET returns 405 method not allowed.\n  protected_resources: [https://api.rosentic.com/mcp]\nscopes:\n- scope: rosentic:remote:read\n  description: >-\n    Read access to Rosentic Remote — the hosted MCP tools run_status, which_lane and get_verdict, which answer\n    from stored scan snapshots scoped to the caller's workspace. The only\
  \ scope the authorization server\n    advertises and the scope the MCP endpoint's WWW-Authenticate challenge demands.\n  resource: https://api.rosentic.com/mcp\n  flows: [authorizationCode]\n  sources: [well-known/rosentic-com-oauth-authorization-server.json, well-known/rosentic-com-oauth-protected-resource.json, 'MCP 401 WWW-Authenticate: Bearer resource_metadata=\"https://api.rosentic.com/.well-known/oauth-protected-resource/mcp\", scope=\"rosentic:remote:read\"']\n  write_scope: none published — the remote surface is read-only\ngithub_oauth_delegation:\n  note: >-\n    Dashboard sign-in (https://api.rosentic.com/auth/github) is a separate GitHub OAuth app requesting\n    read:org read:user user:email (observed in the 302 Location); those are GitHub's scopes, not Rosentic's,\n    and are recorded in authentication/rosentic-com-authentication.yml rather than here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rosentic-com/refs/heads/main/scopes/rosentic-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Developer Tools
- CI/CD
- Git
- Static Analysis
- Merge Safety
- AI Coding Agents
- MCP
- A2A
- GitHub Actions
- Agent-Native
token_urls:
- https://api.rosentic.com/oauth/token
---
