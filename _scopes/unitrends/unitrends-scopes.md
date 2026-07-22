---
api_specs:
- filename: unitrends-public-api-openapi.json
  format: json
  label: Unitrends MSP Public API (UniView Portal)
  slug: unitrends-msp-public-api-uniview-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-public-api-openapi.json
authorization_urls:
- https://login.backup.net/connect/authorize
description: ''
docs: https://help.unitrends.kaseya.com/uniview-help/Content/MSP/public-api.htm
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Unitrends Scopes
name_suffix: OAuth Scopes
note: The Public API OpenAPI declares only a Bearer header scheme (no oauth2 flows or per-operation scopes), so the derive pass yields none. The identity service behind it (login.backup.net, UniView / Unitrends MSP portal) publishes its supported scopes via OIDC discovery; API access tokens are obtained with the OAuth 2.0 client_credentials grant and visibility is restricted by the tenant which issued the credentials rather than by fine-grained scopes.
overview: 'Unitrends publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unitrends API on a user''s behalf.


  Tokens are issued from https://login.backup.net/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unitrends
provider_slug: unitrends
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.backup.net/connect/token
  - authorizationUrl: https://login.backup.net/connect/authorize
    flow: authorizationCode
    tokenUrl: https://login.backup.net/connect/token
  issuer: https://login.backup.net
  name: UniView Portal identity service
scope_count: 3
scope_names:
- openid
- role
- profile
scopes:
- description: OpenID Connect authentication scope.
  flows: []
  scope: openid
- description: Role claims for the authenticated principal.
  flows: []
  scope: role
- description: Profile claims for the authenticated principal.
  flows: []
  scope: profile
slug: unitrends-scopes
source_filename: unitrends-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://login.backup.net/.well-known/openid-configuration\ndocs: https://help.unitrends.kaseya.com/uniview-help/Content/MSP/public-api.htm\nnote: >-\n  The Public API OpenAPI declares only a Bearer header scheme (no oauth2 flows\n  or per-operation scopes), so the derive pass yields none. The identity\n  service behind it (login.backup.net, UniView / Unitrends MSP portal)\n  publishes its supported scopes via OIDC discovery; API access tokens are\n  obtained with the OAuth 2.0 client_credentials grant and visibility is\n  restricted by the tenant which issued the credentials rather than by\n  fine-grained scopes.\nschemes:\n- name: UniView Portal identity service\n  issuer: https://login.backup.net\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.backup.net/connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://login.backup.net/connect/authorize\n    tokenUrl: https://login.backup.net/connect/token\n\
  scopes:\n- scope: openid\n  description: OpenID Connect authentication scope.\n  sources: [well-known/unitrends-openid-configuration.json]\n- scope: role\n  description: Role claims for the authenticated principal.\n  sources: [well-known/unitrends-openid-configuration.json]\n- scope: profile\n  description: Profile claims for the authenticated principal.\n  sources: [well-known/unitrends-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/scopes/unitrends-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Company
- Backup
- Disaster Recovery
- Data Protection
- BCDR
- Ransomware Protection
- MSP
- Endpoint Backup
token_urls:
- https://login.backup.net/connect/token
---
