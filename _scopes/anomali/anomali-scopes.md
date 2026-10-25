---
api_specs:
- filename: anomali-openapi-generated.yml
  format: yaml
  label: Anomali API
  slug: anomali-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomali/refs/heads/main/openapi/_ae-authored/anomali-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Anomali Scopes
name_suffix: OAuth Scopes
note: Scope names published only as scopes_supported in the protected-resource document; no descriptions are published.
overview: 'Anomali publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Anomali API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Anomali
provider_slug: anomali
schemes: []
scope_count: 6
scope_names:
- MCP_ENRICHMENTS_ACCESS
- MCP_READ_PIR_DATA
- MCP_READ_TS_DATA
- MCP_SA_ACCESS
- MCP_WRITE_PIR_DATA
- MCP_WRITE_TS_DATA
scopes:
- description: ''
  flows: []
  scope: MCP_ENRICHMENTS_ACCESS
- description: ''
  flows: []
  scope: MCP_READ_PIR_DATA
- description: ''
  flows: []
  scope: MCP_READ_TS_DATA
- description: ''
  flows: []
  scope: MCP_SA_ACCESS
- description: ''
  flows: []
  scope: MCP_WRITE_PIR_DATA
- description: ''
  flows: []
  scope: MCP_WRITE_TS_DATA
slug: anomali-scopes
source_filename: anomali-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'name: Anomali OAuth scopes

  generated: ''2026-10-20''

  method: probed

  source: https://api.threatstream.com/.well-known/oauth-protected-resource

  scopes:

  - {name: MCP_ENRICHMENTS_ACCESS, resource: https://api.threatstream.com/mcp}

  - {name: MCP_READ_PIR_DATA, resource: https://api.threatstream.com/mcp}

  - {name: MCP_READ_TS_DATA, resource: https://api.threatstream.com/mcp}

  - {name: MCP_SA_ACCESS, resource: https://api.threatstream.com/mcp}

  - {name: MCP_WRITE_PIR_DATA, resource: https://api.threatstream.com/mcp}

  - {name: MCP_WRITE_TS_DATA, resource: https://api.threatstream.com/mcp}

  note: Scope names published only as scopes_supported in the protected-resource document; no descriptions are published.

  '
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anomali/refs/heads/main/scopes/anomali-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Enterprise
- Cybersecurity
- Threat Intelligence
- Security
- SIEM
- SOAR
- XDR
- Threat Intelligence Platform
token_bound: false
token_urls: []
---
