---
api_specs:
- filename: ledgerbotje-nl-app-api-openapi.yml
  format: yaml
  label: Ledger Botje App API
  slug: ledgerbotje-nl-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgerbotje-nl/openapi/ledgerbotje-nl-app-api-openapi.yml
- filename: ledgerbotje-nl-well-known-api-openapi.yml
  format: yaml
  label: Ledger Botje .well Known API
  slug: ledgerbotje-nl-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgerbotje-nl/openapi/ledgerbotje-nl-well-known-api-openapi.yml
authorization_urls:
- https://ledgerbotje.nl/app/mcp/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ledger Botje Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ledger Botje publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ledger Botje API on a user''s behalf.


  Tokens are issued from https://ledgerbotje.nl/app/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ledger Botje
provider_slug: ledgerbotje-nl
schemes:
- description: OAuth 2.1 with mandatory PKCE (S256). Dynamic client registration via POST https://ledgerbotje.nl/app/mcp/oauth/register (RFC 7591). Access tokens live 1 hour; refresh tokens 30 days, rotating.
  flows:
  - authorizationUrl: https://ledgerbotje.nl/app/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://ledgerbotje.nl/app/mcp/oauth/token
  name: oauth2
  source: openapi/ledgerbotje-nl-openapi.json
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Call the Exact Online MCP tools on behalf of the user
  flows:
  - authorizationCode
  scope: mcp:tools
slug: ledgerbotje-nl-scopes
source_filename: ledgerbotje-nl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/ledgerbotje-nl-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/ledgerbotje-nl-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ledgerbotje.nl/app/mcp/oauth/authorize\n    tokenUrl: https://ledgerbotje.nl/app/mcp/oauth/token\n  description: OAuth 2.1 with mandatory PKCE (S256). Dynamic client registration via POST https://ledgerbotje.nl/app/mcp/oauth/register\n    (RFC 7591). Access tokens live 1 hour; refresh tokens 30 days, rotating.\nscopes:\n- scope: mcp:tools\n  description: Call the Exact Online MCP tools on behalf of the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ledgerbotje-nl-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ledgerbotje-nl/scopes/ledgerbotje-nl-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Accounting
- Artificial Intelligence
- Automation
- ExactOnline
- Netherlands
token_bound: false
token_urls:
- https://ledgerbotje.nl/app/mcp/oauth/token
---
