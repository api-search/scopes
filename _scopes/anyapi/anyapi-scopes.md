---
api_specs:
- filename: anyapi-gateway-openapi.json
  format: json
  label: AnyAPI Gateway API
  slug: anyapi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anyapi/refs/heads/main/openapi/anyapi-gateway-openapi.json
authorization_urls:
- https://api.getanyapi.com/oauth/authorize
description: ''
docs: https://getanyapi.com/docs/mcp-server
flows:
- authorizationCode
- refreshToken
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Anyapi Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only apiKey and http-bearer security schemes, so derive-oauth-scopes.py correctly found nothing there. The OAuth surface is real but lives OUTSIDE the spec, in the RFC 8414 authorization-server metadata served at the API host, and it is what an MCP client actually authenticates against. Both scopes below are read verbatim from that document's scopes_supported, and are corroborated by the RFC 9728 protected-resource document and by the WWW-Authenticate challenge the MCP endpoint returns (scope="run balance:read").
overview: 'AnyAPI publishes 2 OAuth 2.0 scopes via the authorizationCode, refreshToken, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AnyAPI API on a user''s behalf.


  Tokens are issued from https://api.getanyapi.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AnyAPI
provider_slug: anyapi
schemes:
- code_challenge_methods_supported:
  - S256
  dynamic_client_registration: https://api.getanyapi.com/oauth/register
  flows:
  - authorizationUrl: https://api.getanyapi.com/oauth/authorize
    flow: authorizationCode
    pkce_required: true
    tokenUrl: https://api.getanyapi.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://api.getanyapi.com/oauth/token
  - deviceAuthorizationUrl: https://api.getanyapi.com/oauth/device_authorization
    flow: deviceCode
    grant_type: urn:ietf:params:oauth:grant-type:device_code
    rfc: RFC 8628
  issuer: https://api.getanyapi.com
  name: OAuth2
  response_types_supported:
  - code
  revocation_endpoint: https://api.getanyapi.com/oauth/revoke
  source: https://api.getanyapi.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
scope_count: 2
scope_names:
- run
- balance:read
scopes:
- description: Execute APIs - the run_api tool and POST /v1/run/{sku}. This is the spending scope; a grant carries the spending limit its owner approved, and exceeding it returns the grant_cap_exceeded error.
  flows:
  - authorizationCode
  - deviceCode
  scope: run
- description: Read the remaining USD wallet balance - the get_balance tool and GET /v1/balance.
  flows:
  - authorizationCode
  - deviceCode
  scope: balance:read
slug: anyapi-scopes
source_filename: anyapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://api.getanyapi.com/.well-known/oauth-authorization-server\ndocs: https://getanyapi.com/docs/mcp-server\nnote: >-\n  The OpenAPI declares only apiKey and http-bearer security schemes, so derive-oauth-scopes.py\n  correctly found nothing there. The OAuth surface is real but lives OUTSIDE the spec, in the\n  RFC 8414 authorization-server metadata served at the API host, and it is what an MCP client\n  actually authenticates against. Both scopes below are read verbatim from that document's\n  scopes_supported, and are corroborated by the RFC 9728 protected-resource document and by the\n  WWW-Authenticate challenge the MCP endpoint returns (scope=\"run balance:read\").\nschemes:\n  - name: OAuth2\n    source: https://api.getanyapi.com/.well-known/oauth-authorization-server\n    issuer: https://api.getanyapi.com\n    dynamic_client_registration: https://api.getanyapi.com/oauth/register\n    token_endpoint_auth_methods_supported:\
  \ [none]\n    code_challenge_methods_supported: [S256]\n    response_types_supported: [code]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.getanyapi.com/oauth/authorize\n        tokenUrl: https://api.getanyapi.com/oauth/token\n        pkce_required: true\n      - flow: refreshToken\n        tokenUrl: https://api.getanyapi.com/oauth/token\n      - flow: deviceCode\n        grant_type: 'urn:ietf:params:oauth:grant-type:device_code'\n        deviceAuthorizationUrl: https://api.getanyapi.com/oauth/device_authorization\n        rfc: RFC 8628\n    revocation_endpoint: https://api.getanyapi.com/oauth/revoke\nprotected_resources:\n  - resource: https://api.getanyapi.com/mcp\n    authorization_servers: [https://api.getanyapi.com]\n    scopes_supported: [run, balance:read]\n    source: https://api.getanyapi.com/.well-known/oauth-protected-resource\n    rfc: RFC 9728\nscopes:\n  - scope: run\n    description: >-\n      Execute APIs - the run_api tool and POST\
  \ /v1/run/{sku}. This is the spending scope; a\n      grant carries the spending limit its owner approved, and exceeding it returns the\n      grant_cap_exceeded error.\n    flows: [authorizationCode, deviceCode]\n    sources: [/.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource]\n  - scope: balance:read\n    description: Read the remaining USD wallet balance - the get_balance tool and GET /v1/balance.\n    flows: [authorizationCode, deviceCode]\n    sources: [/.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource]\nobservations:\n  - >-\n    Only two scopes, and they split exactly along the line that matters to an agent's owner:\n    spending money versus reading how much is left. Discovery (list/search/describe/quote)\n    needs no scope at all and no credential - those paths are anonymous.\n  - >-\n    token_endpoint_auth_methods_supported is [\"none\"] with dynamic client registration open,\n    which is the MCP-client profile: a public\
  \ client registers itself and authenticates the\n    user with PKCE rather than holding a client secret.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyapi/refs/heads/main/scopes/anyapi-scopes.yml
summary_line: 2 scopes · authorizationCode/refreshToken/deviceCode
tags:
- developer_tools
- data
- search
- scraping
- social_media
- ecommerce
- seo
- enrichment
- mcp
- agent-native
- web-data
- api-marketplace
- agent-payments
- x402
token_urls:
- https://api.getanyapi.com/oauth/token
---
