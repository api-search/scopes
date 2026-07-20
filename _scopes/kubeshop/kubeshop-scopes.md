---
api_specs:
- filename: kubeshop-testkube-control-plane-openapi-original.yml
  format: yaml
  label: Testkube Control Plane API
  slug: testkube-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeshop/refs/heads/main/openapi/kubeshop-testkube-control-plane-openapi-original.yml
- filename: kubeshop-testkube-agent-openapi-original.yml
  format: yaml
  label: Testkube Standalone Agent API
  slug: testkube-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeshop/refs/heads/main/openapi/kubeshop-testkube-agent-openapi-original.yml
- filename: kubeshop-testkube-openapi-original.yml
  format: yaml
  label: Testkube API (open source)
  slug: testkube-oss
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubeshop/refs/heads/main/openapi/kubeshop-testkube-openapi-original.yml
authorization_urls:
- https://api.testkube.io/mcp/auth/authorize
description: ''
docs: https://docs.testkube.io/articles/mcp-security
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kubeshop Scopes
name_suffix: OAuth Scopes
note: Testkube's three published OpenAPI documents declare no oauth2 security scheme — the REST surface is bearer-token authenticated (see authentication/). The only OAuth scope surface Testkube publishes is the OAuth 2.1 authorization server fronting the MCP endpoint, discovered live at /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource. Those scopes are recorded here verbatim.
overview: 'Kubeshop publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kubeshop API on a user''s behalf.


  Tokens are issued from https://api.testkube.io/mcp/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kubeshop
provider_slug: kubeshop
schemes:
- applies_to: https://api.testkube.io/mcp
  flows:
  - authorizationUrl: https://api.testkube.io/mcp/auth/authorize
    flow: authorizationCode
    pkce: S256
    refresh_token: true
    registrationUrl: https://api.testkube.io/mcp/auth/register
    revocationUrl: https://api.testkube.io/mcp/auth/revoke
    tokenUrl: https://api.testkube.io/mcp/auth/token
  issuer: https://api.testkube.io
  name: TestkubeMCPOAuth
  source: https://api.testkube.io/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp:full
scopes:
- description: Full access to the Testkube MCP endpoint for the authorized organization and environment. This is the only scope the authorization server advertises; Testkube does not currently publish a finer-grained scope breakdown.
  flows:
  - authorizationCode
  scope: mcp:full
slug: kubeshop-scopes
source_filename: kubeshop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.testkube.io/.well-known/oauth-authorization-server\ndocs: https://docs.testkube.io/articles/mcp-security\nnote: >-\n  Testkube's three published OpenAPI documents declare no oauth2 security scheme — the\n  REST surface is bearer-token authenticated (see authentication/). The only OAuth\n  scope surface Testkube publishes is the OAuth 2.1 authorization server fronting the\n  MCP endpoint, discovered live at /.well-known/oauth-authorization-server and\n  /.well-known/oauth-protected-resource. Those scopes are recorded here verbatim.\nschemes:\n- name: TestkubeMCPOAuth\n  source: https://api.testkube.io/.well-known/oauth-authorization-server\n  issuer: https://api.testkube.io\n  applies_to: https://api.testkube.io/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.testkube.io/mcp/auth/authorize\n    tokenUrl: https://api.testkube.io/mcp/auth/token\n    revocationUrl: https://api.testkube.io/mcp/auth/revoke\n\
  \    registrationUrl: https://api.testkube.io/mcp/auth/register\n    pkce: S256\n    refresh_token: true\nscopes:\n- scope: mcp:full\n  description: >-\n    Full access to the Testkube MCP endpoint for the authorized organization and\n    environment. This is the only scope the authorization server advertises; Testkube\n    does not currently publish a finer-grained scope breakdown.\n  flows: [authorizationCode]\n  sources:\n  - https://api.testkube.io/.well-known/oauth-authorization-server\n  - https://api.testkube.io/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubeshop/refs/heads/main/scopes/kubeshop-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Testing
- Kubernetes
- Continuous Integration
- Developer Tools
- Test Automation
- Observability
- DevOps
- Cloud Native
- Quality Assurance
- Open Source
- Model Context Protocol
token_urls:
- https://api.testkube.io/mcp/auth/token
---
