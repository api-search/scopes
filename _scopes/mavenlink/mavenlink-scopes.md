---
api_specs:
- filename: mavenlink-openapi.yml
  format: yaml
  label: Kantata OX API
  slug: kantata-ox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mavenlink/refs/heads/main/openapi/mavenlink-openapi.yml
authorization_urls:
- https://app.mavenlink.com/oauth/authorize
- https://api.mavenlink.com/oauth/authorize
description: ''
docs: https://developer.kantata.com/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Mavenlink Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mavenlink publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mavenlink API on a user''s behalf.


  Tokens are issued from https://app.mavenlink.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mavenlink
provider_slug: mavenlink
schemes:
- flows:
  - authorizationUrl: https://app.mavenlink.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.mavenlink.com/oauth/token
  name: OauthSecurity
  source: openapi/mavenlink-openapi.yml
- flows:
  - authorizationUrl: https://api.mavenlink.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.mavenlink.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.mavenlink.com/oauth/token
  name: KantataOpenIDConnect
  source: well-known/mavenlink-api-openid-configuration.json
scope_count: 6
scope_names:
- api_only
- openid
- email
- profile
- mcp
- offline_access
scopes:
- description: Kantata OX API access without OpenID identity claims. Published in scopes_supported; Kantata does not publish a prose description for it.
  flows: []
  scope: api_only
- description: Standard OpenID Connect scope requesting an ID token.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope releasing the `email` claim.
  flows: []
  scope: email
- description: Standard OpenID Connect scope releasing profile claims. Kantata's userinfo advertises name, given_name, family_name, preferred_username plus the Kantata-specific account_id and account_name claims.
  flows: []
  scope: profile
- description: Grants access to the Kantata OX MCP server at https://api.mavenlink.com/mcp. It is the ONLY scope listed in the MCP authorization-server metadata, so the MCP surface is gated behind one all-or-nothing scope rather than per-tool scopes.
  flows: []
  scope: mcp
- description: Standard OpenID Connect scope requesting a refresh token.
  flows: []
  scope: offline_access
slug: mavenlink-scopes
source_filename: mavenlink-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://api.mavenlink.com/.well-known/openid-configuration\ndocs: https://developer.kantata.com/\nnotes: >-\n  The Swagger 2.0 securityDefinition `OauthSecurity` declares an EMPTY scopes map, so nothing is derivable from\n  the spec. The real scope list is published anonymously in the OpenID Connect discovery document on both\n  api.mavenlink.com and app.mavenlink.com (probed 2026-08-25, HTTP 200), and the MCP authorization-server\n  metadata narrows to a single `mcp` scope. No prose scope/permission reference page was found on\n  developer.kantata.com or the Kantata knowledge base; the knowledge base article set covering API limits is\n  behind the customer login.\nschemes:\n- name: OauthSecurity\n  source: openapi/mavenlink-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.mavenlink.com/oauth/authorize\n    tokenUrl: https://app.mavenlink.com/oauth/token\n- name: KantataOpenIDConnect\n  source:\
  \ well-known/mavenlink-api-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.mavenlink.com/oauth/authorize\n    tokenUrl: https://api.mavenlink.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.mavenlink.com/oauth/token\nscopes:\n- scope: api_only\n  description: >-\n    Kantata OX API access without OpenID identity claims. Published in scopes_supported; Kantata does not\n    publish a prose description for it.\n  source: https://api.mavenlink.com/.well-known/openid-configuration\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n  source: https://api.mavenlink.com/.well-known/openid-configuration\n- scope: email\n  description: Standard OpenID Connect scope releasing the `email` claim.\n  source: https://api.mavenlink.com/.well-known/openid-configuration\n- scope: profile\n  description: >-\n    Standard OpenID Connect scope releasing profile claims. Kantata's userinfo advertises\
  \ name, given_name,\n    family_name, preferred_username plus the Kantata-specific account_id and account_name claims.\n  source: https://api.mavenlink.com/.well-known/openid-configuration\n- scope: mcp\n  description: >-\n    Grants access to the Kantata OX MCP server at https://api.mavenlink.com/mcp. It is the ONLY scope listed in\n    the MCP authorization-server metadata, so the MCP surface is gated behind one all-or-nothing scope rather\n    than per-tool scopes.\n  source: https://api.mavenlink.com/.well-known/oauth-authorization-server\n- scope: offline_access\n  description: Standard OpenID Connect scope requesting a refresh token.\n  source: https://api.mavenlink.com/.well-known/openid-configuration\nscope_count: 6\nobservations:\n- >-\n  Scopes are coarse. There is no read/write split and no per-resource scope: an application authorised for the\n  Kantata OX API can reach every one of the 419 operations the user's own permissions allow, including the 251\n  write operations (86\
  \ POST, 91 PUT, 74 DELETE). Authorisation granularity is enforced by Kantata's in-product\n  access groups and roles, not by OAuth scope.\n- >-\n  The MCP authorization server advertises PKCE S256 only (the OIDC document also allows `plain`), and\n  authorization_code only - no client_credentials for the MCP surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mavenlink/refs/heads/main/scopes/mavenlink-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Professional Services Automation
- Project Management
- Resource Management
- Time Tracking
- Expense Management
- Invoicing
- Project Accounting
- Business Intelligence
- Workflow Automation
- MCP
- agent-native
- Company
token_urls:
- https://app.mavenlink.com/oauth/token
- https://api.mavenlink.com/oauth/token
---
