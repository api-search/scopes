---
api_specs:
- filename: amuncore-dynamic-api-openapi.yml
  format: yaml
  label: AmunCore API
  slug: amuncore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/openapi/amuncore-dynamic-api-openapi.yml
authorization_urls:
- https://amuncore.com/oauth/authorize
description: AmunCore's OAuth surface exists solely to authorize the MCP endpoint. The RFC 8414 authorization server metadata declares exactly one scope — "mcp" — and the RFC 9728 protected resource metadata confirms it applies to https://amuncore.com/mcp. The REST API itself does not use OAuth at all; it is authenticated with an X-Api-Key header, so there is no scope surface on the REST side and none is invented here.
docs: https://amuncore.com/llms.txt
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Amuncore Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AmunCore publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AmunCore API on a user''s behalf.


  Tokens are issued from https://amuncore.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AmunCore
provider_slug: amuncore
schemes:
- flows:
  - authorizationUrl: https://amuncore.com/oauth/authorize
    flow: authorizationCode
    note: PKCE with S256 is the only code challenge method advertised.
    pkce: S256
    tokenUrl: https://amuncore.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://amuncore.com
  name: OAuth 2.0 (MCP authorization)
  registration_endpoint: https://amuncore.com/oauth/register
  registration_spec: RFC 7591 dynamic client registration
  source: https://amuncore.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to the AmunCore MCP endpoint at https://amuncore.com/mcp. AmunCore publishes no finer-grained scope decomposition; authorization is coarse at the protocol boundary and the actual data a caller can reach is bounded by the API key / company tenancy behind the token rather than by scope.
  flows:
  - authorizationCode
  scope: mcp
slug: amuncore-scopes
source_filename: amuncore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: https://amuncore.com/.well-known/oauth-authorization-server\ndocs: https://amuncore.com/llms.txt\ndescription: >-\n  AmunCore's OAuth surface exists solely to authorize the MCP endpoint. The\n  RFC 8414 authorization server metadata declares exactly one scope — \"mcp\" —\n  and the RFC 9728 protected resource metadata confirms it applies to\n  https://amuncore.com/mcp. The REST API itself does not use OAuth at all; it is\n  authenticated with an X-Api-Key header, so there is no scope surface on the\n  REST side and none is invented here.\nschemes:\n- name: OAuth 2.0 (MCP authorization)\n  source: https://amuncore.com/.well-known/oauth-authorization-server\n  issuer: https://amuncore.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://amuncore.com/oauth/authorize\n    tokenUrl: https://amuncore.com/oauth/token\n    pkce: S256\n    note: PKCE with S256 is the only code challenge method advertised.\n  grant_types:\
  \ [authorization_code, refresh_token]\n  registration_endpoint: https://amuncore.com/oauth/register\n  registration_spec: RFC 7591 dynamic client registration\n  token_endpoint_auth_methods: [none, client_secret_post]\nscopes:\n- scope: mcp\n  description: >-\n    Access to the AmunCore MCP endpoint at https://amuncore.com/mcp. AmunCore\n    publishes no finer-grained scope decomposition; authorization is coarse at\n    the protocol boundary and the actual data a caller can reach is bounded by\n    the API key / company tenancy behind the token rather than by scope.\n  flows: [authorizationCode]\n  resource: https://amuncore.com/mcp\n  sources: ['https://amuncore.com/.well-known/oauth-authorization-server']\ncoverage:\n  scopes_declared: 1\n  rest_api_uses_oauth: false\ngaps:\n- Single coarse scope. There is no read-only vs read-write split at the OAuth\n  layer, so an agent token cannot be narrowed below \"everything this company's\n  key can reach\". Per-endpoint and read-only keys exist\
  \ on the REST side\n  (scoped API keys) but are not projected into OAuth scopes.\n- No openid-configuration, so this is plain OAuth 2.0 authorization rather than\n  OpenID Connect; there is no identity token for the acting agent.\nevidence:\n- url: https://amuncore.com/.well-known/oauth-authorization-server\n  status: 200\n- url: https://amuncore.com/.well-known/oauth-protected-resource\n  status: 200\n- url: https://amuncore.com/mcp\n  status: 401\n  method: POST\n  note: >-\n    Returns WWW-Authenticate: Bearer\n    resource_metadata=\"https://amuncore.com/.well-known/oauth-protected-resource\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/scopes/amuncore-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Database
- API Management
- Backend
- No Code
- SQL
- PostgreSQL
- MySQL
- Oracle
- MCP
- Agents
- Data
- SQL Server
- Webhooks
- OpenAPI
- Low Code
- Egypt
token_urls:
- https://amuncore.com/oauth/token
---
