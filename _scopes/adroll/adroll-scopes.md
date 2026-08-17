---
authorization_urls:
- https://services.adroll.com/auth/authorize
- https://services.adroll.com/mcp/auth/authorize
description: ''
docs: https://apidocs.nextroll.com/guides/oauth.html
flows:
- authorizationCode
- implicit
- password
kind: oauth-scopes
layout: scope
method: searched
name: Adroll Scopes
name_suffix: OAuth Scopes
note: Two distinct OAuth authorization surfaces exist and they do not share a scope vocabulary. The platform OAuth server supports exactly one scope; the MCP authorization server (published as RFC 8414 metadata) supports exactly one different scope. Neither is fine-grained. This file was written from the docs and the live metadata document, not derived from an OpenAPI — NextRoll publishes no spec file.
overview: 'AdRoll publishes 2 OAuth 2.0 scopes via the authorizationCode, implicit, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AdRoll API on a user''s behalf.


  Tokens are issued from https://services.adroll.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AdRoll
provider_slug: adroll
schemes:
- applies_to: All NextRoll REST + GraphQL services on https://services.adroll.com
  flows:
  - authorizationUrl: https://services.adroll.com/auth/authorize
    flow: authorizationCode
    tokenUrl: https://services.adroll.com/auth/token
  - authorizationUrl: https://services.adroll.com/auth/authorize
    flow: implicit
  - flow: password
    tokenUrl: https://services.adroll.com/auth/token
  name: platform-oauth2
  source: https://apidocs.nextroll.com/guides/oauth.html
- applies_to: AdRoll MCP Server — https://services.adroll.com/mcp
  flows:
  - authorizationUrl: https://services.adroll.com/mcp/auth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://services.adroll.com/mcp/auth/token
  name: mcp-oauth2
  source: https://services.adroll.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- all
- mcp
scopes:
- description: Gives access to all resources. This is the default when no scope is specified. It is currently the ONLY scope the platform OAuth server offers.
  flows:
  - authorizationCode
  - implicit
  - password
  scope: all
- description: The single scope advertised by the MCP authorization server metadata (scopes_supported) and echoed by the protected-resource metadata for https://services.adroll.com/mcp.
  flows:
  - authorizationCode
  scope: mcp
slug: adroll-scopes
source_filename: adroll-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://apidocs.nextroll.com/guides/oauth.html\ndocs: https://apidocs.nextroll.com/guides/oauth.html\nnote: >-\n  Two distinct OAuth authorization surfaces exist and they do not share a scope\n  vocabulary. The platform OAuth server supports exactly one scope; the MCP\n  authorization server (published as RFC 8414 metadata) supports exactly one\n  different scope. Neither is fine-grained. This file was written from the docs\n  and the live metadata document, not derived from an OpenAPI — NextRoll\n  publishes no spec file.\n\nschemes:\n- name: platform-oauth2\n  source: https://apidocs.nextroll.com/guides/oauth.html\n  applies_to: All NextRoll REST + GraphQL services on https://services.adroll.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://services.adroll.com/auth/authorize\n    tokenUrl: https://services.adroll.com/auth/token\n  - flow: implicit\n    authorizationUrl: https://services.adroll.com/auth/authorize\n\
  \  - flow: password\n    tokenUrl: https://services.adroll.com/auth/token\n\n- name: mcp-oauth2\n  source: https://services.adroll.com/.well-known/oauth-authorization-server\n  applies_to: AdRoll MCP Server — https://services.adroll.com/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://services.adroll.com/mcp/auth/authorize\n    tokenUrl: https://services.adroll.com/mcp/auth/token\n    pkce: [S256]\n\nscopes:\n- scope: all\n  description: >-\n    Gives access to all resources. This is the default when no scope is\n    specified. It is currently the ONLY scope the platform OAuth server offers.\n  flows: [authorizationCode, implicit, password]\n  schemes: [platform-oauth2]\n  sources: ['https://apidocs.nextroll.com/guides/oauth.html']\n- scope: mcp\n  description: >-\n    The single scope advertised by the MCP authorization server metadata\n    (scopes_supported) and echoed by the protected-resource metadata for\n    https://services.adroll.com/mcp.\n  flows: [authorizationCode]\n\
  \  schemes: [mcp-oauth2]\n  sources: ['https://services.adroll.com/.well-known/oauth-authorization-server', 'https://services.adroll.com/.well-known/oauth-protected-resource']\n\ngranularity:\n  fine_grained: false\n  provider_statement: >-\n    \"At this time, we only support a single scope. We plan to implement\n    fine-grained scopes in the future.\"\n  consequence: >-\n    There is no read-only grant. Any application a user authorizes — including an\n    AI agent — receives full access to every resource in the account, so\n    least-privilege delegation is not expressible on this API today.\n\nx-evidence:\n  checked: '2026-08-13'\n  probes:\n  - {url: 'https://apidocs.nextroll.com/guides/oauth.html', http_status: 200}\n  - {url: 'https://services.adroll.com/.well-known/oauth-authorization-server', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adroll/refs/heads/main/scopes/adroll-scopes.yml
summary_line: 2 scopes · authorizationCode/implicit/password
tags:
- Advertising
- Display Advertising
- Retargeting
- Marketing
- AdTech
- Programmatic
token_urls:
- https://services.adroll.com/auth/token
- https://services.adroll.com/mcp/auth/token
---
