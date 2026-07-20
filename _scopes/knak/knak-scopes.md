---
api_specs:
- filename: knak-enterprise-openapi-original.yml
  format: yaml
  label: Knak Enterprise API
  slug: enterprise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-enterprise-openapi-original.yml
- filename: knak-send-openapi-original.yml
  format: yaml
  label: Knak Send Contacts API
  slug: send
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-send-openapi-original.yml
- filename: knak-scim-openapi-original.yml
  format: yaml
  label: Knak SCIM API
  slug: scim
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/openapi/knak-scim-openapi-original.yml
authorization_urls:
- https://enterprise.knak.io/oauth/authorize
description: ''
docs: https://developer.knak.com/api/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Knak Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Knak publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Knak API on a user''s behalf.


  Tokens are issued from https://enterprise.knak.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Knak
provider_slug: knak
schemes:
- flows:
  - authorizationUrl: https://enterprise.knak.io/oauth/authorize
    flow: authorizationCode
    notes: Authorization code grant. Applications are registered at https://enterprise.knak.io/account/oauth-applications and receive a client_id, client_secret and redirect_uri. Returns an (access_token, refresh_token) pair.
    scopes_documented: false
    tokenUrl: https://enterprise.knak.io/oauth/token
  name: Knak Enterprise OAuth2
  source: https://developer.knak.com/api/
- flows:
  - authorizationUrl: https://enterprise.knak.io/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://enterprise.knak.io/oauth/register
    scopes_documented: true
    tokenUrl: https://enterprise.knak.io/oauth/token
  name: Knak MCP OAuth 2.1
  source: https://enterprise.knak.io/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp:use
scopes:
- description: Permits an MCP client to invoke the Knak MCP server tools on behalf of the authorizing user.
  flows:
  - authorizationCode
  scope: mcp:use
slug: knak-scopes
source_filename: knak-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://enterprise.knak.io/.well-known/oauth-authorization-server\ndocs: https://developer.knak.com/api/\nnotes: >-\n  The Knak Enterprise API OpenAPI does not declare formal oauth2 securitySchemes, so the\n  mechanical derive pass returns nothing. OAuth 2.0 is nevertheless documented in the\n  Enterprise API overview and a live RFC 8414 authorization server metadata document is\n  published for the MCP server. Access granted through the Enterprise authorization code\n  flow is bounded by the permissions of the authorizing Knak user and their API role\n  rather than by named request scopes; the only scope Knak advertises is mcp:use.\nschemes:\n- name: Knak Enterprise OAuth2\n  source: https://developer.knak.com/api/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://enterprise.knak.io/oauth/authorize\n    tokenUrl: https://enterprise.knak.io/oauth/token\n    scopes_documented: false\n    notes: Authorization\
  \ code grant. Applications are registered at\n      https://enterprise.knak.io/account/oauth-applications and receive a client_id,\n      client_secret and redirect_uri. Returns an (access_token, refresh_token) pair.\n- name: Knak MCP OAuth 2.1\n  source: https://enterprise.knak.io/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://enterprise.knak.io/oauth/authorize\n    tokenUrl: https://enterprise.knak.io/oauth/token\n    registrationUrl: https://enterprise.knak.io/oauth/register\n    pkce: S256\n    scopes_documented: true\nscopes:\n- scope: mcp:use\n  description: Permits an MCP client to invoke the Knak MCP server tools on behalf of the\n    authorizing user.\n  flows:\n  - authorizationCode\n  sources:\n  - https://enterprise.knak.io/.well-known/oauth-authorization-server\ngrant_types:\n- authorization_code\n- refresh_token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knak/refs/heads/main/scopes/knak-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Email Marketing
- Marketing Automation
- Landing Pages
- Content Creation
- Marketing Operations
- Campaign Management
- No-Code
- SCIM
- Webhooks
token_urls:
- https://enterprise.knak.io/oauth/token
---
