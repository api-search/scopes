---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Klutch Public API
  slug: klutch-public-api
  spec_type: Postman
  url: https://api-docs.klutchcard.com/
authorization_urls:
- https://graphql.klutchcard.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Klutch Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Klutch publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Klutch API on a user''s behalf.


  Tokens are issued from https://graphql.klutchcard.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Klutch
provider_slug: klutch
schemes:
- flows:
  - authorizationUrl: https://graphql.klutchcard.com/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    tokenUrl: https://graphql.klutchcard.com/oauth/token
  name: oauth2
  source: well-known/klutch-graphql-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- phone
- profile
scopes:
- description: OpenID Connect subject identifier; required to obtain an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: The user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: The user's phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: The user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: klutch-scopes
source_filename: klutch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/klutch-graphql-oauth-authorization-server.json,\n  well-known/klutch-mcp-oauth-protected-resource.json\ndocs: null\ndocs_note: >-\n  Klutch does not publish a scopes / permissions reference page. The scope list below\n  is taken verbatim from the live RFC 8414 authorization-server metadata on all three\n  hosts and the RFC 9728 protected-resource metadata on the MCP server, which agree.\n  These are the standard OpenID Connect identity scopes — Klutch does not expose\n  resource-level (cards / transactions / rules) scopes over OAuth. Fine-grained access\n  is instead governed by the Mini App permission model, where the installing user\n  grants a Mini App the ability to create cards, read transactions and create spending\n  controls.\nschemes:\n- name: oauth2\n  source: well-known/klutch-graphql-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://graphql.klutchcard.com/oauth/authorize\n\
  \    tokenUrl: https://graphql.klutchcard.com/oauth/token\n    code_challenge_methods_supported: [S256]\nscopes:\n- scope: openid\n  description: OpenID Connect subject identifier; required to obtain an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/klutch-graphql-oauth-authorization-server.json, well-known/klutch-mcp-oauth-protected-resource.json]\n- scope: email\n  description: The user's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/klutch-graphql-oauth-authorization-server.json, well-known/klutch-mcp-oauth-protected-resource.json]\n- scope: phone\n  description: The user's phone number claim.\n  flows: [authorizationCode]\n  sources: [well-known/klutch-graphql-oauth-authorization-server.json, well-known/klutch-mcp-oauth-protected-resource.json]\n- scope: profile\n  description: The user's basic profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/klutch-graphql-oauth-authorization-server.json, well-known/klutch-mcp-oauth-protected-resource.json]\n\
  miniapp_permissions:\n  model: >-\n    Documented in the Klutch Public API collection as the \"Miniapp Developer\" mode:\n    a registered Mini App authenticates on behalf of a user and, once authorized by\n    that user, may act in their context.\n  granted_capabilities:\n  - Create cards on behalf of users\n  - Read transactions\n  - Create spending controls\n  source: postman/klutch-public-api-postman.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klutch/refs/heads/main/scopes/klutch-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Financial Services
- Fintech
- Credit Cards
- Payments
- Card Issuing
- Virtual Cards
- Transactions
- Spend Management
- Personal Finance
- GraphQL
- Embedded Finance
- Agents
token_urls:
- https://graphql.klutchcard.com/oauth/token
---
