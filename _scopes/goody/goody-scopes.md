---
api_specs:
- filename: goody-api-openapi-original.json
  format: json
  label: Goody API
  slug: goody-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-api-openapi-original.json
authorization_urls:
- https://api.ongoody.com/oauth/authorize
description: ''
docs: https://developer.ongoody.com/mcp/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Goody Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Goody publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Goody API on a user''s behalf.


  Tokens are issued from https://api.ongoody.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Goody
provider_slug: goody
schemes:
- flows:
  - authorizationUrl: https://api.ongoody.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.ongoody.com/oauth/token
  name: mcp_oauth2
  source: well-known/goody-oauth-authorization-server.json
scope_count: 4
scope_names:
- mcp.read
- mcp.write
- mcp.gifts
- chrome.write
scopes:
- description: 'Read access via the MCP server / OAuth clients: list workspaces, search the catalog and contacts, price and preview gifts, read orders.'
  flows:
  - authorizationCode
  scope: mcp.read
- description: 'Write access short of charging: create/update contacts and contact lists, cancel orders, build previews, pause autogift rules, submit feedback.'
  flows:
  - authorizationCode
  scope: mcp.write
- description: 'Send gifts / spend money: create an order batch (charges the payment method) and create or activate autogift rules. Highest-consequence scope.'
  flows:
  - authorizationCode
  scope: mcp.gifts
- description: Scope used by Goody's browser extension / Chrome client integration.
  flows:
  - authorizationCode
  scope: chrome.write
slug: goody-scopes
source_filename: goody-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/goody-oauth-authorization-server.json\ndocs: https://developer.ongoody.com/mcp/authentication\nschemes:\n- name: mcp_oauth2\n  source: well-known/goody-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.ongoody.com/oauth/authorize\n    tokenUrl: https://api.ongoody.com/oauth/token\n    pkce: S256\nscopes:\n- scope: mcp.read\n  description: >-\n    Read access via the MCP server / OAuth clients: list workspaces, search\n    the catalog and contacts, price and preview gifts, read orders.\n  flows: [authorizationCode]\n  sources: [well-known/goody-oauth-authorization-server.json]\n- scope: mcp.write\n  description: >-\n    Write access short of charging: create/update contacts and contact lists,\n    cancel orders, build previews, pause autogift rules, submit feedback.\n  flows: [authorizationCode]\n  sources: [well-known/goody-oauth-authorization-server.json]\n\
  - scope: mcp.gifts\n  description: >-\n    Send gifts / spend money: create an order batch (charges the payment\n    method) and create or activate autogift rules. Highest-consequence scope.\n  flows: [authorizationCode]\n  sources: [well-known/goody-oauth-authorization-server.json]\n- scope: chrome.write\n  description: >-\n    Scope used by Goody's browser extension / Chrome client integration.\n  flows: [authorizationCode]\n  sources: [well-known/goody-oauth-authorization-server.json]\nnotes: >-\n  The MCP permission model (Read / Write / Send gifts) maps directly onto the\n  three mcp.* scopes. The REST Commerce/Automation API itself uses a bearer\n  API key with no scope surface; these scopes govern the OAuth/MCP path only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/scopes/goody-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- Gifting
- Gift Cards
- E-Commerce
- Commerce
- Payments
- MCP
- Webhooks
- Rewards
token_urls:
- https://api.ongoody.com/oauth/token
---
