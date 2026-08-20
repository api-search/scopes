---
api_specs:
- filename: ahrefs-openapi-original.json
  format: json
  label: Ahrefs API v3
  slug: api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahrefs/refs/heads/main/openapi/_original/ahrefs-openapi-original.json
authorization_urls:
- https://app.ahrefs.com/web/oauth/authorize
description: ''
docs: https://docs.ahrefs.com/ahrefs-connect/docs/oauth-guide.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ahrefs Scopes
name_suffix: OAuth Scopes
note: 'The Ahrefs OpenAPI declares only an `http` bearer scheme, so derive-oauth-scopes.py found no oauth2 flows in the spec. The scope surface is real but lives outside the spec: it is documented in the Ahrefs Connect OAuth guide and advertised anonymously in the RFC 8414 authorization-server metadata at https://api.ahrefs.com/.well-known/oauth-authorization-server. Ahrefs does not publish a fine-grained permission catalog — access is coarse (one scope per program), and what a token can reach is governed by the connected account''s plan and API-unit allowance rather than by scopes.'
overview: 'Ahrefs publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ahrefs API on a user''s behalf.


  Tokens are issued from https://ahrefs.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ahrefs
provider_slug: ahrefs
schemes:
- flows:
  - authorizationUrl: https://app.ahrefs.com/web/oauth/authorize
    flow: authorizationCode
    pkce: required (S256)
    tokenUrl: https://ahrefs.com/oauth/token
  name: ahrefs-connect-oauth2
  source: docs
- flows:
  - authorizationUrl: https://app.ahrefs.com/web/oauth/authorize
    flow: authorizationCode
    pkce: supported (S256)
    registrationUrl: https://api.ahrefs.com/mcp/register
    tokenUrl: https://ahrefs.com/oauth/token
  name: ahrefs-mcp-oauth2
  source: well-known/ahrefs-oauth-authorization-server.json
scope_count: 2
scope_names:
- apiv3-integration-apps
- apiv3-mcp
scopes:
- description: Granted to an approved Ahrefs Connect partner application. Lets the app call Ahrefs API v3 on behalf of the authorizing user, spending that user's API units.
  flows:
  - authorizationCode
  scope: apiv3-integration-apps
- description: Granted to an AI client connecting to the hosted Ahrefs MCP server. Advertised as `scopes_supported` by the authorization-server metadata and `scopes_provided` by the protected-resource metadata. Produces an API key tagged with `MCP` scope in the user's account.
  flows:
  - authorizationCode
  scope: apiv3-mcp
slug: ahrefs-scopes
source_filename: ahrefs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.ahrefs.com/ahrefs-connect/docs/oauth-guide.md\ndocs: https://docs.ahrefs.com/ahrefs-connect/docs/oauth-guide.md\nnote: >-\n  The Ahrefs OpenAPI declares only an `http` bearer scheme, so derive-oauth-scopes.py found no oauth2\n  flows in the spec. The scope surface is real but lives outside the spec: it is documented in the\n  Ahrefs Connect OAuth guide and advertised anonymously in the RFC 8414 authorization-server metadata\n  at https://api.ahrefs.com/.well-known/oauth-authorization-server. Ahrefs does not publish a\n  fine-grained permission catalog — access is coarse (one scope per program), and what a token can\n  reach is governed by the connected account's plan and API-unit allowance rather than by scopes.\nschemes:\n- name: ahrefs-connect-oauth2\n  source: docs\n  flows:\n  - flow: authorizationCode\n    pkce: required (S256)\n    authorizationUrl: https://app.ahrefs.com/web/oauth/authorize\n    tokenUrl:\
  \ https://ahrefs.com/oauth/token\n- name: ahrefs-mcp-oauth2\n  source: well-known/ahrefs-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    pkce: supported (S256)\n    authorizationUrl: https://app.ahrefs.com/web/oauth/authorize\n    tokenUrl: https://ahrefs.com/oauth/token\n    registrationUrl: https://api.ahrefs.com/mcp/register\nscopes:\n- scope: apiv3-integration-apps\n  description: >-\n    Granted to an approved Ahrefs Connect partner application. Lets the app call Ahrefs API v3 on\n    behalf of the authorizing user, spending that user's API units.\n  flows:\n  - authorizationCode\n  sources:\n  - https://docs.ahrefs.com/ahrefs-connect/docs/oauth-guide.md\n- scope: apiv3-mcp\n  description: >-\n    Granted to an AI client connecting to the hosted Ahrefs MCP server. Advertised as\n    `scopes_supported` by the authorization-server metadata and `scopes_provided` by the\n    protected-resource metadata. Produces an API key tagged with `MCP` scope in the user's\
  \ account.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/ahrefs-oauth-authorization-server.json\n  - well-known/ahrefs-oauth-protected-resource.json\n  - https://docs.ahrefs.com/mcp/docs/introduction.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahrefs/refs/heads/main/scopes/ahrefs-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- SEO
- Marketing
- Search
- Analytics
- Backlinks
- Keywords
- Web Analytics
- Rank Tracking
- Site Audit
- Brand Monitoring
- Social-Media
token_urls:
- https://ahrefs.com/oauth/token
---
