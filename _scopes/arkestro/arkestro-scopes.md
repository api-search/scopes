---
api_specs:
- filename: arkestro-awards-api-openapi.yml
  format: yaml
  label: Arkestro Awards API
  slug: arkestro-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-awards-api-openapi.yml
- filename: arkestro-business-unit-api-openapi.yml
  format: yaml
  label: Arkestro business unit API
  slug: arkestro-business-unit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-business-unit-api-openapi.yml
- filename: arkestro-corporate-categories-api-openapi.yml
  format: yaml
  label: Arkestro corporate categories API
  slug: arkestro-corporate-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-corporate-categories-api-openapi.yml
- filename: arkestro-corporate-items-api-openapi.yml
  format: yaml
  label: Arkestro corporate items API
  slug: arkestro-corporate-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-corporate-items-api-openapi.yml
- filename: arkestro-corporate-purchase-orders-api-openapi.yml
  format: yaml
  label: Arkestro corporate purchase orders API
  slug: arkestro-corporate-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-corporate-purchase-orders-api-openapi.yml
- filename: arkestro-document-submissions-api-openapi.yml
  format: yaml
  label: Arkestro document submissions API
  slug: arkestro-document-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-document-submissions-api-openapi.yml
- filename: arkestro-event-analytics-api-openapi.yml
  format: yaml
  label: Arkestro event analytics API
  slug: arkestro-event-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-event-analytics-api-openapi.yml
- filename: arkestro-event-documents-api-openapi.yml
  format: yaml
  label: Arkestro event documents API
  slug: arkestro-event-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-event-documents-api-openapi.yml
- filename: arkestro-events-api-openapi.yml
  format: yaml
  label: Arkestro Events API
  slug: arkestro-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-events-api-openapi.yml
- filename: arkestro-quote-submissions-api-openapi.yml
  format: yaml
  label: Arkestro quote submissions API
  slug: arkestro-quote-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-quote-submissions-api-openapi.yml
- filename: arkestro-schedules-api-openapi.yml
  format: yaml
  label: Arkestro Schedules API
  slug: arkestro-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-schedules-api-openapi.yml
- filename: arkestro-supplier-contacts-api-openapi.yml
  format: yaml
  label: Arkestro supplier contacts API
  slug: arkestro-supplier-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-supplier-contacts-api-openapi.yml
- filename: arkestro-supplier-organizations-api-openapi.yml
  format: yaml
  label: Arkestro supplier organizations API
  slug: arkestro-supplier-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/openapi/arkestro-supplier-organizations-api-openapi.yml
authorization_urls:
- https://api.arkestro.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Arkestro Scopes
name_suffix: OAuth Scopes
note: These scopes are not derivable from the OpenAPI — the published spec declares only an apiKey scheme. They come from Arkestro's live RFC 8414 authorization-server metadata and govern the remote MCP server at https://api.arkestro.com/api/v2/mcp, not the REST API V2. Arkestro publishes no scope reference page; descriptions below are the plain reading of the scope names and are marked as such rather than quoted from documentation.
overview: 'Arkestro publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arkestro API on a user''s behalf.


  Tokens are issued from https://api.arkestro.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arkestro
provider_slug: arkestro
schemes:
- flows:
  - authorizationUrl: https://api.arkestro.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pkce_required: true
    tokenUrl: https://api.arkestro.com/oauth/token
  issuer: https://api.arkestro.com
  name: OAuth2
  source: well-known/arkestro-oauth-authorization-server.json
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- offline_access
scopes:
- description: Read access through the MCP server.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access through the MCP server.
  flows:
  - authorizationCode
  scope: mcp:write
- description: Issue a refresh token so the client can act without the user present.
  flows:
  - authorizationCode
  scope: offline_access
slug: arkestro-scopes
source_filename: arkestro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://api.arkestro.com/.well-known/oauth-authorization-server\nnote: >-\n  These scopes are not derivable from the OpenAPI — the published spec declares only an\n  apiKey scheme. They come from Arkestro's live RFC 8414 authorization-server metadata and\n  govern the remote MCP server at https://api.arkestro.com/api/v2/mcp, not the REST API V2.\n  Arkestro publishes no scope reference page; descriptions below are the plain reading of\n  the scope names and are marked as such rather than quoted from documentation.\nschemes:\n- name: OAuth2\n  source: well-known/arkestro-oauth-authorization-server.json\n  issuer: https://api.arkestro.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.arkestro.com/oauth/authorize\n    tokenUrl: https://api.arkestro.com/oauth/token\n    pkce_required: true\n    code_challenge_methods:\n    - S256\nscopes:\n- scope: mcp:read\n  description: Read access through the MCP server.\n\
  \  description_source: inferred-from-scope-name\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/arkestro-oauth-authorization-server.json\n- scope: mcp:write\n  description: Write access through the MCP server.\n  description_source: inferred-from-scope-name\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/arkestro-oauth-authorization-server.json\n- scope: offline_access\n  description: Issue a refresh token so the client can act without the user present.\n  description_source: standard-oidc-scope\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/arkestro-oauth-authorization-server.json\ncoverage:\n  scopes_published: 3\n  granularity: coarse\n  note: >-\n    Two functional scopes for an entire procurement platform. A read/write split alone\n    cannot express least privilege across events, awards, purchase orders, supplier\n    organizations and analytics — an agent granted mcp:write to schedule an event also\n    holds whatever write reach the server\
  \ exposes over awards and purchase orders.\nx-evidence:\n- url: https://api.arkestro.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arkestro/refs/heads/main/scopes/arkestro-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Procurement
- sourcing
- Supply Chain
- spend-management
- e-sourcing
- supplier-management
- purchase-orders
- procurement-analytics
- enterprise-software
- predictive-procurement
- MCP
- Webhook
token_urls:
- https://api.arkestro.com/oauth/token
---
