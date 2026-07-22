---
authorization_urls: []
description: ''
docs: https://docs.opsera.io/api-platform-and-integration/opsera-api-platform/personal-access-tokens
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Opsera Scopes
name_suffix: OAuth Scopes
note: Opsera Personal Access Tokens carry a single predefined scope selected at creation time. The scope limits which family of APIs the token may call (a pipeline-scoped token can ONLY perform pipeline actions). Scope match is combined with the token owner's RBAC before access is granted; a mismatch or insufficient permission returns 403 Forbidden. These are token scopes on a JWT bearer model, not OAuth2 authorization flows.
overview: 'Opsera publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Opsera API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Opsera
provider_slug: opsera
schemes: []
scope_count: 2
scope_names:
- API Access
- Pipeline Access
scopes:
- description: General access required to call the Opsera platform APIs (e.g. pipeline run/status, MCP server).
  flows: []
  scope: API Access
- description: Permits pipeline actions such as triggering a run and reading run status.
  flows: []
  scope: Pipeline Access
slug: opsera-scopes
source_filename: opsera-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.opsera.io/api-platform-and-integration/opsera-api-platform\ndocs: https://docs.opsera.io/api-platform-and-integration/opsera-api-platform/personal-access-tokens\nmodel: personal-access-token-scopes\nnote: >-\n  Opsera Personal Access Tokens carry a single predefined scope selected at creation time. The\n  scope limits which family of APIs the token may call (a pipeline-scoped token can ONLY perform\n  pipeline actions). Scope match is combined with the token owner's RBAC before access is granted;\n  a mismatch or insufficient permission returns 403 Forbidden. These are token scopes on a JWT\n  bearer model, not OAuth2 authorization flows.\nscopes:\n  - scope: API Access\n    description: General access required to call the Opsera platform APIs (e.g. pipeline run/status, MCP server).\n    sources: [docs]\n  - scope: Pipeline Access\n    description: Permits pipeline actions such as triggering a run and reading run\
  \ status.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsera/refs/heads/main/scopes/opsera-scopes.yml
summary_line: 2 scopes
tags:
- Company
- DevOps
- CI/CD
- DevSecOps
- Pipeline Orchestration
- Developer Tools
- Software Delivery
- Governance
- MCP
- AI Agents
token_urls: []
---
