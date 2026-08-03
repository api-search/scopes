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
name: Nextroll Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NextRoll publishes 2 OAuth 2.0 scopes via the authorizationCode, implicit, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the NextRoll API on a user''s behalf.


  Tokens are issued from https://services.adroll.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NextRoll
provider_slug: nextroll
schemes:
- conforms:
  - RFC 6749
  - RFC 6750
  flows:
  - authorizationUrl: https://services.adroll.com/auth/authorize
    flow: authorizationCode
    tokenUrl: https://services.adroll.com/auth/token
  - authorizationUrl: https://services.adroll.com/auth/authorize
    flow: implicit
  - flow: password
    tokenUrl: https://services.adroll.com/auth/token
  name: nextroll_developer_oauth
  source: https://apidocs.nextroll.com/guides/oauth.html
- conforms:
  - RFC 8414
  - RFC 9728
  - OAuth 2.1
  flows:
  - authorizationUrl: https://services.adroll.com/mcp/auth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://services.adroll.com/mcp/auth/token
  name: adroll_mcp_oauth
  source: well-known/nextroll-oauth-authorization-server.json
scope_count: 2
scope_names:
- all
- mcp
scopes:
- description: Gives access to all resources. The default if no scope is specified.
  flows: []
  scope: all
- description: The single scope advertised by the AdRoll MCP Server authorization server metadata; grants an MCP client access to the tools and data the authenticated AdRoll user is permitted to reach.
  flows: []
  scope: mcp
slug: nextroll-scopes
source_filename: nextroll-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://apidocs.nextroll.com/guides/oauth.html\ndocs: https://apidocs.nextroll.com/guides/oauth.html\nderived_from_openapi: false\nschemes:\n- name: nextroll_developer_oauth\n  source: https://apidocs.nextroll.com/guides/oauth.html\n  conforms: [RFC 6749, RFC 6750]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://services.adroll.com/auth/authorize\n    tokenUrl: https://services.adroll.com/auth/token\n  - flow: implicit\n    authorizationUrl: https://services.adroll.com/auth/authorize\n  - flow: password\n    tokenUrl: https://services.adroll.com/auth/token\n- name: adroll_mcp_oauth\n  source: well-known/nextroll-oauth-authorization-server.json\n  conforms: [RFC 8414, RFC 9728, OAuth 2.1]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://services.adroll.com/mcp/auth/authorize\n    tokenUrl: https://services.adroll.com/mcp/auth/token\n    code_challenge_methods: [S256]\nscopes:\n- scope:\
  \ all\n  description: Gives access to all resources. The default if no scope is specified.\n  schemes: [nextroll_developer_oauth]\n  sources: [https://apidocs.nextroll.com/guides/oauth.html]\n- scope: mcp\n  description: The single scope advertised by the AdRoll MCP Server authorization\n    server metadata; grants an MCP client access to the tools and data the\n    authenticated AdRoll user is permitted to reach.\n  schemes: [adroll_mcp_oauth]\n  sources: [https://services.adroll.com/.well-known/oauth-authorization-server]\ncoverage:\n  scope_count: 2\n  granularity: coarse\n  note: >-\n    Two coarse, all-or-nothing scopes across two separate OAuth deployments. NextRoll\n    states in its own OAuth guide that fine-grained scopes are planned but not yet\n    implemented, so there is no read-only, per-service or per-object scope available\n    to a delegated application or an AI agent today. Authorization granularity is\n    instead enforced by the AdRoll user's account permissions behind\
  \ the token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextroll/refs/heads/main/scopes/nextroll-scopes.yml
summary_line: 2 scopes · authorizationCode/implicit/password
tags:
- Company
- Advertising
- AdTech
- Marketing
- Account Based Marketing
- Retargeting
- Audiences
- Campaign Management
- Analytics
- Reporting
- MarTech
- Agents
token_urls:
- https://services.adroll.com/auth/token
- https://services.adroll.com/mcp/auth/token
---
