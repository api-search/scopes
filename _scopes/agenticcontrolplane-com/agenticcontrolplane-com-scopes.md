---
api_specs:
- filename: agenticcontrolplane-com-agents-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Agents API
  slug: agenticcontrolplane-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-agents-api-openapi.yml
- filename: agenticcontrolplane-com-credentials-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Credentials API
  slug: agenticcontrolplane-com-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-credentials-api-openapi.yml
- filename: agenticcontrolplane-com-delegation-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Delegation API
  slug: agenticcontrolplane-com-delegation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-delegation-api-openapi.yml
- filename: agenticcontrolplane-com-introspect-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Introspect API
  slug: agenticcontrolplane-com-introspect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-introspect-api-openapi.yml
- filename: agenticcontrolplane-com-mcp-api-openapi.yml
  format: yaml
  label: Agentic Control Plane MCP API
  slug: agenticcontrolplane-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-mcp-api-openapi.yml
- filename: agenticcontrolplane-com-meta-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Meta API
  slug: agenticcontrolplane-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-meta-api-openapi.yml
- filename: agenticcontrolplane-com-proxy-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Proxy API
  slug: agenticcontrolplane-com-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-proxy-api-openapi.yml
- filename: agenticcontrolplane-com-runs-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Runs API
  slug: agenticcontrolplane-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-runs-api-openapi.yml
- filename: agenticcontrolplane-com-sandbox-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Sandbox API
  slug: agenticcontrolplane-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-sandbox-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Agenticcontrolplane Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agentic Control Plane publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agentic Control Plane API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agentic Control Plane
provider_slug: agenticcontrolplane-com
schemes: []
scope_count: 4
scope_names:
- '*'
- admin.audit.read
- agents.write
- agents.read
scopes:
- description: Everything — full read/write across agents and governance.
  flows: []
  scope: '*'
- description: Read the audit log.
  flows: []
  scope: admin.audit.read
- description: Create and modify agent profiles.
  flows: []
  scope: agents.write
- description: List and read agent profiles.
  flows: []
  scope: agents.read
slug: agenticcontrolplane-com-scopes
source_filename: agenticcontrolplane-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://agenticcontrolplane.com/docs/api/authentication.md\nscopes:\n  - name: \"*\"\n    description: \"Everything — full read/write across agents and governance.\"\n  - name: \"admin.audit.read\"\n    description: \"Read the audit log.\"\n  - name: \"agents.write\"\n    description: \"Create and modify agent profiles.\"\n  - name: \"agents.read\"\n    description: \"List and read agent profiles.\"\n"
source_yaml_url: https://artifacts.apis.io/agenticcontrolplane-com/scopes/agenticcontrolplane-com-scopes.yml
summary_line: 4 scopes
tags:
- Artificial Intelligence
- Agents
- Control Plane
- Tool Management
- Monitoring
token_bound: false
token_urls: []
---
