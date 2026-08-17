---
api_specs:
- filename: clickfunnels-api-openapi.json
  format: json
  label: ClickFunnels API
  slug: clickfunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/openapi/clickfunnels-api-openapi.json
authorization_urls:
- https://accounts.myclickfunnels.com/oauth/authorize
description: ''
docs: https://developers.myclickfunnels.com/docs/oauth-20
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Clickfunnels Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only a bearer scheme and no oauth2 securityScheme, so nothing is derivable from the spec. The scope list below is the authoritative one ClickFunnels publishes, in its RFC 8414 authorization-server metadata. The OAuth guide tells integrators "You should not need to specify any scopes" and that the default grant is full access to the authorized workspace; a real token response in the docs shows scope "admin read". The `mcp` scope is advertised but no reachable MCP endpoint was found — see mcp/clickfunnels-mcp.yml.
overview: 'ClickFunnels publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClickFunnels API on a user''s behalf.


  Tokens are issued from https://accounts.myclickfunnels.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClickFunnels
provider_slug: clickfunnels
schemes:
- flows:
  - authorizationUrl: https://accounts.myclickfunnels.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://accounts.myclickfunnels.com/oauth/register
    revocationUrl: https://accounts.myclickfunnels.com/oauth/revoke
    tokenUrl: https://accounts.myclickfunnels.com/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
    - client_secret_basic
  grant_types:
  - authorization_code
  - refresh_token
  name: OAuth2
  source: https://accounts.myclickfunnels.com/.well-known/oauth-authorization-server
scope_count: 5
scope_names:
- admin
- read
- write
- delete
- mcp
scopes:
- description: Administrative access to the authorized workspace. Part of the default grant shown in the OAuth token response example.
  flows: []
  scope: admin
- description: Read access to the authorized workspace. Part of the default grant.
  flows: []
  scope: read
- description: Write access to the authorized workspace.
  flows: []
  scope: write
- description: Delete access to the authorized workspace.
  flows: []
  scope: delete
- description: Advertised scope for Model Context Protocol access. No reachable MCP endpoint was found on any ClickFunnels host on 2026-08-13.
  flows: []
  scope: mcp
slug: clickfunnels-scopes
source_filename: clickfunnels-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://accounts.myclickfunnels.com/.well-known/oauth-authorization-server\ndocs: https://developers.myclickfunnels.com/docs/oauth-20\nnote: The OpenAPI declares only a bearer scheme and no oauth2 securityScheme, so nothing is derivable from\n  the spec. The scope list below is the authoritative one ClickFunnels publishes, in its RFC 8414 authorization-server\n  metadata. The OAuth guide tells integrators \"You should not need to specify any scopes\" and that the default\n  grant is full access to the authorized workspace; a real token response in the docs shows scope \"admin read\".\n  The `mcp` scope is advertised but no reachable MCP endpoint was found — see mcp/clickfunnels-mcp.yml.\nschemes:\n- name: OAuth2\n  source: https://accounts.myclickfunnels.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.myclickfunnels.com/oauth/authorize\n    tokenUrl:\
  \ https://accounts.myclickfunnels.com/oauth/token\n    revocationUrl: https://accounts.myclickfunnels.com/oauth/revoke\n    registrationUrl: https://accounts.myclickfunnels.com/oauth/register\n    pkce:\n    - S256\n    token_endpoint_auth_methods:\n    - none\n    - client_secret_post\n    - client_secret_basic\n  grant_types:\n  - authorization_code\n  - refresh_token\nscopes:\n- scope: admin\n  description: Administrative access to the authorized workspace. Part of the default grant shown in the OAuth\n    token response example.\n  sources:\n  - /.well-known/oauth-authorization-server\n- scope: read\n  description: Read access to the authorized workspace. Part of the default grant.\n  sources:\n  - /.well-known/oauth-authorization-server\n- scope: write\n  description: Write access to the authorized workspace.\n  sources:\n  - /.well-known/oauth-authorization-server\n- scope: delete\n  description: Delete access to the authorized workspace.\n  sources:\n  - /.well-known/oauth-authorization-server\n\
  - scope: mcp\n  description: Advertised scope for Model Context Protocol access. No reachable MCP endpoint was found on any\n    ClickFunnels host on 2026-08-13.\n  sources:\n  - /.well-known/oauth-authorization-server\nenforcement:\n  error: 403\n  description: The spec declares a 403 variant reading \"the access token's scopes do not cover this request\"\n    on 5 operations.\ntoken_lifetime:\n  expires: false\n  note: The OAuth guide states tokens do not expire and there is no refresh-token rotation in practice — ignore\n    the expires_in field. The metadata nonetheless advertises the refresh_token grant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/scopes/clickfunnels-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Sales Funnels
- Landing Pages
- E-commerce
- Marketing
- Checkout
- CRM
- Email Marketing
- Online Courses
- Webhooks
- Website Builder
- Subscriptions
- Marketing Automation
- Agent Skills
token_urls:
- https://accounts.myclickfunnels.com/oauth/token
---
