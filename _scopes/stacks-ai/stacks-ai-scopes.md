---
api_specs:
- filename: stacks-ai-analytics-api-openapi.yml
  format: yaml
  label: Stacks Ai Analytics API
  slug: stacks-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-analytics-api-openapi.yml
- filename: stacks-ai-knowledge-base-resources-api-openapi.yml
  format: yaml
  label: Stacks Ai Knowledge Base Resources API
  slug: stacks-ai-knowledge-base-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-knowledge-base-resources-api-openapi.yml
- filename: stacks-ai-knowledge-base-sync-api-openapi.yml
  format: yaml
  label: Stacks Ai Knowledge Base Sync API
  slug: stacks-ai-knowledge-base-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-knowledge-base-sync-api-openapi.yml
- filename: stacks-ai-knowledge-bases-api-openapi.yml
  format: yaml
  label: Stacks Ai Knowledge Bases API
  slug: stacks-ai-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-knowledge-bases-api-openapi.yml
- filename: stacks-ai-run-flow-api-openapi.yml
  format: yaml
  label: Stacks Ai Run Flow API
  slug: stacks-ai-run-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-run-flow-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Stacks Ai Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Stacks Ai uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stacks Ai
provider_slug: stacks-ai
schemes:
- description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).
  flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/stacks-ai-analytics-api-openapi.yml
- description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).
  flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/stacks-ai-knowledge-base-resources-api-openapi.yml
- description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).
  flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/stacks-ai-knowledge-base-sync-api-openapi.yml
- description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).
  flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/stacks-ai-knowledge-bases-api-openapi.yml
- description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).
  flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/stacks-ai-run-flow-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: stacks-ai-scopes
source_filename: stacks-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/stacks-ai-analytics-api-openapi.yml, openapi/stacks-ai-knowledge-base-resources-api-openapi.yml,\n  openapi/stacks-ai-knowledge-base-sync-api-openapi.yml, openapi/stacks-ai-knowledge-bases-api-openapi.yml,\n  openapi/stacks-ai-run-flow-api-openapi.yml\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/stacks-ai-analytics-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n  description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).\n- name: OAuth2PasswordBearer\n  source: openapi/stacks-ai-knowledge-base-resources-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n  description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).\n- name: OAuth2PasswordBearer\n  source: openapi/stacks-ai-knowledge-base-sync-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n  description: Authorization\
  \ header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).\n- name: OAuth2PasswordBearer\n  source: openapi/stacks-ai-knowledge-bases-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n  description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).\n- name: OAuth2PasswordBearer\n  source: openapi/stacks-ai-run-flow-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: token\n  description: Authorization header. [Learn how to get it](/docs/api-reference/how-to-get-credentials).\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/scopes/stacks-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Artificial Intelligence
- Agents
- LLM
- No-Code
- Automation
- Workflows
- RAG
- Knowledge Base
- Enterprise
token_bound: false
token_urls:
- token
---
