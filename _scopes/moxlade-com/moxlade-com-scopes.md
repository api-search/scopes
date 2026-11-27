---
api_specs:
- filename: moxlade-com-ext-api-openapi.yml
  format: yaml
  label: Moxlade Ext API
  slug: moxlade-com-ext-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moxlade-com/openapi/moxlade-com-ext-api-openapi.yml
- filename: moxlade-com-mcp-api-openapi.yml
  format: yaml
  label: Moxlade MCP API
  slug: moxlade-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moxlade-com/openapi/moxlade-com-mcp-api-openapi.yml
authorization_urls:
- https://clerk.buyer.moxlade.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Moxlade Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Moxlade publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Moxlade API on a user''s behalf.


  Tokens are issued from https://clerk.buyer.moxlade.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moxlade
provider_slug: moxlade-com
schemes:
- description: OAuth 2.1. Discover from the 401's WWW-Authenticate header, or read https://buyer.moxlade.com/.well-known/oauth-protected-resource directly. Clients register themselves; PKCE required; pass resource=https://buyer.moxlade.com/mcp/ so the token is bound to this server.
  flows:
  - authorizationUrl: https://clerk.buyer.moxlade.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clerk.buyer.moxlade.com/oauth/token
  name: oauth2
  source: openapi/moxlade-com-openapi.json
scope_count: 4
scope_names:
- email
- mcp:tools
- offline_access
- profile
scopes:
- description: Your email address
  flows:
  - authorizationCode
  scope: email
- description: Call the corpus tools
  flows:
  - authorizationCode
  scope: mcp:tools
- description: Refresh without signing in again
  flows:
  - authorizationCode
  scope: offline_access
- description: Your name
  flows:
  - authorizationCode
  scope: profile
slug: moxlade-com-scopes
source_filename: moxlade-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/moxlade-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/moxlade-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.buyer.moxlade.com/oauth/authorize\n    tokenUrl: https://clerk.buyer.moxlade.com/oauth/token\n  description: OAuth 2.1. Discover from the 401's WWW-Authenticate header, or read https://buyer.moxlade.com/.well-known/oauth-protected-resource\n    directly. Clients register themselves; PKCE required; pass resource=https://buyer.moxlade.com/mcp/\n    so the token is bound to this server.\nscopes:\n- scope: email\n  description: Your email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/moxlade-com-openapi.json\n- scope: mcp:tools\n  description: Call the corpus tools\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/moxlade-com-openapi.json\n- scope: offline_access\n  description: Refresh without signing in again\n  flows:\n  -\
  \ authorizationCode\n  sources:\n  - openapi/moxlade-com-openapi.json\n- scope: profile\n  description: Your name\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/moxlade-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/moxlade-com/scopes/moxlade-com-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Upwork data
- Freelancer data
- Buyer Intelligence
- Data Marketplace
- Apify actors
token_bound: false
token_urls:
- https://clerk.buyer.moxlade.com/oauth/token
---
