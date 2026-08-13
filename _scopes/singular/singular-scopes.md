---
authorization_urls:
- https://mcp.singular.net/oauth_server/authorize
- https://www.singular.net/oauth/authorize
description: ''
docs: https://support.singular.net/hc/en-us/articles/37923459892507-Singular-MCP
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Singular Scopes
name_suffix: OAuth Scopes
note: Singular's REST APIs are API-key authenticated and have no scope surface at all. The only OAuth scopes Singular publishes belong to its two MCP endpoints, and both are declared in RFC 8414 authorization-server metadata fetched anonymously. Singular publishes no scopes reference page; these are read from the metadata documents themselves, which is why the descriptions below are derived from the published server behaviour rather than quoted.
overview: 'Singular publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Singular API on a user''s behalf.


  Tokens are issued from https://mcp.singular.net/oauth_server/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Singular
provider_slug: singular
schemes:
- flows:
  - authorizationUrl: https://mcp.singular.net/oauth_server/authorize
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://mcp.singular.net/oauth_server/register
    tokenUrl: https://mcp.singular.net/oauth_server/token
  name: Singular MCP
  resource: https://mcp.singular.net
  source: https://mcp.singular.net/.well-known/oauth-authorization-server
- flows:
  - authorizationUrl: https://www.singular.net/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://www.singular.net/oauth/token
  name: Singular WordPress MCP adapter
  resource: https://www.singular.net/wp-json/mcp/mcp-oauth-server
  source: https://www.singular.net/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- mcp:read
- mcp
scopes:
- description: Read-only access to the connecting Singular user's aggregated marketing report data through the Singular MCP server. Singular documents that the MCP inherits the connecting user's own data permissions and cannot reach user-level data.
  flows:
  - authorizationCode
  scope: mcp:read
- description: The single scope advertised by the WordPress MCP adapter on www.singular.net for its website-content MCP endpoint.
  flows:
  - authorizationCode
  scope: mcp
slug: singular-scopes
source_filename: singular-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://mcp.singular.net/.well-known/oauth-authorization-server\ndocs: https://support.singular.net/hc/en-us/articles/37923459892507-Singular-MCP\nnote: >-\n  Singular's REST APIs are API-key authenticated and have no scope surface at all. The only\n  OAuth scopes Singular publishes belong to its two MCP endpoints, and both are declared in\n  RFC 8414 authorization-server metadata fetched anonymously. Singular publishes no scopes\n  reference page; these are read from the metadata documents themselves, which is why the\n  descriptions below are derived from the published server behaviour rather than quoted.\nschemes:\n  - name: Singular MCP\n    source: https://mcp.singular.net/.well-known/oauth-authorization-server\n    resource: https://mcp.singular.net\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.singular.net/oauth_server/authorize\n        tokenUrl: https://mcp.singular.net/oauth_server/token\n\
  \        registrationUrl: https://mcp.singular.net/oauth_server/register\n        pkce: [S256]\n  - name: Singular WordPress MCP adapter\n    source: https://www.singular.net/.well-known/oauth-authorization-server\n    resource: https://www.singular.net/wp-json/mcp/mcp-oauth-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.singular.net/oauth/authorize\n        tokenUrl: https://www.singular.net/oauth/token\n        pkce: [S256]\nscopes:\n  - scope: mcp:read\n    description: >-\n      Read-only access to the connecting Singular user's aggregated marketing report data\n      through the Singular MCP server. Singular documents that the MCP inherits the connecting\n      user's own data permissions and cannot reach user-level data.\n    flows: [authorizationCode]\n    sources: [https://mcp.singular.net/.well-known/oauth-authorization-server]\n  - scope: mcp\n    description: >-\n      The single scope advertised by the WordPress MCP adapter on www.singular.net\
  \ for its\n      website-content MCP endpoint.\n    flows: [authorizationCode]\n    sources: [https://www.singular.net/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singular/refs/heads/main/scopes/singular-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Marketing Analytics
- Mobile Attribution
- Attribution
- Marketing
- Advertising
- Analytics
- Mobile Measurement Partner
- SKAdNetwork
- Deep Linking
- Fraud Prevention
- ETL
- MCP
- Ad Monetization
- Privacy
token_urls:
- https://mcp.singular.net/oauth_server/token
- https://www.singular.net/oauth/token
---
