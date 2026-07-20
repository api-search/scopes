---
api_specs:
- filename: celonis-knowledge-model-openapi.yaml
  format: yaml
  label: Celonis Knowledge Model API
  slug: celonis-knowledge-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-knowledge-model-openapi.yaml
- filename: celonis-agents-ai-openapi.yaml
  format: yaml
  label: Celonis AI Agent API
  slug: celonis-ai-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-agents-ai-openapi.yaml
- filename: celonis-subscription-openapi.yaml
  format: yaml
  label: Celonis Event Subscription API
  slug: celonis-event-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-subscription-openapi.yaml
- filename: celonis-mlwb-openapi.yaml
  format: yaml
  label: Celonis Machine Learning Workbench API
  slug: celonis-machine-learning-workbench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-mlwb-openapi.yaml
- filename: celonis-team-openapi.yaml
  format: yaml
  label: Celonis Team API
  slug: celonis-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-team-openapi.yaml
- filename: celonis-permissions-openapi.yaml
  format: yaml
  label: Celonis Permissions API
  slug: celonis-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-permissions-openapi.yaml
- filename: celonis-mcp-tool-calling-openapi.yaml
  format: yaml
  label: Celonis Agent Tools (MCP) Tool Calling API
  slug: celonis-agent-tools-mcp-tool-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-mcp-tool-calling-openapi.yaml
authorization_urls: []
description: ''
docs: https://developer.celonis.com/celonis-apis/audit-log-api/overview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Celonis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Celonis publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Celonis API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Celonis
provider_slug: celonis
schemes: []
scope_count: 2
scope_names:
- audit.log:read
- audit.log
scopes:
- description: Read-only access to the Audit Log API.
  flows:
  - clientCredentials
  - authorizationCode
  scope: audit.log:read
- description: Access to the Audit Log API (audit.log family).
  flows:
  - clientCredentials
  - authorizationCode
  scope: audit.log
slug: celonis-scopes
source_filename: celonis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.celonis.com/celonis-apis/oauth-authentication/\ndocs: https://developer.celonis.com/celonis-apis/audit-log-api/overview\nmodel: >-\n  Celonis OAuth 2.0 uses scopes to gate which APIs an OAuth client may reach. A client\n  can only access an API if it holds BOTH the OAuth scope and the matching Celonis\n  permission. With the client-credentials grant, the requested scopes are passed in the\n  space-separated `scope` parameter of the token request. The full scope catalog is\n  published inside the authenticated Celonis Platform docs (docs.celonis.com is\n  login-gated); the entries below are the scopes confirmed on public developer pages.\ngrant_types:\n- clientCredentials\n- authorizationCode\ntoken_url: https://{team_domain}.{realm}.celonis.cloud/oauth2/token\nscopes:\n- scope: audit.log:read\n  description: Read-only access to the Audit Log API.\n  flows: [clientCredentials, authorizationCode]\n  source:\
  \ https://developer.celonis.com/celonis-apis/audit-log-api/overview\n- scope: audit.log\n  description: Access to the Audit Log API (audit.log family).\n  flows: [clientCredentials, authorizationCode]\n  source: https://developer.celonis.com/celonis-apis/audit-log-api/overview\ncaveat: >-\n  The complete OAuth scope reference (intelligence / integration / machine-learning\n  families, etc.) is behind the authenticated docs.celonis.com portal and was not\n  captured verbatim to avoid fabrication; only publicly confirmed scopes are listed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/scopes/celonis-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Automation
- Process Mining
- Process Intelligence
- Data
- Analytics
- Machine Learning
- AI Agents
- Enterprise
token_urls: []
---
