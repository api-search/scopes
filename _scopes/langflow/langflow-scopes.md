---
authorization_urls: []
description: ''
docs: https://docs.langflow.org/api-keys-and-authentication
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Langflow Scopes
name_suffix: OAuth Scopes
note: Langflow does not publish OAuth scopes — API access is authorized via API keys that adopt the privileges of the creating user (superuser vs regular user roles), not scope-based permissions (https://docs.langflow.org/api-keys-and-authentication).
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
  source: openapi/langflow-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: langflow-scopes
source_filename: langflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/langflow-openapi.yml\ndocs: https://docs.langflow.org/api-keys-and-authentication\nnote: >-\n  Langflow does not publish OAuth scopes — API access is authorized via API keys that\n  adopt the privileges of the creating user (superuser vs regular user roles), not\n  scope-based permissions (https://docs.langflow.org/api-keys-and-authentication).\nschemes:\n- name: OAuth2PasswordBearerCookie\n  source: openapi/langflow-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: api/v1/login\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/scopes/langflow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI
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
token_urls:
- api/v1/login
---
