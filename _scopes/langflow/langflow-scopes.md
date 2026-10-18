---
api_specs:
- filename: langflow-base-api-openapi.yml
  format: yaml
  label: Langflow Base API
  slug: langflow-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-base-api-openapi.yml
- filename: langflow-chat-api-openapi.yml
  format: yaml
  label: Langflow Chat API
  slug: langflow-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-chat-api-openapi.yml
- filename: langflow-files-api-openapi.yml
  format: yaml
  label: Langflow Files API
  slug: langflow-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-files-api-openapi.yml
- filename: langflow-flow-events-api-openapi.yml
  format: yaml
  label: Langflow Flow Events API
  slug: langflow-flow-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-flow-events-api-openapi.yml
- filename: langflow-flows-api-openapi.yml
  format: yaml
  label: Langflow Flows API
  slug: langflow-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-flows-api-openapi.yml
- filename: langflow-health-check-api-openapi.yml
  format: yaml
  label: Langflow Health Check API
  slug: langflow-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-health-check-api-openapi.yml
- filename: langflow-log-api-openapi.yml
  format: yaml
  label: Langflow Log API
  slug: langflow-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-log-api-openapi.yml
- filename: langflow-mcp-api-openapi.yml
  format: yaml
  label: Langflow MCP API
  slug: langflow-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-mcp-api-openapi.yml
- filename: langflow-mcp-projects-api-openapi.yml
  format: yaml
  label: Langflow MCP Projects API
  slug: langflow-mcp-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-mcp-projects-api-openapi.yml
- filename: langflow-monitor-api-openapi.yml
  format: yaml
  label: Langflow Monitor API
  slug: langflow-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-monitor-api-openapi.yml
- filename: langflow-openai-responses-api-api-openapi.yml
  format: yaml
  label: Langflow OpenAI Responses API
  slug: langflow-openai-responses-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openai-responses-api-api-openapi.yml
- filename: langflow-projects-api-openapi.yml
  format: yaml
  label: Langflow Projects API
  slug: langflow-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-projects-api-openapi.yml
- filename: langflow-traces-api-openapi.yml
  format: yaml
  label: Langflow Traces API
  slug: langflow-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-traces-api-openapi.yml
- filename: langflow-users-api-openapi.yml
  format: yaml
  label: Langflow Users API
  slug: langflow-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-users-api-openapi.yml
- filename: langflow-workflow-api-openapi.yml
  format: yaml
  label: Langflow Workflow API
  slug: langflow-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-workflow-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Langflow Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Langflow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from api/v1/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Langflow
provider_slug: langflow
schemes:
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-base-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-chat-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-files-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-flow-events-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-flows-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-health-check-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-log-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-mcp-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-mcp-projects-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-monitor-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-openai-responses-api-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-projects-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-traces-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-users-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: api/v1/login
  name: OAuth2PasswordBearerCookie
  source: openapi/langflow-workflow-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: langflow-scopes
source_filename: langflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/langflow-base-api-openapi.yml, openapi/langflow-chat-api-openapi.yml, openapi/langflow-files-api-openapi.yml,\n  openapi/langflow-flow-events-api-openapi.yml, openapi/langflow-flows-api-openapi.yml, openapi/langflow-health-check-api-openapi.yml,\n  openapi/langflow-log-api-openapi.yml, openapi/langflow-mcp-api-openapi.yml, openapi/langflow-mcp-projects-api-openapi.yml,\n  openapi/langflow-monitor-api-openapi.yml, openapi/langflow-openai-responses-api-api-openapi.yml,\n  openapi/langflow-projects-api-openapi.yml, openapi/langflow-traces-api-openapi.yml, openapi/langflow-users-api-openapi.yml,\n  openapi/langflow-workflow-api-openapi.yml\nschemes:\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-base-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-chat-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n\
  - name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-files-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-flow-events-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-flows-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-health-check-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-log-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-mcp-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-mcp-projects-api-openapi.yml\n  flows:\n  - flow: password\n   \
  \ tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-monitor-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-openai-responses-api-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-projects-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-traces-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-users-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-workflow-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and\
  \ no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/scopes/langflow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Agents
- Workflows
- Low-Code
- Visual Builder
- LangChain
- RAG
- MCP
- Open Source
- FastAPI
token_bound: false
token_urls:
- api/v1/login
---
