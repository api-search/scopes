---
api_specs:
- filename: gumloop-openapi-original.yml
  format: yaml
  label: Gumloop Public API
  slug: gumloop-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-openapi-original.yml
authorization_urls:
- https://api.gumloop.com/oauth/authorize
description: ''
docs: https://docs.gumloop.com/api-reference/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Gumloop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gumloop publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gumloop API on a user''s behalf.


  Tokens are issued from https://api.gumloop.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gumloop
provider_slug: gumloop
schemes:
- flows:
  - authorizationUrl: https://api.gumloop.com/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://api.gumloop.com/oauth/revoke
    tokenUrl: https://api.gumloop.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: OAuth2
  pkce: S256 (required)
  registration: invite-only (email support@gumloop.com for a client_id)
  source: https://api.gumloop.com/.well-known/oauth-authorization-server
scope_count: 5
scope_names:
- gumloop_api
- userinfo
- gumloop_api.mcp
- gumstack
- gumloop_university
scopes:
- description: Call the Gumloop developer API on behalf of the user. Requires the user to be on the Pro plan or higher.
  flows:
  - authorizationCode
  scope: gumloop_api
- description: Read the user's basic profile (email, name).
  flows:
  - authorizationCode
  scope: userinfo
- description: Access the Gumloop API's MCP surface on behalf of the user.
  flows:
  - authorizationCode
  scope: gumloop_api.mcp
- description: Access user-deployed Gumstack MCP servers.
  flows:
  - authorizationCode
  scope: gumstack
- description: Access Gumloop University resources.
  flows:
  - authorizationCode
  scope: gumloop_university
slug: gumloop-scopes
source_filename: gumloop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.gumloop.com/.well-known/oauth-authorization-server\ndocs: https://docs.gumloop.com/api-reference/oauth\nschemes:\n- name: OAuth2\n  source: https://api.gumloop.com/.well-known/oauth-authorization-server\n  grant_types: [authorization_code, refresh_token]\n  pkce: S256 (required)\n  registration: invite-only (email support@gumloop.com for a client_id)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.gumloop.com/oauth/authorize\n    tokenUrl: https://api.gumloop.com/oauth/token\n    revocationUrl: https://api.gumloop.com/oauth/revoke\nscopes:\n- scope: gumloop_api\n  description: Call the Gumloop developer API on behalf of the user. Requires the user to be on the Pro plan or higher.\n  flows: [authorizationCode]\n  sources: [https://docs.gumloop.com/api-reference/oauth]\n- scope: userinfo\n  description: Read the user's basic profile (email, name).\n  flows: [authorizationCode]\n  sources:\
  \ [https://docs.gumloop.com/api-reference/oauth]\n- scope: gumloop_api.mcp\n  description: Access the Gumloop API's MCP surface on behalf of the user.\n  flows: [authorizationCode]\n  sources: [https://api.gumloop.com/.well-known/oauth-authorization-server]\n- scope: gumstack\n  description: Access user-deployed Gumstack MCP servers.\n  flows: [authorizationCode]\n  sources: [https://api.gumloop.com/.well-known/oauth-authorization-server]\n- scope: gumloop_university\n  description: Access Gumloop University resources.\n  flows: [authorizationCode]\n  sources: [https://api.gumloop.com/.well-known/oauth-authorization-server]\nnotes: >\n  The public OpenAPI declares only a bearerAuth (http bearer) scheme, but the API\n  host publishes a full OAuth 2.0 authorization server. Scopes gumloop_api and\n  userinfo are described in the docs; gumstack, gumloop_api.mcp and gumloop_university\n  are advertised in the RFC 8414 metadata. token_endpoint_auth_method is `none`\n  (public clients with PKCE).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/scopes/gumloop-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- Workflow Automation
- Agent Platform
- MCP
- LLM
- No-Code
- Developer Tools
token_urls:
- https://api.gumloop.com/oauth/token
---
