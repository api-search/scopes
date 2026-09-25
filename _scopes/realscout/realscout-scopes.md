---
authorization_urls:
- https://www.realscout.com/oauth/authorize
description: ''
docs: https://www.realscout.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Realscout Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RealScout publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RealScout API on a user''s behalf.


  Tokens are issued from https://www.realscout.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RealScout
provider_slug: realscout
schemes:
- flows:
  - authorizationUrl: https://www.realscout.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.realscout.com/oauth/token
  name: OAuth2
  source: well-known/realscout-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to the RealScout admin MCP server (protected resource api://realscout-admin-mcp). Declared in scopes_supported of the authorization-server metadata.
  flows:
  - authorizationCode
  scope: mcp
slug: realscout-scopes
source_filename: realscout-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.realscout.com/.well-known/oauth-authorization-server\ndocs: https://www.realscout.com/.well-known/oauth-authorization-server\nschemes:\n  - name: OAuth2\n    source: well-known/realscout-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.realscout.com/oauth/authorize\n        tokenUrl: https://www.realscout.com/oauth/token\nscopes:\n  - scope: mcp\n    description: >-\n      Access to the RealScout admin MCP server (protected resource\n      api://realscout-admin-mcp). Declared in scopes_supported of the\n      authorization-server metadata.\n    flows: [authorizationCode]\n    sources: [well-known/realscout-oauth-authorization-server.json]\nnotes: >-\n  Only one scope (\"mcp\") is published in the authorization-server metadata. It\n  gates the hosted MCP server. No broader scope/permission reference is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realscout/refs/heads/main/scopes/realscout-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Enterprise
- Real Estate
- PropTech
- Lead Nurture
- Home Search
- MLS
- MCP
- Artificial Intelligence
token_urls:
- https://www.realscout.com/oauth/token
---
