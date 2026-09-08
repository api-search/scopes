---
api_specs:
- filename: worklittle-job-boards-api-openapi.yml
  format: yaml
  label: Worklittle Job Boards API
  slug: worklittle-job-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-job-boards-api-openapi.yml
- filename: worklittle-jobs-api-openapi.yml
  format: yaml
  label: Worklittle Jobs API
  slug: worklittle-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-jobs-api-openapi.yml
- filename: worklittle-platform-api-openapi.yml
  format: yaml
  label: Worklittle Business Platform API
  slug: worklittle-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/openapi/worklittle-platform-api-openapi.yml
authorization_urls:
- https://api.worklittle.com/oauth/authorize
description: ''
docs: https://docs.worklittle.com/jobs/get-started/api-keys
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Worklittle Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only bearer keys, but the provider both documents key scopes and serves RFC 8414 authorization-server metadata (saved at well-known/worklittle-oauth-authorization-server.json) used for MCP Connect OAuth. Scope list below is the union of the discovery document's scopes_supported and the scope tables on the API-keys and pricing docs pages.
overview: 'Worklittle publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Worklittle API on a user''s behalf.


  Tokens are issued from https://api.worklittle.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Worklittle
provider_slug: worklittle
schemes:
- flows:
  - authorizationUrl: https://api.worklittle.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.worklittle.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.worklittle.com
  name: OAuth2 (MCP Connect)
  pkce:
  - S256
  registration_endpoint: https://api.worklittle.com/oauth/register
  source: well-known/worklittle-oauth-authorization-server.json
- name: bearerAuth (API keys)
  note: sk-wl-api01- prefixed keys; scopes attached per key.
  source: openapi/worklittle-jobs-api-openapi.yml
scope_count: 11
scope_names:
- jobs:read
- jobs:apply
- jobs:apply_with_ai
- jobs:post
- jobs:applications
- webhooks:manage
- agent:tools
- people:read
- openid
- email
- profile
scopes:
- description: GET /jobs, GET /jobs/:id, GET /jobs/map, GET /jobs/stats, GET /account; MCP search/read tools.
  flows: []
  scope: jobs:read
- description: POST /jobs/:id/apply and MCP submit_job_application.
  flows: []
  scope: jobs:apply
- description: Apply-with-AI sessions via MCP Connect OAuth.
  flows: []
  scope: jobs:apply_with_ai
- description: Post and manage job listings (/business/jobs, /jobs/manage).
  flows: []
  scope: jobs:post
- description: ATS candidate, employee, offer, email-template and organization routes.
  flows: []
  scope: jobs:applications
- description: /webhooks CRUD and delivery log.
  flows: []
  scope: webhooks:manage
- description: POST /jobs/resumes, POST /jobs/cover-letters, POST /v1/agent/tool.
  flows: []
  scope: agent:tools
- description: Reserved — public People Search is temporarily unavailable (410 GONE).
  flows: []
  scope: people:read
- description: OIDC identity scope on the MCP Connect authorization server.
  flows: []
  scope: openid
- description: OIDC email scope on the MCP Connect authorization server.
  flows: []
  scope: email
- description: OIDC profile scope on the MCP Connect authorization server.
  flows: []
  scope: profile
slug: worklittle-scopes
source_filename: worklittle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://api.worklittle.com/.well-known/oauth-authorization-server\ndocs: https://docs.worklittle.com/jobs/get-started/api-keys\nnote: >-\n  The OpenAPI declares only bearer keys, but the provider both documents key scopes and serves\n  RFC 8414 authorization-server metadata (saved at well-known/worklittle-oauth-authorization-server.json)\n  used for MCP Connect OAuth. Scope list below is the union of the discovery document's\n  scopes_supported and the scope tables on the API-keys and pricing docs pages.\nschemes:\n- name: OAuth2 (MCP Connect)\n  source: well-known/worklittle-oauth-authorization-server.json\n  issuer: https://api.worklittle.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.worklittle.com/oauth/authorize\n    tokenUrl: https://api.worklittle.com/oauth/token\n  registration_endpoint: https://api.worklittle.com/oauth/register\n  pkce: [S256]\n  grant_types: [authorization_code, refresh_token]\n\
  - name: bearerAuth (API keys)\n  source: openapi/worklittle-jobs-api-openapi.yml\n  note: sk-wl-api01- prefixed keys; scopes attached per key.\nscopes:\n- scope: jobs:read\n  description: \"GET /jobs, GET /jobs/:id, GET /jobs/map, GET /jobs/stats, GET /account; MCP search/read tools.\"\n  sources: [oauth-authorization-server, docs api-keys]\n- scope: jobs:apply\n  description: \"POST /jobs/:id/apply and MCP submit_job_application.\"\n  sources: [oauth-authorization-server, docs api-keys]\n- scope: jobs:apply_with_ai\n  description: Apply-with-AI sessions via MCP Connect OAuth.\n  sources: [oauth-authorization-server]\n- scope: jobs:post\n  description: \"Post and manage job listings (/business/jobs, /jobs/manage).\"\n  sources: [docs pricing]\n- scope: jobs:applications\n  description: \"ATS candidate, employee, offer, email-template and organization routes.\"\n  sources: [docs pricing]\n- scope: webhooks:manage\n  description: \"/webhooks CRUD and delivery log.\"\n  sources: [docs pricing]\n\
  - scope: agent:tools\n  description: \"POST /jobs/resumes, POST /jobs/cover-letters, POST /v1/agent/tool.\"\n  sources: [docs api-keys]\n- scope: people:read\n  description: Reserved — public People Search is temporarily unavailable (410 GONE).\n  sources: [docs api-keys]\n- scope: openid\n  description: OIDC identity scope on the MCP Connect authorization server.\n  sources: [oauth-authorization-server]\n- scope: email\n  description: OIDC email scope on the MCP Connect authorization server.\n  sources: [oauth-authorization-server]\n- scope: profile\n  description: OIDC profile scope on the MCP Connect authorization server.\n  sources: [oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worklittle/refs/heads/main/scopes/worklittle-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Job Search
- ATS
- Recruiting
- Workforce Intelligence
- Job Boards
- Webhooks
- MCP
token_urls:
- https://api.worklittle.com/oauth/token
---
