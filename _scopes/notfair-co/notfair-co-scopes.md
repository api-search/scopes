---
api_specs:
- filename: notfair-co-health-api-openapi.yml
  format: yaml
  label: notfair-co Health API
  slug: notfair-co-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-health-api-openapi.yml
- filename: notfair-co-mcp-api-openapi.yml
  format: yaml
  label: notfair-co MCP API
  slug: notfair-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-mcp-api-openapi.yml
- filename: notfair-co-well-known-api-openapi.yml
  format: yaml
  label: notfair-co .well Known API
  slug: notfair-co-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-well-known-api-openapi.yml
authorization_urls:
- https://notfair.co/api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Notfair Co Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'notfair-co uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://notfair.co/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: notfair-co
provider_slug: notfair-co
schemes:
- description: Clients self-register at https://notfair.co/api/oauth/register (RFC 7591). The authorization step opens NotFair sign-in, where a person signs up or signs in, chooses a workspace and connects platforms; an agent cannot create the account or approve platform access for them. Authorization code with PKCE (S256) and RFC 8707 resource=https://notfair.co/api/mcp/notfair. Discover authorization server metadata at /.well-known/oauth-authorization-server. For www clients, use that origin for discovery, issuer and resource throughout the flow.
  flows:
  - authorizationUrl: https://notfair.co/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://notfair.co/api/oauth/token
  name: NotFairOAuth
  source: openapi/notfair-co-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: notfair-co-scopes
source_filename: notfair-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: none\nsource: openapi/notfair-co-openapi.json\nschemes:\n- name: NotFairOAuth\n  source: openapi/notfair-co-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://notfair.co/api/oauth/authorize\n    tokenUrl: https://notfair.co/api/oauth/token\n  description: Clients self-register at https://notfair.co/api/oauth/register (RFC 7591). The\n    authorization step opens NotFair sign-in, where a person signs up or signs in, chooses a\n    workspace and connects platforms; an agent cannot create the account or approve platform\n    access for them. Authorization code with PKCE (S256) and RFC 8707 resource=https://notfair.co/api/mcp/notfair.\n    Discover authorization server metadata at /.well-known/oauth-authorization-server. For www\n    clients, use that origin for discovery, issuer and resource throughout the flow.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n\
  \  references one.\n"
source_yaml_url: https://artifacts.apis.io/notfair-co/scopes/notfair-co-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- Artificial Intelligence
- Marketing
- Automation
token_bound: false
token_urls:
- https://notfair.co/api/oauth/token
---
