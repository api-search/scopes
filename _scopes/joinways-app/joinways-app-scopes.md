---
api_specs:
- filename: joinways-app-analytics-api-openapi.yml
  format: yaml
  label: Joinways Analytics API
  slug: joinways-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-analytics-api-openapi.yml
- filename: joinways-app-catalog-api-openapi.yml
  format: yaml
  label: Joinways Catalog API
  slug: joinways-app-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-catalog-api-openapi.yml
- filename: joinways-app-companies-api-openapi.yml
  format: yaml
  label: Joinways Companies API
  slug: joinways-app-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-companies-api-openapi.yml
- filename: joinways-app-events-api-openapi.yml
  format: yaml
  label: Joinways Events API
  slug: joinways-app-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-events-api-openapi.yml
- filename: joinways-app-invoices-api-openapi.yml
  format: yaml
  label: Joinways Invoices API
  slug: joinways-app-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-invoices-api-openapi.yml
- filename: joinways-app-leads-api-openapi.yml
  format: yaml
  label: Joinways Leads API
  slug: joinways-app-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-leads-api-openapi.yml
- filename: joinways-app-notifications-api-openapi.yml
  format: yaml
  label: Joinways Notifications API
  slug: joinways-app-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-notifications-api-openapi.yml
- filename: joinways-app-people-api-openapi.yml
  format: yaml
  label: Joinways People API
  slug: joinways-app-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-people-api-openapi.yml
- filename: joinways-app-quotes-api-openapi.yml
  format: yaml
  label: Joinways Quotes API
  slug: joinways-app-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-quotes-api-openapi.yml
- filename: joinways-app-search-api-openapi.yml
  format: yaml
  label: Joinways Search API
  slug: joinways-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-search-api-openapi.yml
- filename: joinways-app-tasks-api-openapi.yml
  format: yaml
  label: Joinways Tasks API
  slug: joinways-app-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-tasks-api-openapi.yml
- filename: joinways-app-team-api-openapi.yml
  format: yaml
  label: Joinways Team API
  slug: joinways-app-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-team-api-openapi.yml
- filename: joinways-app-venues-api-openapi.yml
  format: yaml
  label: Joinways Venues API
  slug: joinways-app-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-venues-api-openapi.yml
- filename: joinways-app-webhooks-api-openapi.yml
  format: yaml
  label: Joinways Webhooks API
  slug: joinways-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-webhooks-api-openapi.yml
authorization_urls:
- https://joinways.app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Joinways Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Joinways publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Joinways API on a user''s behalf.


  Tokens are issued from https://joinways.app/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Joinways
provider_slug: joinways-app
schemes:
- description: 'OAuth 2.1 authorization code grant with mandatory PKCE (S256). Access tokens are opaque strings prefixed `jw_oat_`, presented as `Authorization: Bearer …`: valid 1 hour with a refresh token (`jw_ort_…`, rotated on each use, 90 days idle), 30 days for a client without the refresh grant. Send `resource=https://joinways.app/api/v1` (RFC 8707). Clients register dynamically or use an https `client_id` (Client ID Metadata Document). Tokens are bound to a single workspace.'
  flows:
  - authorizationUrl: https://joinways.app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://joinways.app/api/oauth/token
  name: oauth2
  source: openapi/joinways-app-openapi.yml
scope_count: 2
scope_names:
- mcp.read
- mcp.write
scopes:
- description: Read the workspace data the member's role can read.
  flows:
  - authorizationCode
  scope: mcp.read
- description: Create, update, delete and actions within the member's role (implies read).
  flows:
  - authorizationCode
  scope: mcp.write
slug: joinways-app-scopes
source_filename: joinways-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/joinways-app-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/joinways-app-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://joinways.app/oauth/authorize\n    tokenUrl: https://joinways.app/api/oauth/token\n  description: 'OAuth 2.1 authorization code grant with mandatory PKCE (S256). Access tokens\n    are opaque strings prefixed `jw_oat_`, presented as `Authorization: Bearer …`: valid 1 hour\n    with a refresh token (`jw_ort_…`, rotated on each use, 90 days idle), 30 days for a client\n    without the refresh grant. Send `resource=https://joinways.app/api/v1` (RFC 8707). Clients\n    register dynamically or use an https `client_id` (Client ID Metadata Document). Tokens are\n    bound to a single workspace.'\nscopes:\n- scope: mcp.read\n  description: Read the workspace data the member's role can read.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/joinways-app-openapi.yml\n\
  - scope: mcp.write\n  description: Create, update, delete and actions within the member's role (implies read).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/joinways-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/joinways-app/scopes/joinways-app-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Event Management
- Software-as-a-Service
- CRM
- Venue Software
- Multilingual
token_bound: false
token_urls:
- https://joinways.app/api/oauth/token
---
