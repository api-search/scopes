---
authorization_urls: []
description: ''
docs: https://help.tellius.com/kaiya/tellius-mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Tellius Scopes
name_suffix: OAuth Scopes
note: Read from the RFC 8414 authorization server metadata a Tellius deployment serves anonymously, probed 2026-08-30 (HTTP 200). Tellius publishes no scope reference page and no OpenAPI securitySchemes, so this metadata document is the only machine-readable statement of the scope surface. It declares exactly ONE scope. The derive-oauth-scopes.py baseline was not runnable here because there is no OpenAPI in the repo to derive from.
overview: 'Tellius publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tellius API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tellius
provider_slug: tellius
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to the Tellius MCP server at /mcp. Declared in both the authorization server metadata (scopes_supported) and the RFC 9728 protected resource metadata for the resource https://{tellius-deployment-host}/mcp.
  flows: []
  scope: mcp
slug: tellius-scopes
source_filename: tellius-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://qa1.dev.tellius.com/.well-known/oauth-authorization-server\ndocs: https://help.tellius.com/kaiya/tellius-mcp-server\nname: Tellius OAuth scopes\nnote: 'Read from the RFC 8414 authorization server metadata a Tellius deployment\n  serves anonymously, probed 2026-08-30 (HTTP 200). Tellius publishes no scope\n  reference page and no OpenAPI securitySchemes, so this metadata document is the\n  only machine-readable statement of the scope surface. It declares exactly ONE\n  scope. The derive-oauth-scopes.py baseline was not runnable here because there is\n  no OpenAPI in the repo to derive from.'\nauthorization_server: https://{tellius-deployment-host}\nendpoints:\n  authorization: https://{tellius-deployment-host}/oauth/authorize\n  token: https://{tellius-deployment-host}/oauth/token\n  registration: https://{tellius-deployment-host}/oauth/register\n  client_credentials_token: https://{tellius-deployment-host}/oauth/client_credentials_token\n\
  \  refresh_token: https://{tellius-deployment-host}/oauth/refresh_token\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\nresponse_types_supported:\n- code\ncode_challenge_methods_supported:\n- S256\ntoken_endpoint_auth_methods_supported:\n- none\n- client_secret_post\ndynamic_client_registration: true\nscope_count: 1\nscopes:\n- scope: mcp\n  description: 'Access to the Tellius MCP server at /mcp. Declared in both the\n    authorization server metadata (scopes_supported) and the RFC 9728 protected\n    resource metadata for the resource https://{tellius-deployment-host}/mcp.'\n  resource: https://{tellius-deployment-host}/mcp\n  method: probed\n  source: https://qa1.dev.tellius.com/.well-known/oauth-protected-resource\nfindings:\n- 'Tellius does NOT decompose MCP access into per-capability scopes. A single \"mcp\"\n  scope covers all 25 tools, including the two the docs themselves mark Destructive\n  (tellius_delete_workflow, tellius_delete_schedule).\
  \ An agent granted the scope to\n  ask a question is granted the scope to permanently delete a schedule.'\n- 'Authorization is instead enforced downstream: every MCP request runs as a specific\n  Tellius user, and Business View permissions plus row-level security apply to that\n  user. That is real governance, but it is user-level, not token-level — the token\n  itself carries no least-privilege boundary.'\n- 'The ML Model REST endpoints use OAuth2 client_credentials with no scope parameter\n  documented at all.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tellius/refs/heads/main/scopes/tellius-scopes.yml
summary_line: 1 scope
tags:
- Company
- Analytics
- Business Intelligence
- Agentic Analytics
- Decision Intelligence
- Artificial Intelligence
- Machine-Learning
- Data
- Embedded Analytics
- MCP
- Natural Language Query
- Pharmaceuticals
- Consumer Packaged Goods
- Financial Planning
token_urls: []
---
