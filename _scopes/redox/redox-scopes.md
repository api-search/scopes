---
authorization_urls:
- https://api.redoxengine.com/platform/v1/oauth/authorize
description: ''
docs: https://developer.redoxengine.com
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Redox Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Redox publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Redox API on a user''s behalf.


  Tokens are issued from https://api.redoxengine.com/platform/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Redox
provider_slug: redox
schemes:
- flows:
  - authorizationUrl: https://api.redoxengine.com/platform/v1/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.redoxengine.com/platform/v1/oauth/token
  name: RedoxPlatformOAuth
  source: well-known/redox-oauth-authorization-server.json
scope_count: 3
scope_names:
- openid
- offline_access
- platform_access
scopes:
- description: OpenID Connect authentication scope.
  flows:
  - authorizationCode
  scope: openid
- description: Requests a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Access to the Redox Platform API (organizations, sources, destinations).
  flows:
  - authorizationCode
  scope: platform_access
slug: redox-scopes
source_filename: redox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.redoxengine.com/.well-known/oauth-authorization-server\ndocs: https://developer.redoxengine.com\nschemes:\n- name: RedoxPlatformOAuth\n  source: well-known/redox-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.redoxengine.com/platform/v1/oauth/authorize\n    tokenUrl: https://api.redoxengine.com/platform/v1/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication scope.\n  flows: [authorizationCode]\n  sources: [well-known/redox-oauth-authorization-server.json]\n- scope: offline_access\n  description: Requests a refresh token for long-lived access.\n  flows: [authorizationCode]\n  sources: [well-known/redox-oauth-authorization-server.json]\n- scope: platform_access\n  description: Access to the Redox Platform API (organizations, sources, destinations).\n  flows: [authorizationCode]\n  sources: [well-known/redox-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redox/refs/heads/main/scopes/redox-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Healthcare
- Interoperability
- FHIR
- EHR
- Health Data
- Integration
- HL7
- Digital Health
- Healthcare API
token_urls:
- https://api.redoxengine.com/platform/v1/oauth/token
---
