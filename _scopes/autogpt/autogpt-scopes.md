---
api_specs:
- filename: autogpt-external-api-openapi.json
  format: json
  label: AutoGPT External API
  slug: autogpt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/openapi/autogpt-external-api-openapi.json
- filename: autogpt-agent-server-openapi.json
  format: json
  label: AutoGPT Agent Server API
  slug: autogpt-agent-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/openapi/autogpt-agent-server-openapi.json
authorization_urls: []
description: 'The ten OAuth 2.0 scopes AutoGPT Platform publishes for third-party applications. NOTE ON PROVENANCE: these are read from the AutoGPT docs, NOT from the OpenAPI. The authorization server at https://backend.agpt.co/api/oauth/* declares no oauth2 securityScheme and no scopes[] in either published spec — every protected operation is documented as plain HTTP bearer — so derive-oauth-scopes.py found nothing and this file is entirely docs-sourced. That gap is the finding: an agent reading the contract cannot discover the permission model.'
docs: https://agpt.co/docs/platform/api-and-integrations/api-guide.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Autogpt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AutoGPT uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AutoGPT
provider_slug: autogpt
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: autogpt-scopes
source_filename: autogpt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://agpt.co/docs/platform/api-and-integrations/api-guide.md\ndocs: https://agpt.co/docs/platform/api-and-integrations/api-guide.md\noauth_guide: https://agpt.co/docs/platform/api-and-integrations/oauth-guide.md\ndescription: >-\n  The ten OAuth 2.0 scopes AutoGPT Platform publishes for third-party\n  applications. NOTE ON PROVENANCE: these are read from the AutoGPT docs, NOT\n  from the OpenAPI. The authorization server at\n  https://backend.agpt.co/api/oauth/* declares no oauth2 securityScheme and no\n  scopes[] in either published spec — every protected operation is documented as\n  plain HTTP bearer — so derive-oauth-scopes.py found nothing and this file is\n  entirely docs-sourced. That gap is the finding: an agent reading the contract\n  cannot discover the permission model.\nauthorization_endpoint: https://platform.agpt.co/auth/authorize\ntoken_endpoint: https://backend.agpt.co/api/oauth/token\nintrospection_endpoint:\
  \ https://backend.agpt.co/api/oauth/introspect\nrevocation_endpoint: https://backend.agpt.co/api/oauth/revoke\nflow: authorization_code\npkce:\n  required: true\n  method: S256\nscope_delimiter: space\ntoken_prefix: agpt_xt_\nregistration: >-\n  No self-service OAuth app registration. The docs say to \"contact the platform\n  administrator\" to obtain a client_id, client_secret and registered redirect\n  URIs. There is a /api/oauth/apps/mine surface in the platform API, but app\n  creation is not documented as public.\nscopes:\n  - name: IDENTITY\n    description: Read user ID, e-mail, and timezone.\n    use: \"Sign in with AutoGPT / SSO.\"\n  - name: EXECUTE_GRAPH\n    description: Run agents.\n  - name: READ_GRAPH\n    description: Read agent run results.\n  - name: EXECUTE_BLOCK\n    description: Run individual blocks.\n  - name: READ_BLOCK\n    description: Read block definitions.\n  - name: READ_STORE\n    description: Access the agent store.\n  - name: USE_TOOLS\n    description:\
  \ Use platform tools.\n  - name: MANAGE_INTEGRATIONS\n    description: Create and update user integrations.\n  - name: READ_INTEGRATIONS\n    description: Read user integration status.\n  - name: DELETE_INTEGRATIONS\n    description: Remove user integrations.\nscope_count: 10\ngaps:\n  - >-\n    No securitySchemes.oauth2 block in either OpenAPI, so no per-operation scope\n    requirement is machine-readable. A client cannot compute which scopes an\n    operation needs.\n  - >-\n    No RFC 8414 metadata document at\n    https://backend.agpt.co/.well-known/oauth-authorization-server (404 probed\n    2026-08-29).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/scopes/autogpt-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI Agents
- AI Automation
- Agent Platform
- Workflow Automation
- Model Context Protocol
- Open Source
- No-Code
- LLM Orchestration
- Agent Marketplace
token_urls: []
---
