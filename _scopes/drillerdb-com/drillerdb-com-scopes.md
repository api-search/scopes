---
api_specs:
- filename: drillerdb-com-conferences-api-openapi.yml
  format: yaml
  label: DrillerDB Conferences API
  slug: drillerdb-com-conferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-conferences-api-openapi.yml
- filename: drillerdb-com-contacts-api-openapi.yml
  format: yaml
  label: DrillerDB Contacts API
  slug: drillerdb-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-contacts-api-openapi.yml
- filename: drillerdb-com-documentation-api-openapi.yml
  format: yaml
  label: DrillerDB Documentation API
  slug: drillerdb-com-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-documentation-api-openapi.yml
- filename: drillerdb-com-driller-directory-api-openapi.yml
  format: yaml
  label: DrillerDB Driller directory API
  slug: drillerdb-com-driller-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-driller-directory-api-openapi.yml
- filename: drillerdb-com-enterprise-mcp-api-openapi.yml
  format: yaml
  label: DrillerDB Enterprise MCP API
  slug: drillerdb-com-enterprise-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-enterprise-mcp-api-openapi.yml
- filename: drillerdb-com-equipment-api-openapi.yml
  format: yaml
  label: DrillerDB Equipment API
  slug: drillerdb-com-equipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-equipment-api-openapi.yml
- filename: drillerdb-com-geocoding-api-openapi.yml
  format: yaml
  label: DrillerDB Geocoding API
  slug: drillerdb-com-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-geocoding-api-openapi.yml
- filename: drillerdb-com-inventory-api-openapi.yml
  format: yaml
  label: DrillerDB Inventory API
  slug: drillerdb-com-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-inventory-api-openapi.yml
- filename: drillerdb-com-invoices-api-openapi.yml
  format: yaml
  label: DrillerDB Invoices API
  slug: drillerdb-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-invoices-api-openapi.yml
- filename: drillerdb-com-platform-api-openapi.yml
  format: yaml
  label: DrillerDB Platform API
  slug: drillerdb-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-platform-api-openapi.yml
- filename: drillerdb-com-projects-api-openapi.yml
  format: yaml
  label: DrillerDB Projects API
  slug: drillerdb-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-projects-api-openapi.yml
- filename: drillerdb-com-well-data-api-openapi.yml
  format: yaml
  label: DrillerDB Well data API
  slug: drillerdb-com-well-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-well-data-api-openapi.yml
- filename: drillerdb-com-work-orders-api-openapi.yml
  format: yaml
  label: DrillerDB Work Orders API
  slug: drillerdb-com-work-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-work-orders-api-openapi.yml
authorization_urls:
- https://enterprise.drillerdb.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Drillerdb Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DrillerDB publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DrillerDB API on a user''s behalf.


  Tokens are issued from https://enterprise.drillerdb.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DrillerDB
provider_slug: drillerdb-com
schemes:
- description: 'OAuth 2.1 authorization-code flow with PKCE (S256), as published at https://enterprise.drillerdb.com/.well-known/oauth-authorization-server. Dynamic client registration is available at https://enterprise.drillerdb.com/oauth/register. Tokens are presented as Bearer in the Authorization header. Protected-resource metadata (RFC 9728): https://enterprise.drillerdb.com/.well-known/oauth-protected-resource.'
  flows:
  - authorizationUrl: https://enterprise.drillerdb.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://enterprise.drillerdb.com/oauth/token
  name: EnterpriseMcpOAuth
  source: openapi/drillerdb-com-openapi.json
scope_count: 1
scope_names:
- mcp:read:enterprise
scopes:
- description: Read drilling-company prospect data, lead scores, lists, territories, and market signals on the user's behalf (read-only).
  flows:
  - authorizationCode
  scope: mcp:read:enterprise
slug: drillerdb-com-scopes
source_filename: drillerdb-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/drillerdb-com-openapi.json\nschemes:\n- name: EnterpriseMcpOAuth\n  source: openapi/drillerdb-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://enterprise.drillerdb.com/oauth/authorize\n    tokenUrl: https://enterprise.drillerdb.com/oauth/token\n  description: 'OAuth 2.1 authorization-code flow with PKCE (S256), as published at https://enterprise.drillerdb.com/.well-known/oauth-authorization-server.\n    Dynamic client registration is available at https://enterprise.drillerdb.com/oauth/register.\n    Tokens are presented as Bearer in the Authorization header. Protected-resource metadata\n    (RFC 9728): https://enterprise.drillerdb.com/.well-known/oauth-protected-resource.'\nscopes:\n- scope: mcp:read:enterprise\n  description: Read drilling-company prospect data, lead scores, lists, territories, and market\n    signals on the user's behalf (read-only).\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/drillerdb-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/drillerdb-com/scopes/drillerdb-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Water Well
- DrillingSoftware
- PumpService
- Project Management
- Software-as-a-Service
token_bound: false
token_urls:
- https://enterprise.drillerdb.com/oauth/token
---
