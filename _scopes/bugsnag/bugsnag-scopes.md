---
api_specs:
- filename: bugsnag-builds-api-openapi.yml
  format: yaml
  label: bugsnag Builds API
  slug: bugsnag-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-builds-api-openapi.yml
- filename: bugsnag-collaborators-api-openapi.yml
  format: yaml
  label: bugsnag Collaborators API
  slug: bugsnag-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-collaborators-api-openapi.yml
- filename: bugsnag-comments-api-openapi.yml
  format: yaml
  label: bugsnag Comments API
  slug: bugsnag-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-comments-api-openapi.yml
- filename: bugsnag-errors-api-openapi.yml
  format: yaml
  label: bugsnag Errors API
  slug: bugsnag-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-errors-api-openapi.yml
- filename: bugsnag-eventfields-api-openapi.yml
  format: yaml
  label: bugsnag EventFields API
  slug: bugsnag-eventfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-eventfields-api-openapi.yml
- filename: bugsnag-events-api-openapi.yml
  format: yaml
  label: bugsnag Events API
  slug: bugsnag-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-events-api-openapi.yml
- filename: bugsnag-organizations-api-openapi.yml
  format: yaml
  label: bugsnag Organizations API
  slug: bugsnag-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-organizations-api-openapi.yml
- filename: bugsnag-pivots-api-openapi.yml
  format: yaml
  label: bugsnag Pivots API
  slug: bugsnag-pivots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-pivots-api-openapi.yml
- filename: bugsnag-projects-api-openapi.yml
  format: yaml
  label: bugsnag Projects API
  slug: bugsnag-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-projects-api-openapi.yml
- filename: bugsnag-releases-api-openapi.yml
  format: yaml
  label: bugsnag Releases API
  slug: bugsnag-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-releases-api-openapi.yml
- filename: bugsnag-sessions-api-openapi.yml
  format: yaml
  label: bugsnag Sessions API
  slug: bugsnag-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-sessions-api-openapi.yml
- filename: bugsnag-stability-api-openapi.yml
  format: yaml
  label: bugsnag Stability API
  slug: bugsnag-stability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-stability-api-openapi.yml
- filename: bugsnag-traces-api-openapi.yml
  format: yaml
  label: bugsnag Traces API
  slug: bugsnag-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-traces-api-openapi.yml
- filename: bugsnag-trends-api-openapi.yml
  format: yaml
  label: bugsnag Trends API
  slug: bugsnag-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-trends-api-openapi.yml
- filename: bugsnag-current-user-api-openapi.yml
  format: yaml
  label: Bugsnag Current User API
  slug: bugsnag-current-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-current-user-api-openapi.yml
- filename: bugsnag-error-reporting-api-openapi.json
  format: json
  label: BugSnag Error Reporting API
  slug: bugsnag-error-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-error-reporting-api-openapi.json
- filename: bugsnag-upload-api-openapi.json
  format: json
  label: BugSnag Upload API
  slug: bugsnag-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-upload-api-openapi.json
authorization_urls: []
description: BugSnag's OAuth surface is the authorization server behind the remote MCP server (bugsnag.mcp.smartbear.com). The REST Data Access API itself does not use OAuth — it authenticates with a personal auth token (see authentication/bugsnag-authentication.yml). Scopes below are read verbatim from the RFC 8414 authorization-server metadata document, not inferred.
docs: https://developer.smartbear.com/smartbear-mcp/docs/remote-mcp-servers
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Bugsnag Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bugsnag uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bugsnag
provider_slug: bugsnag
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: bugsnag-scopes
source_filename: bugsnag-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: https://oauth.bugsnag.com/.well-known/oauth-authorization-server\ndocs: https://developer.smartbear.com/smartbear-mcp/docs/remote-mcp-servers\ndescription: >-\n  BugSnag's OAuth surface is the authorization server behind the remote MCP\n  server (bugsnag.mcp.smartbear.com). The REST Data Access API itself does not\n  use OAuth — it authenticates with a personal auth token (see\n  authentication/bugsnag-authentication.yml). Scopes below are read verbatim\n  from the RFC 8414 authorization-server metadata document, not inferred.\nauthorization_server: https://oauth.bugsnag.com\nissuer: https://oauth.bugsnag.com\nendpoints:\n  authorization: https://oauth.bugsnag.com/authorize\n  token: https://oauth.bugsnag.com/token\n  registration: https://oauth.bugsnag.com/register\n  jwks: https://oauth.bugsnag.com/.well-known/jwks.json\nflows:\n  - authorization_code\n  - refresh_token\npkce:\n  required_methods:\n    - S256\ndynamic_client_registration:\
  \ true\ntoken_endpoint_auth_methods:\n  - client_secret_post\n  - none\nscopes:\n  - name: api\n    description: >-\n      Access to the BugSnag API on behalf of the authenticated user. Declared in\n      scopes_supported; the provider publishes no per-resource breakdown of what\n      it covers, so no finer decomposition is recorded here.\n  - name: openid\n    description: OpenID Connect sign-in scope, requesting an ID token.\n  - name: profile\n    description: Standard OIDC profile claims for the authenticated user.\nscope_count: 3\nnotes:\n  - >-\n    scopes_supported is coarse — one `api` scope covers the whole surface. An\n    agent cannot request read-only access to BugSnag over OAuth today.\n  - >-\n    The authorization server advertises no /.well-known/openid-configuration\n    (404) despite supporting the openid scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/scopes/bugsnag-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Monitoring
- Observability
- Error Monitoring
- Application Performance Monitoring
- Distributed Tracing
- Developer Tools
- SmartBear
token_urls: []
---
