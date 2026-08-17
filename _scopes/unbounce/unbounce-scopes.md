---
api_specs:
- filename: unbounce-accounts-api-openapi.yml
  format: yaml
  label: Unbounce Accounts API
  slug: unbounce-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-accounts-api-openapi.yml
- filename: unbounce-domains-api-openapi.yml
  format: yaml
  label: Unbounce Domains API
  slug: unbounce-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-domains-api-openapi.yml
- filename: unbounce-leads-api-openapi.yml
  format: yaml
  label: Unbounce Leads API
  slug: unbounce-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-leads-api-openapi.yml
- filename: unbounce-meta-api-openapi.yml
  format: yaml
  label: Unbounce Meta API
  slug: unbounce-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-meta-api-openapi.yml
- filename: unbounce-pagegroups-api-openapi.yml
  format: yaml
  label: Unbounce PageGroups API
  slug: unbounce-pagegroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-pagegroups-api-openapi.yml
- filename: unbounce-pages-api-openapi.yml
  format: yaml
  label: Unbounce Pages API
  slug: unbounce-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-pages-api-openapi.yml
- filename: unbounce-users-api-openapi.yml
  format: yaml
  label: Unbounce Users API
  slug: unbounce-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/openapi/unbounce-users-api-openapi.yml
authorization_urls:
- https://api.unbounce.com/oauth/authorize
- https://mcp.unbounce.com/authorize
description: ''
docs: https://developer.unbounce.com/getting_started/#Authorization
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Unbounce Scopes
name_suffix: OAuth Scopes
note: 'Unbounce publishes no scope reference page, because there are no granular scopes to reference. Two independent OAuth surfaces exist and each supports exactly one scope. CORRECTION: an earlier derived pass recorded read/write scopes taken from this repo''s hand-built OpenAPI; Unbounce''s own docs contradict that, and the specs have been corrected to `full`. No scope in this file was inferred.'
overview: 'Unbounce publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unbounce API on a user''s behalf.


  Tokens are issued from https://api.unbounce.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unbounce
provider_slug: unbounce
schemes:
- description: OAuth 2.0 Authorization Code; access tokens are short-lived JWTs.
  flows:
  - authorizationUrl: https://api.unbounce.com/oauth/authorize
    flow: authorizationCode
    refresh: supported via grant_type=refresh_token
    tokenUrl: https://api.unbounce.com/oauth/token
  name: oauth2
  registration: manual — OAuth applications are granted case-by-case via a request form
  source: https://developer.unbounce.com/getting_started/#Authorization
  surface: REST API v0.4
  token_format: JWT
  token_lifetime_seconds: 600
- description: OAuth 2.0 with PKCE and dynamic client registration, per the MCP authorization spec.
  flows:
  - authorizationUrl: https://mcp.unbounce.com/authorize
    flow: authorizationCode
    pkce: S256
    refresh: supported
    tokenUrl: https://mcp.unbounce.com/token
  name: mcp-oauth2
  registration: dynamic — https://mcp.unbounce.com/register (RFC 7591)
  source: https://mcp.unbounce.com/.well-known/oauth-authorization-server
  surface: MCP server (https://mcp.unbounce.com/mcp)
scope_count: 2
scope_names:
- full
- unbounce
scopes:
- description: '"Currently only (default) scope: ''full'' is supported. Which provides access based on the user''s credentials." OAuth tokens grant exactly the permissions the authenticating user already has — there is no narrowing.'
  flows:
  - authorizationCode
  scope: full
- description: 'The single scope advertised by the MCP authorization server (scopes_supported: ["unbounce"]) and demanded in its 401 WWW-Authenticate challenge. Covers every one of the 37 tools, including the destructive ones.'
  flows:
  - authorizationCode
  scope: unbounce
slug: unbounce-scopes
source_filename: unbounce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.unbounce.com/getting_started/#Authorization\ndocs: https://developer.unbounce.com/getting_started/#Authorization\nnote: >-\n  Unbounce publishes no scope reference page, because there are no granular scopes to\n  reference. Two independent OAuth surfaces exist and each supports exactly one scope.\n  CORRECTION: an earlier derived pass recorded read/write scopes taken from this repo's\n  hand-built OpenAPI; Unbounce's own docs contradict that, and the specs have been\n  corrected to `full`. No scope in this file was inferred.\nschemes:\n- name: oauth2\n  surface: REST API v0.4\n  source: https://developer.unbounce.com/getting_started/#Authorization\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.unbounce.com/oauth/authorize\n    tokenUrl: https://api.unbounce.com/oauth/token\n    refresh: supported via grant_type=refresh_token\n  token_format: JWT\n  token_lifetime_seconds: 600\n \
  \ registration: manual — OAuth applications are granted case-by-case via a request form\n  description: OAuth 2.0 Authorization Code; access tokens are short-lived JWTs.\n- name: mcp-oauth2\n  surface: MCP server (https://mcp.unbounce.com/mcp)\n  source: https://mcp.unbounce.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.unbounce.com/authorize\n    tokenUrl: https://mcp.unbounce.com/token\n    pkce: S256\n    refresh: supported\n  registration: dynamic — https://mcp.unbounce.com/register (RFC 7591)\n  description: OAuth 2.0 with PKCE and dynamic client registration, per the MCP authorization spec.\nscopes:\n- scope: full\n  surface: REST API v0.4\n  description: >-\n    \"Currently only (default) scope: 'full' is supported. Which provides access based on\n    the user's credentials.\" OAuth tokens grant exactly the permissions the authenticating\n    user already has — there is no narrowing.\n  flows: [authorizationCode]\n\
  \  sources: [https://developer.unbounce.com/getting_started/#Authorization]\n- scope: unbounce\n  surface: MCP server\n  description: >-\n    The single scope advertised by the MCP authorization server\n    (scopes_supported: [\"unbounce\"]) and demanded in its 401 WWW-Authenticate challenge.\n    Covers every one of the 37 tools, including the destructive ones.\n  flows: [authorizationCode]\n  sources: [https://mcp.unbounce.com/.well-known/oauth-authorization-server]\napi_key:\n  scoped: false\n  note: >-\n    The API key is not scoped at all — \"API keys currently act like Unbounce account\n    administrators\", granting read access to every account, sub-account, domain, page\n    group, page, lead and user an administrator can see.\ngaps:\n- No granular or least-privilege scopes on either surface; both are all-or-nothing.\n- No incremental authorization, no per-resource consent, no scope reference page.\n- An agent holding the `unbounce` MCP scope can delete pages, delete variants and\
  \ reset stats with no further consent step.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbounce/refs/heads/main/scopes/unbounce-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Landing Pages
- Conversion Rate Optimization
- Marketing
- A/B Testing
- Lead Generation
- Marketing Automation
token_urls:
- https://api.unbounce.com/oauth/token
- https://mcp.unbounce.com/token
---
