---
api_specs:
- filename: rybbit-analytics-api-openapi.yml
  format: yaml
  label: Rybbit Analytics API
  slug: rybbit-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-analytics-api-openapi.yml
- filename: rybbit-event-tracking-api-openapi.yml
  format: yaml
  label: Rybbit Event Tracking API
  slug: rybbit-event-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-event-tracking-api-openapi.yml
- filename: rybbit-sessions-api-openapi.yml
  format: yaml
  label: Rybbit Sessions API
  slug: rybbit-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-sessions-api-openapi.yml
authorization_urls:
- https://app.rybbit.io/api/auth/mcp/authorize
description: Rybbit runs an OAuth 2.1 authorization server for its hosted MCP endpoint. It is NOT declared in any OpenAPI securityScheme — Rybbit publishes no OpenAPI — so this scope list was read directly off the RFC 8414 / RFC 9728 discovery documents the API host serves anonymously. The same `resource:action` scope vocabulary also governs scoped API keys created via POST /api/user/api-keys with a `permissions` object, so these scopes are the provider's single permission model for both credentials. derive-oauth-scopes.py finds nothing here (0 oauth2 schemes in the specs); this file is deliberately probed, not derived, and must not be overwritten by that script.
docs: https://rybbit.com/docs/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Rybbit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rybbit publishes 29 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rybbit API on a user''s behalf.


  Tokens are issued from https://app.rybbit.io/api/auth/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rybbit
provider_slug: rybbit
schemes:
- bearer_methods:
  - header
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://app.rybbit.io/api/auth/mcp/authorize
    flow: authorizationCode
    refreshUrl: https://app.rybbit.io/api/auth/mcp/token
    tokenUrl: https://app.rybbit.io/api/auth/mcp/token
  grant_types:
  - authorization_code
  - refresh_token
  id_token_signing_alg:
  - RS256
  issuer: https://app.rybbit.io
  jwks_uri: https://app.rybbit.io/api/auth/mcp/jwks
  name: RybbitMCP
  pkce:
  - S256
  registration_endpoint: https://app.rybbit.io/api/auth/mcp/register
  resource: https://app.rybbit.io/api/mcp
  response_types:
  - code
  source: well-known/rybbit-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  userinfo_endpoint: https://app.rybbit.io/api/auth/mcp/userinfo
scope_count: 29
scope_names:
- openid
- profile
- email
- offline_access
- analytics:read
- sessions:read
- events:read
- users:read
- users:write
- goals:read
- goals:write
- funnels:read
- funnels:write
- dashboards:read
- dashboards:write
- flags:read
- flags:write
- experiments:read
- experiments:write
- sites:read
- sites:write
- gsc:read
- gsc:write
- org:read
- org:write
- replay:read
- replay:write
- sql:read
- ingest:write
scopes:
- description: Standard OIDC scope. Requesting only OIDC scopes yields an unrestricted grant.
  flows: []
  scope: openid
- description: Standard OIDC profile claims (name).
  flows: []
  scope: profile
- description: Standard OIDC email claims (email, email_verified).
  flows: []
  scope: email
- description: Issue a refresh token for long-lived agent sessions.
  flows: []
  scope: offline_access
- description: Read aggregate analytics — overview KPIs, time series, dimensional breakdowns, live visitors, errors, web vitals, retention, journeys.
  flows: []
  scope: analytics:read
- description: Read raw visitor sessions and individual session timelines.
  flows: []
  scope: sessions:read
- description: Read raw events and custom event names with counts.
  flows: []
  scope: events:read
- description: Read the person inventory and individual person profiles, traits, devices and locations.
  flows: []
  scope: users:read
- description: Identify a person, replace traits, and erase a person's analytics data (GDPR erasure).
  flows: []
  scope: users:write
- description: Read conversion goals and their conversion statistics.
  flows: []
  scope: goals:read
- description: Create, update and delete conversion goals.
  flows: []
  scope: goals:write
- description: Read saved funnels and run ad-hoc funnel analysis.
  flows: []
  scope: funnels:read
- description: Save, update and delete funnels.
  flows: []
  scope: funnels:write
- description: Read dashboard configuration.
  flows: []
  scope: dashboards:read
- description: Modify dashboard configuration.
  flows: []
  scope: dashboards:write
- description: Read feature flags.
  flows: []
  scope: flags:read
- description: Create and modify feature flags.
  flows: []
  scope: flags:write
- description: Read experiments.
  flows: []
  scope: experiments:read
- description: Create and modify experiments.
  flows: []
  scope: experiments:write
- description: Read site configuration and the list of accessible sites.
  flows: []
  scope: sites:read
- description: Create sites, change site configuration, and delete sites (admin/owner role also required).
  flows: []
  scope: sites:write
- description: Read the Google Search Console integration data.
  flows: []
  scope: gsc:read
- description: Configure the Google Search Console integration.
  flows: []
  scope: gsc:write
- description: Read organization members, roles, site access and teams.
  flows: []
  scope: org:read
- description: Add members, change member site access, and create/update/delete teams (admin/owner role also required).
  flows: []
  scope: org:write
- description: Read session replay recordings and their rrweb event streams.
  flows: []
  scope: replay:read
- description: Delete session replay recordings.
  flows: []
  scope: replay:write
- description: Read-only ClickHouse SQL against the site-scoped scoped_events table, plus the query schema.
  flows: []
  scope: sql:read
- description: Write events into the ingestion pipeline. Advertised by the authorization server; no MCP tool currently exposes it.
  flows: []
  scope: ingest:write
slug: rybbit-scopes
source_filename: rybbit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://app.rybbit.io/.well-known/oauth-authorization-server (HTTP 200,\n  application/json, fetched 2026-08-13) and\n  https://app.rybbit.io/.well-known/oauth-protected-resource (HTTP 200) —\n  both saved verbatim under well-known/. Scope semantics and the\n  write-implies-read rule come from https://rybbit.com/docs/mcp.\ndocs: https://rybbit.com/docs/mcp\ndescription: >-\n  Rybbit runs an OAuth 2.1 authorization server for its hosted MCP endpoint.\n  It is NOT declared in any OpenAPI securityScheme — Rybbit publishes no\n  OpenAPI — so this scope list was read directly off the RFC 8414 / RFC 9728\n  discovery documents the API host serves anonymously. The same\n  `resource:action` scope vocabulary also governs scoped API keys created via\n  POST /api/user/api-keys with a `permissions` object, so these scopes are the\n  provider's single permission model for both credentials.\n  derive-oauth-scopes.py finds nothing here\
  \ (0 oauth2 schemes in the specs);\n  this file is deliberately probed, not derived, and must not be overwritten\n  by that script.\n\nschemes:\n  - name: RybbitMCP\n    type: oauth2\n    source: well-known/rybbit-oauth-authorization-server.json\n    issuer: https://app.rybbit.io\n    resource: https://app.rybbit.io/api/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.rybbit.io/api/auth/mcp/authorize\n        tokenUrl: https://app.rybbit.io/api/auth/mcp/token\n        refreshUrl: https://app.rybbit.io/api/auth/mcp/token\n    userinfo_endpoint: https://app.rybbit.io/api/auth/mcp/userinfo\n    jwks_uri: https://app.rybbit.io/api/auth/mcp/jwks\n    registration_endpoint: https://app.rybbit.io/api/auth/mcp/register\n    dynamic_client_registration: true\n    pkce: [S256]\n    grant_types: [authorization_code, refresh_token]\n    response_types: [code]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    id_token_signing_alg:\
  \ [RS256]\n    bearer_methods: [header]\n\nrules:\n  - '`write` implies `read` on the same resource.'\n  - >-\n    Scopes never elevate: organization admin/owner role requirements still\n    apply after a scope check passes.\n  - >-\n    A grant (or key) that requests only the standard OIDC scopes is\n    UNRESTRICTED — it acts with the full authority of the user. Restriction\n    only happens when custom `resource:action` scopes are requested.\n  - >-\n    Consent is currently approve-or-deny as a whole; the requesting client\n    chooses which scopes to ask for.\n  - >-\n    An out-of-scope call returns 403 {\"error\":\"Insufficient scope\",\"required\":\"goals:write\"}.\n\nscope_count: 29\n\nscopes:\n  - {scope: openid, description: 'Standard OIDC scope. Requesting only OIDC scopes yields an unrestricted grant.', kind: oidc}\n  - {scope: profile, description: 'Standard OIDC profile claims (name).', kind: oidc}\n  - {scope: email, description: 'Standard OIDC email claims (email, email_verified).',\
  \ kind: oidc}\n  - {scope: offline_access, description: 'Issue a refresh token for long-lived agent sessions.', kind: oidc}\n  - {scope: 'analytics:read', description: 'Read aggregate analytics — overview KPIs, time series, dimensional breakdowns, live visitors, errors, web vitals, retention, journeys.', kind: resource}\n  - {scope: 'sessions:read', description: 'Read raw visitor sessions and individual session timelines.', kind: resource}\n  - {scope: 'events:read', description: 'Read raw events and custom event names with counts.', kind: resource}\n  - {scope: 'users:read', description: 'Read the person inventory and individual person profiles, traits, devices and locations.', kind: resource}\n  - {scope: 'users:write', description: 'Identify a person, replace traits, and erase a person''s analytics data (GDPR erasure).', kind: resource}\n  - {scope: 'goals:read', description: 'Read conversion goals and their conversion statistics.', kind: resource}\n  - {scope: 'goals:write', description:\
  \ 'Create, update and delete conversion goals.', kind: resource}\n  - {scope: 'funnels:read', description: 'Read saved funnels and run ad-hoc funnel analysis.', kind: resource}\n  - {scope: 'funnels:write', description: 'Save, update and delete funnels.', kind: resource}\n  - {scope: 'dashboards:read', description: 'Read dashboard configuration.', kind: resource}\n  - {scope: 'dashboards:write', description: 'Modify dashboard configuration.', kind: resource}\n  - {scope: 'flags:read', description: 'Read feature flags.', kind: resource}\n  - {scope: 'flags:write', description: 'Create and modify feature flags.', kind: resource}\n  - {scope: 'experiments:read', description: 'Read experiments.', kind: resource}\n  - {scope: 'experiments:write', description: 'Create and modify experiments.', kind: resource}\n  - {scope: 'sites:read', description: 'Read site configuration and the list of accessible sites.', kind: resource}\n  - {scope: 'sites:write', description: 'Create sites, change site\
  \ configuration, and delete sites (admin/owner role also required).', kind: resource}\n  - {scope: 'gsc:read', description: 'Read the Google Search Console integration data.', kind: resource}\n  - {scope: 'gsc:write', description: 'Configure the Google Search Console integration.', kind: resource}\n  - {scope: 'org:read', description: 'Read organization members, roles, site access and teams.', kind: resource}\n  - {scope: 'org:write', description: 'Add members, change member site access, and create/update/delete teams (admin/owner role also required).', kind: resource}\n  - {scope: 'replay:read', description: 'Read session replay recordings and their rrweb event streams.', kind: resource}\n  - {scope: 'replay:write', description: 'Delete session replay recordings.', kind: resource}\n  - {scope: 'sql:read', description: 'Read-only ClickHouse SQL against the site-scoped scoped_events table, plus the query schema.', kind: resource}\n  - {scope: 'ingest:write', description: 'Write events into\
  \ the ingestion pipeline. Advertised by the authorization server; no MCP tool currently exposes it.', kind: resource}\n\nx-evidence:\n  - {url: 'https://app.rybbit.io/.well-known/oauth-authorization-server', http_status: 200, content_type: 'application/json'}\n  - {url: 'https://app.rybbit.io/.well-known/openid-configuration', http_status: 200, content_type: 'application/json'}\n  - {url: 'https://app.rybbit.io/.well-known/oauth-protected-resource', http_status: 200, content_type: 'application/json'}\nx-evidence-fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/scopes/rybbit-scopes.yml
summary_line: 29 scopes · authorizationCode
tags:
- Analytics
- Web Analytics
- Product Analytics
- Privacy
- Open-Source
- Cookieless
token_urls:
- https://app.rybbit.io/api/auth/mcp/token
---
