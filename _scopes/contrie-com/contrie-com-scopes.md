---
api_specs:
- filename: contrie-com-account-api-openapi.yml
  format: yaml
  label: Contrie Account API
  slug: contrie-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-account-api-openapi.yml
- filename: contrie-com-evidence-api-openapi.yml
  format: yaml
  label: Contrie Evidence API
  slug: contrie-com-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-evidence-api-openapi.yml
- filename: contrie-com-extract-api-openapi.yml
  format: yaml
  label: Contrie Extract API
  slug: contrie-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-extract-api-openapi.yml
- filename: contrie-com-health-api-openapi.yml
  format: yaml
  label: Contrie Health API
  slug: contrie-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-health-api-openapi.yml
- filename: contrie-com-mcp-api-openapi.yml
  format: yaml
  label: Contrie MCP API
  slug: contrie-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-mcp-api-openapi.yml
- filename: contrie-com-monitors-api-openapi.yml
  format: yaml
  label: Contrie Monitors API
  slug: contrie-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-monitors-api-openapi.yml
- filename: contrie-com-scrape-api-openapi.yml
  format: yaml
  label: Contrie Scrape API
  slug: contrie-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-scrape-api-openapi.yml
- filename: contrie-com-search-api-openapi.yml
  format: yaml
  label: Contrie Search API
  slug: contrie-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-search-api-openapi.yml
- filename: contrie-com-verification-api-openapi.yml
  format: yaml
  label: Contrie Verification API
  slug: contrie-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-verification-api-openapi.yml
- filename: contrie-com-verify-api-openapi.yml
  format: yaml
  label: Contrie Verify API
  slug: contrie-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contrie-com/openapi/contrie-com-verify-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.contrie.com/docs/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Contrie Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only an http bearer scheme; OAuth scopes are documented for the hosted MCP sign-in flow.
overview: 'Contrie publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Contrie API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Contrie
provider_slug: contrie-com
schemes: []
scope_count: 2
scope_names:
- contrie:account
- offline_access
scopes:
- description: That permission grants extraction, verification and monitor access on the same terms as an account API key. Profile and email scopes alone do not grant account access.
  flows: []
  scope: contrie:account
- description: Requested alongside contrie:account in the documented Codex CLI login command (codex mcp login contrie --scopes contrie:account,offline_access).
  flows: []
  scope: offline_access
slug: contrie-com-scopes
source_filename: contrie-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.contrie.com/docs/authentication\ndocs: https://www.contrie.com/docs/authentication\nnote: The OpenAPI declares only an http bearer scheme; OAuth scopes are documented for the hosted MCP sign-in flow.\nscopes:\n- name: contrie:account\n  description: That permission grants extraction, verification and monitor access on the same terms as an account API key. Profile and email scopes alone do not grant account access.\n  source: https://www.contrie.com/docs/authentication\n- name: offline_access\n  description: Requested alongside contrie:account in the documented Codex CLI login command (codex mcp login contrie --scopes contrie:account,offline_access).\n  source: https://www.contrie.com/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/contrie-com/scopes/contrie-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Web Scraping
- Data Extraction
- AI Agents
- MCP
- Structured Data
- Markdown
token_bound: false
token_urls: []
---
