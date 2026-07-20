---
api_specs:
- filename: linqalpha-openapi-original.json
  format: json
  label: LinqAlpha API
  slug: linqalpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linqalpha/refs/heads/main/openapi/linqalpha-openapi-original.json
authorization_urls:
- https://api.linqalpha.com/oauth/authorize
description: ''
docs: https://docs.linqalpha.com/api-reference/basic/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Linqalpha Scopes
name_suffix: OAuth Scopes
note: The published OpenAPI declares only the ApiKeyAuth (X-API-KEY) scheme, so no scopes are derivable from the spec. The OAuth surface is discovered instead from RFC 8414 authorization server metadata at api.linqalpha.com, which fronts the LinqAlpha MCP server.
overview: 'LinqAlpha publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LinqAlpha API on a user''s behalf.


  Tokens are issued from https://api.linqalpha.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LinqAlpha
provider_slug: linqalpha
schemes:
- code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://api.linqalpha.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.linqalpha.com/oauth/token
  issuer: https://api.linqalpha.com
  name: LinqAlphaOAuth
  registration_endpoint: https://api.linqalpha.com/oauth/register
  source: https://api.linqalpha.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Invoke the tools exposed by the LinqAlpha MCP server at https://api.linqalpha.com/v1/mcp. This is the only scope advertised in scopes_supported.
  flows:
  - authorizationCode
  scope: mcp:tools
slug: linqalpha-scopes
source_filename: linqalpha-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.linqalpha.com/.well-known/oauth-authorization-server\ndocs: https://docs.linqalpha.com/api-reference/basic/mcp\nnote: >-\n  The published OpenAPI declares only the ApiKeyAuth (X-API-KEY) scheme, so no scopes are derivable\n  from the spec. The OAuth surface is discovered instead from RFC 8414 authorization server metadata\n  at api.linqalpha.com, which fronts the LinqAlpha MCP server.\nschemes:\n- name: LinqAlphaOAuth\n  type: oauth2\n  source: https://api.linqalpha.com/.well-known/oauth-authorization-server\n  issuer: https://api.linqalpha.com\n  registration_endpoint: https://api.linqalpha.com/oauth/register\n  dynamic_client_registration: true\n  token_endpoint_auth_methods_supported:\n  - none\n  code_challenge_methods_supported:\n  - S256\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.linqalpha.com/oauth/authorize\n    tokenUrl: https://api.linqalpha.com/oauth/token\nscopes:\n- scope:\
  \ mcp:tools\n  description: >-\n    Invoke the tools exposed by the LinqAlpha MCP server at https://api.linqalpha.com/v1/mcp.\n    This is the only scope advertised in scopes_supported.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.linqalpha.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linqalpha/refs/heads/main/scopes/linqalpha-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Financial Services
- Investment Research
- Artificial Intelligence
- Agents
- Market Data
- Equities
- Economic Data
- SEC Filings
- Retrieval Augmented Generation
- MCP
token_urls:
- https://api.linqalpha.com/oauth/token
---
