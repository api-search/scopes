---
api_specs:
- filename: contextdev-openapi.yml
  format: yaml
  label: Context API
  slug: context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-openapi.yml
authorization_urls: []
description: ''
docs: https://www.context.dev/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Contextdev Scopes
name_suffix: OAuth Scopes
note: Scopes are exposed via the OAuth2 agent-auth (service_auth) flow, not via the static-API-key path. The OpenAPI declares only bearerAuth (http bearer); the scope surface is documented in the well-known metadata and auth.md.
overview: 'Context.dev publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Context.dev API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Context.dev
provider_slug: contextdev
schemes:
- authorization_server: https://www.context.dev
  grant_types:
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:workos:agent-auth:grant-type:claim
  name: AgentAuth
  revocation_endpoint: https://www.context.dev/oauth2/revoke
  source: well-known/contextdev-oauth-authorization-server.json
  token_endpoint: https://www.context.dev/oauth2/token
scope_count: 2
scope_names:
- api.read
- api.write
scopes:
- description: Read access to Context.dev API endpoints (brand lookup, web scrape/crawl, search, enrichment, and related read operations).
  flows: []
  scope: api.read
- description: Write access for mutating API operations (e.g. creating/updating/deleting monitors). Agent credentials are issued with both api.read and api.write after the claim ceremony.
  flows: []
  scope: api.write
slug: contextdev-scopes
source_filename: contextdev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://www.context.dev/.well-known/oauth-authorization-server and\n  https://www.context.dev/auth.md\ndocs: https://www.context.dev/auth.md\nschemes:\n- name: AgentAuth\n  source: well-known/contextdev-oauth-authorization-server.json\n  authorization_server: https://www.context.dev\n  token_endpoint: https://www.context.dev/oauth2/token\n  revocation_endpoint: https://www.context.dev/oauth2/revoke\n  grant_types:\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:workos:agent-auth:grant-type:claim\nscopes:\n- scope: api.read\n  description: >-\n    Read access to Context.dev API endpoints (brand lookup, web scrape/crawl,\n    search, enrichment, and related read operations).\n  sources:\n  - well-known/contextdev-oauth-authorization-server.json\n- scope: api.write\n  description: >-\n    Write access for mutating API operations (e.g. creating/updating/deleting\n    monitors). Agent credentials are issued with\
  \ both api.read and api.write\n    after the claim ceremony.\n  sources:\n  - well-known/contextdev-oauth-authorization-server.json\nnote: >-\n  Scopes are exposed via the OAuth2 agent-auth (service_auth) flow, not via the\n  static-API-key path. The OpenAPI declares only bearerAuth (http bearer); the\n  scope surface is documented in the well-known metadata and auth.md.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/scopes/contextdev-scopes.yml
summary_line: 2 scopes
tags:
- Web Scraping
- Brand Intelligence
- Data Enrichment
- AI Agents
- Web Data
- Classification
- Website Monitoring
- Company Data
- Developer Tools
- APIs
token_urls: []
---
