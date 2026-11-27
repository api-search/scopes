---
api_specs:
- filename: contracko-com-authentication-api-openapi.yml
  format: yaml
  label: Contracko Authentication API
  slug: contracko-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-authentication-api-openapi.yml
- filename: contracko-com-contract-types-api-openapi.yml
  format: yaml
  label: Contracko Contract Types API
  slug: contracko-com-contract-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-contract-types-api-openapi.yml
- filename: contracko-com-parsing-api-api-openapi.yml
  format: yaml
  label: Contracko Parsing API
  slug: contracko-com-parsing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-parsing-api-api-openapi.yml
authorization_urls: []
description: ''
docs: https://contracko.com/api/developers/llms.txt
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Contracko Scopes
name_suffix: OAuth Scopes
note: Contracko does not declare oauth2 in its OpenAPI; these are API-key scopes named in the published API reference and changelog (v1 0.3.0, 2026-10-22). The key's granted scopes are returned by GET /health. The MCP server's OAuth grant uses separate Read and Write permissions (https://contracko.com/docs/mcp-server).
overview: 'Contracko publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Contracko API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Contracko
provider_slug: contracko-com
schemes: []
scope_count: 3
scope_names:
- parser:compute
- contract:write
- contract:intake
scopes:
- description: Parser key scope. "`parser:compute` alone can still list, get, create and update extraction schemas, but cannot delete them."
  flows: []
  scope: parser:compute
- description: Contract Management (CLM) write scope; required with active Contract Management API access to delete contract types.
  flows: []
  scope: contract:write
- description: Legacy alias accepted in place of contract:write.
  flows: []
  scope: contract:intake
slug: contracko-com-scopes
source_filename: contracko-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://contracko.com/api/developers/llms.txt\ndocs: https://contracko.com/api/developers/llms.txt\nnote: Contracko does not declare oauth2 in its OpenAPI; these are API-key scopes named in the published API reference and changelog (v1 0.3.0, 2026-10-22). The key's granted scopes are returned by GET /health. The MCP server's OAuth grant uses separate Read and Write permissions (https://contracko.com/docs/mcp-server).\nscopes:\n- name: parser:compute\n  description: Parser key scope. \"`parser:compute` alone can still list, get, create and update extraction schemas, but cannot delete them.\"\n  applies_to: [contractTypes.list, contractTypes.get, contractTypes.create, contractTypes.update]\n- name: contract:write\n  description: Contract Management (CLM) write scope; required with active Contract Management API access to delete contract types.\n  applies_to: [contractTypes.delete]\n- name: contract:intake\n  description: Legacy\
  \ alias accepted in place of contract:write.\n  deprecated: true\n  applies_to: [contractTypes.delete]\n"
source_yaml_url: https://artifacts.apis.io/contracko-com/scopes/contracko-com-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Contract Management
- Legal Tech
- Artificial Intelligence
- Document Parsing
- Data Extraction
- E-Signature
- MCP
token_bound: false
token_urls: []
---
