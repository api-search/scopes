---
authorization_urls: []
description: ''
docs: https://www.getnoded.ai/developers
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Noded Ai Scopes
name_suffix: OAuth Scopes
note: 'Noded publishes no scope/permission reference page. The only scopes visible in public are the OIDC scopes the first-party SDK requests by default against the Noded Auth0 tenant — these are standard OpenID Connect scopes, not Noded-specific API permissions. Authorization in Noded is expressed as tenant + per-user permissions enforced server-side (and, on the MCP layer, as per-agent tool scoping), not as named OAuth scopes a developer selects. Derivation from an OpenAPI was not possible: Noded publishes no OpenAPI. Recorded as an honest partial.'
overview: 'Noded AI publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Noded AI API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Noded AI
provider_slug: noded-ai
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Requests an ID token for the signed-in Noded user.
  flows: []
  scope: openid
- description: Basic profile claims for the signed-in Noded user.
  flows: []
  scope: profile
- description: Email claim for the signed-in Noded user.
  flows: []
  scope: email
- description: Refresh token so the SDK can silently refresh without re-prompting.
  flows: []
  scope: offline_access
slug: noded-ai-scopes
source_filename: noded-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.getnoded.ai/developers\ndocs: https://www.getnoded.ai/developers\nnote: >-\n  Noded publishes no scope/permission reference page. The only scopes visible in public are the\n  OIDC scopes the first-party SDK requests by default against the Noded Auth0 tenant — these are\n  standard OpenID Connect scopes, not Noded-specific API permissions. Authorization in Noded is\n  expressed as tenant + per-user permissions enforced server-side (and, on the MCP layer, as\n  per-agent tool scoping), not as named OAuth scopes a developer selects. Derivation from an\n  OpenAPI was not possible: Noded publishes no OpenAPI. Recorded as an honest partial.\nissuer: https://login.getnoded.ai/\naudience: provisioned per customer (the Noded API audience)\nscopes:\n  - scope: openid\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Requests an ID token for the signed-in Noded user.\n  - scope: profile\n    standard:\
  \ true\n    spec: OpenID Connect Core 1.0\n    description: Basic profile claims for the signed-in Noded user.\n  - scope: email\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Email claim for the signed-in Noded user.\n  - scope: offline_access\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Refresh token so the SDK can silently refresh without re-prompting.\nscope_count: 4\nprovider_specific_scope_count: 0\nauthorization_model: >-\n  Tenant-scoped, permission-aware. Every call runs as the signed-in user and the API enforces\n  that user's permissions; the MCP layer additionally provisions tools per agent identity, so\n  what an agent may see is scoped to the agent rather than to the organization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noded-ai/refs/heads/main/scopes/noded-ai-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Ai Ml
- Customer Success
- Customer Data
- Churn
- Retention
- Revenue Operations
- SaaS
- AI Agents
- GraphQL
- MCP
- Agent Native
- Customer Context Graph
token_urls: []
---
