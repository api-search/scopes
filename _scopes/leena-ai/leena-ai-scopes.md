---
api_specs:
- filename: leena-ai-analytics-api-openapi.yml
  format: yaml
  label: Leena AI Analytics API
  slug: leena-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-analytics-api-openapi.yml
- filename: leena-ai-aop-api-openapi.yml
  format: yaml
  label: Leena AI AOP API
  slug: leena-ai-aop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-aop-api-openapi.yml
- filename: leena-ai-audit-logs-api-openapi.yml
  format: yaml
  label: Leena AI Audit Logs API
  slug: leena-ai-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-audit-logs-api-openapi.yml
- filename: leena-ai-authentication-api-openapi.yml
  format: yaml
  label: Leena AI Authentication API
  slug: leena-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-authentication-api-openapi.yml
- filename: leena-ai-knowledge-articles-api-openapi.yml
  format: yaml
  label: Leena AI Knowledge Articles API
  slug: leena-ai-knowledge-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/openapi/leena-ai-knowledge-articles-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.leena.ai/docs/audit-logs-external-api-authentication-usage-guide-beta
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Leena Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Leena AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Leena AI
provider_slug: leena-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: leena-ai-scopes
source_filename: leena-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\ndocs: https://docs.leena.ai/docs/audit-logs-external-api-authentication-usage-guide-beta\nsource: https://docs.leena.ai/docs/audit-logs-external-api-authentication-usage-guide-beta\nsummary: >-\n  Leena AI's external APIs are OAuth 2.0 protected and the documentation names one concrete\n  scope. Leena AI does not publish a consolidated scope reference page, so only the scope\n  it documents explicitly is recorded here. Insufficient scope is signalled as HTTP 401\n  with the message \"Insufficient OAuth scope\" rather than the more usual 403.\noauth_flow: password\ntoken_endpoint: 'https://<region-code>-acl.leena.ai/api/v1.0/oauth/token'\nscopes:\n  - name: audit-logs:read\n    description: Read audit log records via GET /external/v1/audit-logs.\n    api: openapi/leena-ai-audit-logs-openapi.yml\n    operations:\n      - listAuditLogs\n    source: https://docs.leena.ai/docs/audit-logs-external-api-authentication-usage-guide-beta\nnaming_convention:\n\
  \  pattern: '<resource>:<action>'\n  observed:\n    - audit-logs:read\n  note: >-\n    Only one scope is publicly documented. The External AOP API returns 403 \"insufficient\n    scope\" on its execute and status operations, implying additional scopes exist, but\n    Leena AI does not publish their names — they are deliberately not guessed here.\nenforcement:\n  insufficient_scope_status: 401\n  insufficient_scope_message: Insufficient OAuth scope\ngaps:\n  - No public consolidated OAuth scope / permissions reference page.\n  - AOP execute and status scope names are not published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leena-ai/refs/heads/main/scopes/leena-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Ai Ml
- Agentic AI
- Artificial Intelligence
- Enterprise Software
- Human Resources
- ITSM
- Employee Experience
- Workflow-Automation
- Conversational AI
- MCP
- Knowledge-Management
token_urls: []
---
