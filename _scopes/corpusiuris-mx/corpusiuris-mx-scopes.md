---
api_specs:
- filename: corpusiuris-mx-agent-api-openapi.yml
  format: yaml
  label: Corpus Iuris Agent API
  slug: corpusiuris-mx-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiuris-mx/openapi/corpusiuris-mx-agent-api-openapi.yml
authorization_urls: []
description: ''
docs: https://corpusiuris.mx/agentes
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Corpus Iuris Scopes
name_suffix: OAuth Scopes
note: Scopes come from the MCP server's OAuth authorization-server metadata (HTTP 200, scopes_supported). The REST OpenAPI declares only a bearer scheme; descriptions are not published.
overview: 'Corpus Iuris publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Corpus Iuris API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Corpus Iuris
provider_slug: corpusiuris-mx
schemes: []
scope_count: 2
scope_names:
- search
- perfil
scopes:
- description: ''
  flows: []
  scope: search
- description: ''
  flows: []
  scope: perfil
slug: corpusiuris-mx-scopes
source_filename: corpusiuris-mx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://api.corpusiuris.mx/.well-known/oauth-authorization-server\ndocs: https://corpusiuris.mx/agentes\nnote: Scopes come from the MCP server's OAuth authorization-server metadata (HTTP 200, scopes_supported). The REST OpenAPI declares only a bearer scheme; descriptions are not published.\nscopes:\n- name: search\n  applies_to: https://api.corpusiuris.mx/mcp\n- name: perfil\n  applies_to: https://api.corpusiuris.mx/mcp\n"
source_yaml_url: https://artifacts.apis.io/corpusiuris-mx/scopes/corpusiuris-mx-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Legal
- Legal Research
- Artificial Intelligence
- Mexico
- Jurisprudence
- MCP
- Search
token_bound: false
token_urls: []
---
