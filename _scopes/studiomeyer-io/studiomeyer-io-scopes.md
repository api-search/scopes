---
api_specs:
- filename: studiomeyer-io-account-api-openapi.yml
  format: yaml
  label: studiomeyer-io Account API
  slug: studiomeyer-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-account-api-openapi.yml
- filename: studiomeyer-io-backfill-api-openapi.yml
  format: yaml
  label: studiomeyer-io Backfill API
  slug: studiomeyer-io-backfill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-backfill-api-openapi.yml
- filename: studiomeyer-io-case-study-api-openapi.yml
  format: yaml
  label: studiomeyer-io Case Study API
  slug: studiomeyer-io-case-study-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-case-study-api-openapi.yml
- filename: studiomeyer-io-consultation-api-openapi.yml
  format: yaml
  label: studiomeyer-io Consultation API
  slug: studiomeyer-io-consultation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-consultation-api-openapi.yml
- filename: studiomeyer-io-decide-api-openapi.yml
  format: yaml
  label: studiomeyer-io Decide API
  slug: studiomeyer-io-decide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-decide-api-openapi.yml
- filename: studiomeyer-io-docs-api-openapi.yml
  format: yaml
  label: studiomeyer-io Docs API
  slug: studiomeyer-io-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-docs-api-openapi.yml
- filename: studiomeyer-io-entity-api-openapi.yml
  format: yaml
  label: studiomeyer-io Entity API
  slug: studiomeyer-io-entity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-entity-api-openapi.yml
- filename: studiomeyer-io-export-api-openapi.yml
  format: yaml
  label: studiomeyer-io Export API
  slug: studiomeyer-io-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-export-api-openapi.yml
- filename: studiomeyer-io-generate-agents-json-api-openapi.yml
  format: yaml
  label: studiomeyer-io Generate Agents Json API
  slug: studiomeyer-io-generate-agents-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-generate-agents-json-api-openapi.yml
- filename: studiomeyer-io-learn-api-openapi.yml
  format: yaml
  label: studiomeyer-io Learn API
  slug: studiomeyer-io-learn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-learn-api-openapi.yml
- filename: studiomeyer-io-memory-api-openapi.yml
  format: yaml
  label: studiomeyer-io Memory API
  slug: studiomeyer-io-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-memory-api-openapi.yml
- filename: studiomeyer-io-portfolio-api-openapi.yml
  format: yaml
  label: studiomeyer-io Portfolio API
  slug: studiomeyer-io-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-portfolio-api-openapi.yml
- filename: studiomeyer-io-quote-api-openapi.yml
  format: yaml
  label: studiomeyer-io Quote API
  slug: studiomeyer-io-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-quote-api-openapi.yml
- filename: studiomeyer-io-search-api-openapi.yml
  format: yaml
  label: studiomeyer-io Search API
  slug: studiomeyer-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-search-api-openapi.yml
- filename: studiomeyer-io-services-api-openapi.yml
  format: yaml
  label: studiomeyer-io Services API
  slug: studiomeyer-io-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-services-api-openapi.yml
- filename: studiomeyer-io-studiomeyer-memory-rest-api-api-openapi.yml
  format: yaml
  label: studiomeyer-io StudioMeyer Memory REST API
  slug: studiomeyer-io-studiomeyer-memory-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-studiomeyer-memory-rest-api-api-openapi.yml
- filename: studiomeyer-io-validate-webmcp-api-openapi.yml
  format: yaml
  label: studiomeyer-io Validate Webmcp API
  slug: studiomeyer-io-validate-webmcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/studiomeyer-io/openapi/studiomeyer-io-validate-webmcp-api-openapi.yml
authorization_urls:
- https://memory.studiomeyer.io/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Studiomeyer Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'studiomeyer-io publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the studiomeyer-io API on a user''s behalf.


  Tokens are issued from https://memory.studiomeyer.io/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: studiomeyer-io
provider_slug: studiomeyer-io
schemes:
- description: OAuth 2.1 authorization code with PKCE (S256). The memory scope grants full account access; separate read/write permissions are not implemented.
  flows:
  - authorizationUrl: https://memory.studiomeyer.io/authorize
    flow: authorizationCode
    tokenUrl: https://memory.studiomeyer.io/token
  name: oauth2
  source: openapi/memory-openapi.json
scope_count: 1
scope_names:
- memory
scopes:
- description: Full access to the authenticated account memory operations.
  flows:
  - authorizationCode
  scope: memory
slug: studiomeyer-io-scopes
source_filename: studiomeyer-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/memory-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/memory-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://memory.studiomeyer.io/authorize\n    tokenUrl: https://memory.studiomeyer.io/token\n  description: OAuth 2.1 authorization code with PKCE (S256). The memory scope grants full account\n    access; separate read/write permissions are not implemented.\nscopes:\n- scope: memory\n  description: Full access to the authenticated account memory operations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/memory-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/studiomeyer-io/scopes/studiomeyer-io-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- Web Design
- MCP
- Mallorca
token_bound: false
token_urls:
- https://memory.studiomeyer.io/token
---
