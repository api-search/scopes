---
authorization_urls:
- https://api.chalk.ai/v1/oauth/authorize
description: ''
docs: https://docs.chalk.ai/docs/online-authentication
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Chalk Scopes
name_suffix: OAuth Scopes
note: Programmatic feature access via client_credentials does not use a documented scope surface; fine-grained control is enforced through service-token RBAC tags (see authentication/chalk-authentication.yml), not OAuth scopes. The scopes above are the published OAuth/MCP scopes.
overview: 'Chalk publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Chalk API on a user''s behalf.


  Tokens are issued from https://api.chalk.ai/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chalk
provider_slug: chalk
schemes:
- flows:
  - authorizationUrl: https://api.chalk.ai/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.chalk.ai/v1/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.chalk.ai/v1/oauth/token
  name: OAuth2
  source: https://api.chalk.ai/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- openid
- mcp:read
- mcp:write
scopes:
- description: OpenID Connect authentication scope (openid-configuration discovery).
  flows:
  - authorizationCode
  scope: openid
- description: Read access for Model Context Protocol (MCP) clients.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access for Model Context Protocol (MCP) clients.
  flows:
  - authorizationCode
  scope: mcp:write
slug: chalk-scopes
source_filename: chalk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.chalk.ai/.well-known/oauth-authorization-server\ndocs: https://docs.chalk.ai/docs/online-authentication\nschemes:\n- name: OAuth2\n  source: https://api.chalk.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.chalk.ai/v1/oauth/authorize\n    tokenUrl: https://api.chalk.ai/v1/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.chalk.ai/v1/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication scope (openid-configuration discovery).\n  flows: [authorizationCode]\n  sources: [well-known/chalk-openid-configuration.json]\n- scope: mcp:read\n  description: Read access for Model Context Protocol (MCP) clients.\n  flows: [authorizationCode]\n  sources: [well-known/chalk-oauth-authorization-server.json]\n- scope: mcp:write\n  description: Write access for Model Context Protocol (MCP) clients.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/chalk-oauth-authorization-server.json]\nnote: >-\n  Programmatic feature access via client_credentials does not use a documented scope surface;\n  fine-grained control is enforced through service-token RBAC tags (see authentication/chalk-authentication.yml),\n  not OAuth scopes. The scopes above are the published OAuth/MCP scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chalk/refs/heads/main/scopes/chalk-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Machine Learning
- Feature Store
- Artificial Intelligence
- Data Platform
- MLOps
- Real-Time Data
- LLM
- Agents
- Feature Engineering
token_urls:
- https://api.chalk.ai/v1/oauth/token
---
