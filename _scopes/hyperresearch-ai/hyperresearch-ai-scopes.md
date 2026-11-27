---
api_specs:
- filename: hyperresearch-ai-account-api-openapi.yml
  format: yaml
  label: Hyperresearch Account API
  slug: hyperresearch-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-account-api-openapi.yml
- filename: hyperresearch-ai-agent-connections-api-openapi.yml
  format: yaml
  label: Hyperresearch agent connections API
  slug: hyperresearch-ai-agent-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-agent-connections-api-openapi.yml
- filename: hyperresearch-ai-answers-api-openapi.yml
  format: yaml
  label: Hyperresearch Answers API
  slug: hyperresearch-ai-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-answers-api-openapi.yml
- filename: hyperresearch-ai-auth-api-openapi.yml
  format: yaml
  label: Hyperresearch Auth API
  slug: hyperresearch-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-auth-api-openapi.yml
- filename: hyperresearch-ai-billing-api-openapi.yml
  format: yaml
  label: Hyperresearch Billing API
  slug: hyperresearch-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-billing-api-openapi.yml
- filename: hyperresearch-ai-demo-api-openapi.yml
  format: yaml
  label: Hyperresearch Demo API
  slug: hyperresearch-ai-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-demo-api-openapi.yml
- filename: hyperresearch-ai-keys-api-openapi.yml
  format: yaml
  label: Hyperresearch Keys API
  slug: hyperresearch-ai-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-keys-api-openapi.yml
- filename: hyperresearch-ai-meta-api-openapi.yml
  format: yaml
  label: Hyperresearch Meta API
  slug: hyperresearch-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-meta-api-openapi.yml
- filename: hyperresearch-ai-projects-api-openapi.yml
  format: yaml
  label: Hyperresearch Projects API
  slug: hyperresearch-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-projects-api-openapi.yml
- filename: hyperresearch-ai-runs-api-openapi.yml
  format: yaml
  label: Hyperresearch Runs API
  slug: hyperresearch-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-runs-api-openapi.yml
- filename: hyperresearch-ai-scholar-api-openapi.yml
  format: yaml
  label: Hyperresearch Scholar API
  slug: hyperresearch-ai-scholar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-scholar-api-openapi.yml
- filename: hyperresearch-ai-usage-api-openapi.yml
  format: yaml
  label: Hyperresearch Usage API
  slug: hyperresearch-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-usage-api-openapi.yml
- filename: hyperresearch-ai-vault-api-openapi.yml
  format: yaml
  label: Hyperresearch Vault API
  slug: hyperresearch-ai-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-vault-api-openapi.yml
- filename: hyperresearch-ai-verify-api-openapi.yml
  format: yaml
  label: Hyperresearch Verify API
  slug: hyperresearch-ai-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-verify-api-openapi.yml
- filename: hyperresearch-ai-webhooks-api-openapi.yml
  format: yaml
  label: Hyperresearch Webhooks API
  slug: hyperresearch-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-webhooks-api-openapi.yml
- filename: hyperresearch-ai-workspaces-api-openapi.yml
  format: yaml
  label: Hyperresearch Workspaces API
  slug: hyperresearch-ai-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-workspaces-api-openapi.yml
authorization_urls:
- https://api.hyperresearch.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hyperresearch Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hyperresearch publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hyperresearch API on a user''s behalf.


  Tokens are issued from https://api.hyperresearch.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hyperresearch
provider_slug: hyperresearch-ai
schemes:
- description: 'OAuth 2.1 for agents (MCP clients): authorization code with PKCE (S256), public clients, dynamic client registration at `https://api.hyperresearch.ai/oauth/register`, discovery at `https://api.hyperresearch.ai/.well-known/oauth-authorization-server`. Access tokens (15 min) and rotating refresh tokens (30 days) are bound to the resource `https://mcp.hyperresearch.ai/mcp` and are accepted by the hosted MCP server, not by the REST operations in this document, which take an API key (`bearerAuth`). A member can only delegate scopes their workspace role holds; the token response reports the granted `scope`.'
  flows:
  - authorizationUrl: https://api.hyperresearch.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hyperresearch.ai/oauth/token
  name: oauth2
  source: openapi/hyperresearch-ai-openapi.json
scope_count: 8
scope_names:
- answers:ask
- fetch
- mcp
- runs:read
- runs:write
- vault:read
- vault:write
- verify
scopes:
- description: 'Answers: `ask` and `search` calls billed per call from the prepaid wallet, plus reading the wallet balance (billable).'
  flows:
  - authorizationCode
  scope: answers:ask
- description: Fetch a URL into the vault on the workspace’s budget (billable; OAuth grants only, checked against the member’s role).
  flows:
  - authorizationCode
  scope: fetch
- description: Connect to the hosted MCP server; every OAuth grant carries it.
  flows:
  - authorizationCode
  scope: mcp
- description: 'Read runs: status, event stream, results, reports and artifacts.'
  flows:
  - authorizationCode
  scope: runs:read
- description: Start, clarify, pause, resume, abort and re-run research runs (billable).
  flows:
  - authorizationCode
  scope: runs:write
- description: 'Read and search the workspace vault: notes, claims, sources, hubs, escalations, scholar lookups.'
  flows:
  - authorizationCode
  scope: vault:read
- description: 'Write to the workspace vault: create/update/delete notes, ingest claims, import, resolve escalations.'
  flows:
  - authorizationCode
  scope: vault:write
- description: Run citation, quote, retraction and independence verification jobs and read their results (billable).
  flows:
  - authorizationCode
  scope: verify
slug: hyperresearch-ai-scopes
source_filename: hyperresearch-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/hyperresearch-ai-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/hyperresearch-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.hyperresearch.ai/oauth/authorize\n    tokenUrl: https://api.hyperresearch.ai/oauth/token\n  description: 'OAuth 2.1 for agents (MCP clients): authorization code with PKCE (S256), public\n    clients, dynamic client registration at `https://api.hyperresearch.ai/oauth/register`, discovery\n    at `https://api.hyperresearch.ai/.well-known/oauth-authorization-server`. Access tokens\n    (15 min) and rotating refresh tokens (30 days) are bound to the resource `https://mcp.hyperresearch.ai/mcp`\n    and are accepted by the hosted MCP server, not by the REST operations in this document,\n    which take an API key (`bearerAuth`). A member can only delegate scopes their workspace\n    role holds; the token response reports the granted `scope`.'\nscopes:\n\
  - scope: answers:ask\n  description: 'Answers: `ask` and `search` calls billed per call from the prepaid wallet, plus\n    reading the wallet balance (billable).'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hyperresearch-ai-openapi.json\n- scope: fetch\n  description: Fetch a URL into the vault on the workspace’s budget (billable; OAuth grants\n    only, checked against the member’s role).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hyperresearch-ai-openapi.json\n- scope: mcp\n  description: Connect to the hosted MCP server; every OAuth grant carries it.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hyperresearch-ai-openapi.json\n- scope: runs:read\n  description: 'Read runs: status, event stream, results, reports and artifacts.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hyperresearch-ai-openapi.json\n- scope: runs:write\n  description: Start, clarify, pause, resume, abort and re-run research runs (billable).\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/hyperresearch-ai-openapi.json\n- scope: vault:read\n  description: 'Read and search the workspace vault: notes, claims, sources, hubs, escalations,\n    scholar lookups.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hyperresearch-ai-openapi.json\n- scope: vault:write\n  description: 'Write to the workspace vault: create/update/delete notes, ingest claims, import,\n    resolve escalations.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hyperresearch-ai-openapi.json\n- scope: verify\n  description: Run citation, quote, retraction and independence verification jobs and read their\n    results (billable).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hyperresearch-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hyperresearch-ai/scopes/hyperresearch-ai-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Artificial Intelligence
- Search
- Research
- Data
token_bound: false
token_urls:
- https://api.hyperresearch.ai/oauth/token
---
