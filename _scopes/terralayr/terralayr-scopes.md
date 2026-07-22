---
authorization_urls:
- https://www.trlyr.com/umbraco/delivery/api/v1/security/member/authorize
description: ''
docs: https://www.trlyr.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Terralayr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'terralayr publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the terralayr API on a user''s behalf.


  Tokens are issued from https://www.trlyr.com/umbraco/delivery/api/v1/security/member/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: terralayr
provider_slug: terralayr
schemes:
- flows:
  - authorizationUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    tokenUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/token
  name: oauth2
  source: well-known/terralayr-oauth-authorization-server.json
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: OpenID Connect authentication for a site member
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token so the client can act while the member is offline
  flows:
  - authorizationCode
  scope: offline_access
slug: terralayr-scopes
source_filename: terralayr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.trlyr.com/.well-known/openid-configuration\ndocs: https://www.trlyr.com/.well-known/openid-configuration\nschemes:\n- name: oauth2\n  source: well-known/terralayr-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://www.trlyr.com/umbraco/delivery/api/v1/security/member/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication for a site member\n  flows: [authorizationCode]\n  sources: [well-known/terralayr-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can act while the member is offline\n  flows: [authorizationCode]\n  sources: [well-known/terralayr-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terralayr/refs/heads/main/scopes/terralayr-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Climate
- Energy
- Battery Energy Storage
- Grid Flexibility
- Renewable Energy
- Cleantech
- Energy Trading
token_urls:
- https://www.trlyr.com/umbraco/delivery/api/v1/security/member/token
---
