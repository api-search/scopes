---
api_specs:
- filename: lusha-search-api-openapi.yml
  format: yaml
  label: Lusha Search API
  slug: lusha-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-search-api-openapi.yml
- filename: lusha-enrich-api-openapi.yml
  format: yaml
  label: Lusha Enrich API
  slug: lusha-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-enrich-api-openapi.yml
- filename: lusha-search-enrich-api-openapi.yml
  format: yaml
  label: Lusha Search & Enrich API
  slug: lusha-search-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-search-enrich-api-openapi.yml
- filename: lusha-prospecting-api-openapi.yml
  format: yaml
  label: Lusha Prospecting API
  slug: lusha-prospecting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-prospecting-api-openapi.yml
- filename: lusha-lookalikes-api-openapi.yml
  format: yaml
  label: Lusha Lookalikes API
  slug: lusha-lookalike-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-lookalikes-api-openapi.yml
- filename: lusha-buying-group-api-openapi.yml
  format: yaml
  label: Lusha Buying Group API
  slug: lusha-buying-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-buying-group-api-openapi.yml
- filename: lusha-signals-api-openapi.yml
  format: yaml
  label: Lusha Signals API
  slug: lusha-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-signals-api-openapi.yml
- filename: lusha-website-visits-api-openapi.yml
  format: yaml
  label: Lusha Website Visitors API
  slug: lusha-website-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-website-visits-api-openapi.yml
- filename: lusha-filters-api-openapi.yml
  format: yaml
  label: Lusha Filters API
  slug: lusha-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-filters-api-openapi.yml
- filename: lusha-contacts-tables-api-openapi.yml
  format: yaml
  label: Lusha Contacts Tables API
  slug: lusha-contacts-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-contacts-tables-api-openapi.yml
- filename: lusha-companies-tables-api-openapi.yml
  format: yaml
  label: Lusha Companies Tables API
  slug: lusha-companies-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-companies-tables-api-openapi.yml
- filename: lusha-webhooks-api-openapi.yml
  format: yaml
  label: Lusha Webhooks API
  slug: lusha-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-webhooks-api-openapi.yml
- filename: lusha-account-api-openapi.yml
  format: yaml
  label: Lusha Account API
  slug: lusha-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-account-api-openapi.yml
authorization_urls:
- https://auth.lusha.com/oauth-ui/authorize
description: The Lusha REST API has NO OAuth surface — it authenticates with a single `api_key` header and therefore has no scopes (derive-oauth-scopes.py over the OpenAPI correctly finds zero oauth2 schemes). OAuth exists only in front of the MCP server, and it advertises exactly one coarse scope, `mcp`, which grants a connected agent the whole published tool set. There is no read/write split, no per-product scope, and no per-tool consent surface.
docs: https://docs.lusha.com/mcp-docs
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Lusha Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lusha publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lusha API on a user''s behalf.


  Tokens are issued from https://auth.lusha.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lusha
provider_slug: lusha
schemes:
- authorization_server: https://auth.lusha.com
  bearer_methods:
  - header
  flows:
  - authorizationUrl: https://auth.lusha.com/oauth-ui/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://auth.lusha.com/oauth/token
    registrationUrl: https://auth.lusha.com/oauth/register
    revocationUrl: https://auth.lusha.com/oauth/revoke
    tokenUrl: https://auth.lusha.com/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: LushaMCPOAuth
  resource: https://mcp.lusha.com
  source: https://mcp.lusha.com/.well-known/oauth-protected-resource
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Full access to the Lusha MCP tool surface for the authenticated user — search, enrichment, prospecting, lookalikes, signals, recommendations and account usage. Credit-consuming tools are covered by the same scope as read-only filter tools.
  flows:
  - authorizationCode
  scope: mcp
slug: lusha-scopes
source_filename: lusha-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.lusha.com/.well-known/oauth-authorization-server\ndocs: https://docs.lusha.com/mcp-docs\ndescription: >-\n  The Lusha REST API has NO OAuth surface — it authenticates with a single\n  `api_key` header and therefore has no scopes (derive-oauth-scopes.py over the\n  OpenAPI correctly finds zero oauth2 schemes). OAuth exists only in front of the\n  MCP server, and it advertises exactly one coarse scope, `mcp`, which grants a\n  connected agent the whole published tool set. There is no read/write split, no\n  per-product scope, and no per-tool consent surface.\napplies_to: mcp\nschemes:\n- name: LushaMCPOAuth\n  type: oauth2\n  source: https://mcp.lusha.com/.well-known/oauth-protected-resource\n  resource: https://mcp.lusha.com\n  authorization_server: https://auth.lusha.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.lusha.com/oauth-ui/authorize\n    tokenUrl: https://auth.lusha.com/oauth/token\n\
  \    refreshUrl: https://auth.lusha.com/oauth/token\n    revocationUrl: https://auth.lusha.com/oauth/revoke\n    registrationUrl: https://auth.lusha.com/oauth/register\n    pkce: S256\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n  bearer_methods: [header]\nscopes:\n- scope: mcp\n  description: >-\n    Full access to the Lusha MCP tool surface for the authenticated user —\n    search, enrichment, prospecting, lookalikes, signals, recommendations and\n    account usage. Credit-consuming tools are covered by the same scope as\n    read-only filter tools.\n  flows: [authorizationCode]\n  sources: [https://mcp.lusha.com/.well-known/oauth-authorization-server]\nscope_count: 1\ngaps:\n- >-\n    A single scope means an agent granted MCP access can spend credits (contact\n    and company reveals at 1-5 credits per data point) with no narrower consent\n    step. A read-only / filters-only scope would let an operator hand an agent\n    discovery without spend.\nx-evidence:\n\
  - url: https://mcp.lusha.com/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://mcp.lusha.com/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://auth.lusha.com/.well-known/oauth-protected-resource\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/scopes/lusha-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Sales Intelligence
- B2B
- Enrichment
- Contact Data
- Prospecting
- Intent
- Signals
- Lookalikes
- Webhooks
- MCP
token_urls:
- https://auth.lusha.com/oauth/token
---
