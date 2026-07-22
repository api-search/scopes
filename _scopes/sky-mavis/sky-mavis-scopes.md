---
authorization_urls:
- https://athena.skymavis.com/oauth2/auth
description: ''
docs: https://docs.skymavis.com/mavis/ronin-waypoint/overview
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Sky Mavis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sky Mavis publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sky Mavis API on a user''s behalf.


  Tokens are issued from https://athena.skymavis.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sky Mavis
provider_slug: sky-mavis
schemes:
- flows:
  - authorizationUrl: https://athena.skymavis.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://athena.skymavis.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://athena.skymavis.com/oauth2/token
  issuer: https://athena.skymavis.com/
  name: RoninWaypointOIDC
  source: https://athena.skymavis.com/.well-known/openid-configuration
scope_count: 3
scope_names:
- openid
- offline_access
- offline
scopes:
- description: Standard OpenID Connect scope — issue an ID token identifying the Ronin Waypoint user.
  flows:
  - authorizationCode
  scope: openid
- description: Request a refresh token so the client can obtain new access tokens without re-authenticating.
  flows:
  - authorizationCode
  scope: offline_access
- description: Legacy alias for offline_access (refresh-token issuance) advertised in discovery.
  flows:
  - authorizationCode
  scope: offline
slug: sky-mavis-scopes
source_filename: sky-mavis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://athena.skymavis.com/.well-known/openid-configuration\ndocs: https://docs.skymavis.com/mavis/ronin-waypoint/overview\nschemes:\n- name: RoninWaypointOIDC\n  source: https://athena.skymavis.com/.well-known/openid-configuration\n  issuer: https://athena.skymavis.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://athena.skymavis.com/oauth2/auth\n    tokenUrl: https://athena.skymavis.com/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://athena.skymavis.com/oauth2/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope — issue an ID token identifying the Ronin Waypoint user.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Request a refresh token so the client can obtain new access tokens without re-authenticating.\n  flows: [authorizationCode]\n- scope: offline\n  description: Legacy alias for offline_access (refresh-token issuance) advertised\
  \ in discovery.\n  flows: [authorizationCode]\nnotes: >-\n  Scopes are read verbatim from the Waypoint OIDC discovery\n  (scopes_supported: [offline_access, offline, openid]). Application-specific\n  wallet/profile scopes may be provisioned per client in the Developer Console\n  and are not enumerated in the public discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sky-mavis/refs/heads/main/scopes/sky-mavis-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Blockchain
- Web3
- Gaming
- NFT
- Wallet
- JSON-RPC
- Cryptocurrency
- Developer Tools
token_urls:
- https://athena.skymavis.com/oauth2/token
---
