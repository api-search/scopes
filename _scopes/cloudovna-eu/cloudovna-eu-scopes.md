---
api_specs:
- filename: cloudovna-eu-catalog-api-openapi.yml
  format: yaml
  label: Cloudovňa Catalog API
  slug: cloudovna-eu-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-catalog-api-openapi.yml
- filename: cloudovna-eu-health-api-openapi.yml
  format: yaml
  label: Cloudovňa Health API
  slug: cloudovna-eu-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-health-api-openapi.yml
- filename: cloudovna-eu-hooks-api-openapi.yml
  format: yaml
  label: Cloudovňa Hooks API
  slug: cloudovna-eu-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-hooks-api-openapi.yml
- filename: cloudovna-eu-images-api-openapi.yml
  format: yaml
  label: Cloudovňa Images API
  slug: cloudovna-eu-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-images-api-openapi.yml
- filename: cloudovna-eu-integrations-api-openapi.yml
  format: yaml
  label: Cloudovňa Integrations API
  slug: cloudovna-eu-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-integrations-api-openapi.yml
- filename: cloudovna-eu-invitations-api-openapi.yml
  format: yaml
  label: Cloudovňa Invitations API
  slug: cloudovna-eu-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-invitations-api-openapi.yml
- filename: cloudovna-eu-invoices-api-openapi.yml
  format: yaml
  label: Cloudovňa Invoices API
  slug: cloudovna-eu-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-invoices-api-openapi.yml
- filename: cloudovna-eu-mcp-api-openapi.yml
  format: yaml
  label: Cloudovňa MCP API
  slug: cloudovna-eu-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-mcp-api-openapi.yml
- filename: cloudovna-eu-oauth-api-openapi.yml
  format: yaml
  label: Cloudovňa OAuth API
  slug: cloudovna-eu-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-oauth-api-openapi.yml
- filename: cloudovna-eu-organizations-api-openapi.yml
  format: yaml
  label: Cloudovňa Organizations API
  slug: cloudovna-eu-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-organizations-api-openapi.yml
- filename: cloudovna-eu-payments-api-openapi.yml
  format: yaml
  label: Cloudovňa Payments API
  slug: cloudovna-eu-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-payments-api-openapi.yml
- filename: cloudovna-eu-pool-api-openapi.yml
  format: yaml
  label: Cloudovňa Pool API
  slug: cloudovna-eu-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-pool-api-openapi.yml
- filename: cloudovna-eu-public-api-openapi.yml
  format: yaml
  label: Cloudovňa Public API
  slug: cloudovna-eu-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-public-api-openapi.yml
- filename: cloudovna-eu-services-api-openapi.yml
  format: yaml
  label: Cloudovňa Services API
  slug: cloudovna-eu-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-services-api-openapi.yml
- filename: cloudovna-eu-stacks-api-openapi.yml
  format: yaml
  label: Cloudovňa Stacks API
  slug: cloudovna-eu-stacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-stacks-api-openapi.yml
- filename: cloudovna-eu-well-known-api-openapi.yml
  format: yaml
  label: Cloudovňa .well Known API
  slug: cloudovna-eu-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-well-known-api-openapi.yml
authorization_urls: []
description: ''
docs: https://cloudovna.eu/docs/api.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cloudovňa Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only http bearer; OAuth scopes apply to the MCP server and mirror the personal-token access levels. scopes_supported read via GET (HTTP 200) from both well-known metadata documents.
overview: 'Cloudovňa publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cloudovňa API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cloudovňa
provider_slug: cloudovna-eu
schemes: []
scope_count: 2
scope_names:
- read
- manage
scopes:
- description: Every GET (services, resource pool, logs, domains, databases, payments, invoices) and POST /api/pool/check, which changes nothing; every change is refused.
  flows: []
  scope: read
- description: Everything read can, plus ordering, resizing and splitting the pool, configuring, deploying, domains, database logins and backups.
  flows: []
  scope: manage
slug: cloudovna-eu-scopes
source_filename: cloudovna-eu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://admin.cloudovna.eu/.well-known/oauth-protected-resource/mcp\ndocs: https://cloudovna.eu/docs/api.md\nnote: The OpenAPI declares only http bearer; OAuth scopes apply to the MCP server and mirror the personal-token access levels. scopes_supported read via GET (HTTP 200) from both well-known metadata documents.\nscopes:\n- name: read\n  description: Every GET (services, resource pool, logs, domains, databases, payments, invoices) and POST /api/pool/check, which changes nothing; every change is refused.\n- name: manage\n  description: Everything read can, plus ordering, resizing and splitting the pool, configuring, deploying, domains, database logins and backups.\n"
source_yaml_url: https://artifacts.apis.io/cloudovna-eu/scopes/cloudovna-eu-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Cloud Hosting
- Containers
- Docker
- Database
- PostgreSQL
- SQL Server
- European Union
- MCP
token_bound: false
token_urls: []
---
