---
api_specs:
- filename: celonis-agents-conversation-api-openapi.yml
  format: yaml
  label: Celonis Agents - Conversation API
  slug: celonis-agents-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-agents-conversation-api-openapi.yml
- filename: celonis-beta-odata-protocol-api-openapi.yml
  format: yaml
  label: 'Celonis Beta: OData Protocol API'
  slug: celonis-beta-odata-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-beta-odata-protocol-api-openapi.yml
- filename: celonis-beta-semantics-for-3p-ai-agents-api-openapi.yml
  format: yaml
  label: 'Celonis Beta: Semantics for 3P AI Agents API'
  slug: celonis-beta-semantics-for-3p-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-beta-semantics-for-3p-ai-agents-api-openapi.yml
- filename: celonis-data-api-openapi.yml
  format: yaml
  label: Celonis Data API
  slug: celonis-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-data-api-openapi.yml
- filename: celonis-job-execution-api-openapi.yml
  format: yaml
  label: Celonis Job Execution API
  slug: celonis-job-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-job-execution-api-openapi.yml
- filename: celonis-job-execution-group-api-openapi.yml
  format: yaml
  label: Celonis Job Execution Group API
  slug: celonis-job-execution-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-job-execution-group-api-openapi.yml
- filename: celonis-login-history-api-api-openapi.yml
  format: yaml
  label: Celonis Login History API API
  slug: celonis-login-history-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-login-history-api-api-openapi.yml
- filename: celonis-members-api-api-openapi.yml
  format: yaml
  label: Celonis Members API API
  slug: celonis-members-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-members-api-api-openapi.yml
- filename: celonis-notebook-api-openapi.yml
  format: yaml
  label: Celonis Notebook API
  slug: celonis-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-notebook-api-openapi.yml
- filename: celonis-notebook-execution-api-openapi.yml
  format: yaml
  label: Celonis Notebook Execution API
  slug: celonis-notebook-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-notebook-execution-api-openapi.yml
- filename: celonis-notebook-resources-api-openapi.yml
  format: yaml
  label: Celonis Notebook Resources API
  slug: celonis-notebook-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-notebook-resources-api-openapi.yml
- filename: celonis-openapi-tool-calling-api-openapi.yml
  format: yaml
  label: Celonis OpenAPI Tool Calling API
  slug: celonis-openapi-tool-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-openapi-tool-calling-api-openapi.yml
- filename: celonis-permissions-export-api-api-openapi.yml
  format: yaml
  label: Celonis Permissions Export API API
  slug: celonis-permissions-export-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-permissions-export-api-api-openapi.yml
- filename: celonis-schedule-api-openapi.yml
  format: yaml
  label: Celonis Schedule API
  slug: celonis-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-schedule-api-openapi.yml
- filename: celonis-schema-api-openapi.yml
  format: yaml
  label: Celonis Schema API
  slug: celonis-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-schema-api-openapi.yml
- filename: celonis-subscriptions-api-openapi.yml
  format: yaml
  label: Celonis Subscriptions API
  slug: celonis-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-subscriptions-api-openapi.yml
- filename: celonis-triggers-api-openapi.yml
  format: yaml
  label: Celonis Triggers API
  slug: celonis-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celonis/refs/heads/main/openapi/celonis-triggers-api-openapi.yml
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
- Machine-Learning
- AI Agents
- Enterprise
token_urls: []
---
