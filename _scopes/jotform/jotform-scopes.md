---
api_specs:
- filename: jotform-folder-api-openapi.yml
  format: yaml
  label: Jotform Folder API
  slug: jotform-folder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-folder-api-openapi.yml
- filename: jotform-form-api-openapi.yml
  format: yaml
  label: Jotform Form API
  slug: jotform-form-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-form-api-openapi.yml
- filename: jotform-label-api-openapi.yml
  format: yaml
  label: Jotform Label API
  slug: jotform-label-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-label-api-openapi.yml
- filename: jotform-report-api-openapi.yml
  format: yaml
  label: Jotform Report API
  slug: jotform-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-report-api-openapi.yml
- filename: jotform-submission-api-openapi.yml
  format: yaml
  label: Jotform Submission API
  slug: jotform-submission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-submission-api-openapi.yml
- filename: jotform-system-api-openapi.yml
  format: yaml
  label: Jotform System API
  slug: jotform-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-system-api-openapi.yml
- filename: jotform-user-api-openapi.yml
  format: yaml
  label: Jotform User API
  slug: jotform-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-user-api-openapi.yml
- filename: jotform-webhook-api-openapi.yml
  format: yaml
  label: Jotform Webhook API
  slug: jotform-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-webhook-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.jotform.com/developers/mcp/?tab=mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Jotform Scopes
name_suffix: OAuth Scopes
note: 'Scope descriptions are not published; the names are read from the served authorization-server metadata and the MCP docs (Scopes: readOnly, full).'
overview: 'Jotform publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jotform API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jotform
provider_slug: jotform
schemes: []
scope_count: 2
scope_names:
- readOnly
- full
scopes:
- description: Read-only access to the connected user's Jotform account (scope name as published in scopes_supported; the JavaScript SDK uses the same accessType value).
  flows: []
  scope: readOnly
- description: Full access to the connected user's Jotform account (scope name as published in scopes_supported).
  flows: []
  scope: full
slug: jotform-scopes
source_filename: jotform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://mcp.jotform.com/.well-known/oauth-authorization-server\n- https://mcp.jotform.com/.well-known/oauth-protected-resource\n- https://www.jotform.com/developers/mcp/?tab=mcp\ndocs: https://www.jotform.com/developers/mcp/?tab=mcp\nissuer: https://oauth2.jotform.com\napplies_to: Jotform MCP servers (https://mcp.jotform.com); the REST API uses API keys, not OAuth scopes\nscopes:\n- name: readOnly\n  description: Read-only access to the connected user's Jotform account (scope name as published in scopes_supported;\n    the JavaScript SDK uses the same accessType value).\n  source: https://mcp.jotform.com/.well-known/oauth-authorization-server\n- name: full\n  description: Full access to the connected user's Jotform account (scope name as published in scopes_supported).\n  source: https://mcp.jotform.com/.well-known/oauth-authorization-server\nnote: 'Scope descriptions are not published; the names are read from the served\
  \ authorization-server metadata and\n  the MCP docs (Scopes: readOnly, full).'\n"
source_yaml_url: https://artifacts.apis.io/jotform/scopes/jotform-scopes.yml
summary_line: 2 scopes
tags:
- Forms
- Surveys
- No-Code
- Data Collection
- Workflows
- HIPAA
- EU
- MCP
- E-Signature
- Webhook
- Online Payments
token_bound: false
token_urls: []
---
