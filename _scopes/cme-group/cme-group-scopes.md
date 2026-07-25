---
authorization_urls: []
description: ''
docs: https://cmegroupclientsite.atlassian.net/wiki/spaces/EPICSANDBOX/pages/457316022/Client+API+Service+Adoption+Using+OAuth+2.0+Protocol
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Cme Group Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CME Group publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CME Group API on a user''s behalf.


  Tokens are issued from https://auth.cmegroup.com/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CME Group
provider_slug: cme-group
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.cmegroup.com/as/token.oauth2
  - flow: clientCredentials
    tokenUrl: https://authnr.cmegroup.com/as/token.oauth2
  name: CMEGroupOAuth
  source: well-known/cme-group-oauth-authorization-server.json
scope_count: 5
scope_names:
- UNOEntitlement
- openid
- profile
- email
- offline_access
scopes:
- description: CME Group entitlement scope advertised by the authorization server (RFC 8414 scopes_supported).
  flows:
  - clientCredentials
  scope: UNOEntitlement
- description: OpenID Connect authentication scope.
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: OpenID Connect email claim.
  flows:
  - authorizationCode
  scope: email
- description: Refresh-token issuance for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
slug: cme-group-scopes
source_filename: cme-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://auth.cmegroup.com/.well-known/oauth-authorization-server\ndocs: https://cmegroupclientsite.atlassian.net/wiki/spaces/EPICSANDBOX/pages/457316022/Client+API+Service+Adoption+Using+OAuth+2.0+Protocol\nnotes: >-\n  CME Group authorization is primarily entitlement-based (per-API-ID\n  entitlements managed in the CME Customer Center), not scope-based. The\n  PingFederate authorization server at auth.cmegroup.com advertises the scopes\n  below in its anonymous RFC 8414 metadata; API access itself is granted by\n  entitling the OAuth API ID to each API rather than by requesting granular\n  scopes. No public OpenAPI declares oauth2 scopes.\nschemes:\n  - name: CMEGroupOAuth\n    source: well-known/cme-group-oauth-authorization-server.json\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.cmegroup.com/as/token.oauth2\n      - flow: clientCredentials\n        tokenUrl: https://authnr.cmegroup.com/as/token.oauth2\n\
  scopes:\n  - scope: UNOEntitlement\n    description: CME Group entitlement scope advertised by the authorization server (RFC 8414 scopes_supported).\n    flows: [clientCredentials]\n    sources: [well-known/cme-group-oauth-authorization-server.json]\n  - scope: openid\n    description: OpenID Connect authentication scope.\n    flows: [authorizationCode]\n    sources: [well-known/cme-group-openid-configuration.json]\n  - scope: profile\n    description: OpenID Connect profile claims.\n    flows: [authorizationCode]\n    sources: [well-known/cme-group-openid-configuration.json]\n  - scope: email\n    description: OpenID Connect email claim.\n    flows: [authorizationCode]\n    sources: [well-known/cme-group-openid-configuration.json]\n  - scope: offline_access\n    description: Refresh-token issuance for long-lived access.\n    flows: [authorizationCode]\n    sources: [well-known/cme-group-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cme-group/refs/heads/main/scopes/cme-group-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Capital Markets
- Derivatives
- Exchange
- Financial Markets
- Futures
- Market Data
- Options
- Reference Data
- Trading
- Fortune 1000
token_urls:
- https://auth.cmegroup.com/as/token.oauth2
- https://authnr.cmegroup.com/as/token.oauth2
---
