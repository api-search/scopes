---
api_specs:
- filename: appcharge-openapi.yml
  format: yaml
  label: Appcharge Publisher API
  slug: appcharge-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-openapi.yml
authorization_urls:
- https://api.appcharge.com/oauth/authorize
description: 'OAuth 2.0 scopes published by Appcharge''s authorization server (RFC 8414). These scopes gate the hosted MCP server (mcp.appcharge.com); the publisher REST API itself authenticates with the x-publisher-token API key (see authentication/). Flow: authorization_code with PKCE (S256) and dynamic client registration; token_endpoint_auth_methods_supported = [none] (public clients).'
docs: https://mcp.appcharge.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Appcharge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Appcharge publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Appcharge API on a user''s behalf.


  Tokens are issued from https://api.appcharge.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Appcharge
provider_slug: appcharge
schemes:
- flows:
  - authorizationUrl: https://api.appcharge.com/oauth/authorize
    flow: authorizationCode
    jwksUri: https://api.appcharge.com/.well-known/jwks-oauth.json
    pkce:
    - S256
    registrationUrl: https://api.appcharge.com/oauth/register
    tokenUrl: https://api.appcharge.com/oauth/token
  issuer: https://api.appcharge.com
  name: OAuth2
  source: https://api.appcharge.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access via the Appcharge MCP server.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access via the Appcharge MCP server.
  flows:
  - authorizationCode
  scope: mcp:write
slug: appcharge-scopes
source_filename: appcharge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://api.appcharge.com/.well-known/oauth-authorization-server\ndocs: https://mcp.appcharge.com/.well-known/oauth-protected-resource\ndescription: >-\n  OAuth 2.0 scopes published by Appcharge's authorization server (RFC 8414).\n  These scopes gate the hosted MCP server (mcp.appcharge.com); the publisher\n  REST API itself authenticates with the x-publisher-token API key (see\n  authentication/). Flow: authorization_code with PKCE (S256) and dynamic\n  client registration; token_endpoint_auth_methods_supported = [none] (public\n  clients).\nschemes:\n  - name: OAuth2\n    source: https://api.appcharge.com/.well-known/oauth-authorization-server\n    issuer: https://api.appcharge.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.appcharge.com/oauth/authorize\n        tokenUrl: https://api.appcharge.com/oauth/token\n        registrationUrl: https://api.appcharge.com/oauth/register\n    \
  \    jwksUri: https://api.appcharge.com/.well-known/jwks-oauth.json\n        pkce: [S256]\nscopes:\n  - scope: mcp:read\n    description: Read access via the Appcharge MCP server.\n    flows: [authorizationCode]\n    sources: [https://api.appcharge.com/.well-known/oauth-authorization-server]\n  - scope: mcp:write\n    description: Write access via the Appcharge MCP server.\n    flows: [authorizationCode]\n    sources: [https://api.appcharge.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/scopes/appcharge-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Payments
- Monetization
- Merchant of Record
- Mobile Games
- Gaming
- Checkout
- In-Game Purchases
- Web Store
- eCommerce
token_urls:
- https://api.appcharge.com/oauth/token
---
