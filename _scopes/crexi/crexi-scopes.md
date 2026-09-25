---
authorization_urls: []
description: ''
docs: ''
flows:
- password
- refresh_token
- switch_user
- single_use_token_exchange
kind: oauth-scopes
layout: scope
method: probed
name: Crexi Scopes
name_suffix: OAuth Scopes
note: CREXi publishes no OpenAPI with oauth2 securitySchemes and no public scopes/permissions reference page. The scope list below is exactly what the authorization server's own discovery document advertises anonymously — nothing has been added or inferred.
overview: 'CREXi publishes 2 OAuth 2.0 scopes via the password, refresh_token, switch_user, and single_use_token_exchange flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CREXi API on a user''s behalf.


  Tokens are issued from https://api.crexi.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CREXi
provider_slug: crexi
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.crexi.com/token
  - flow: refresh_token
    tokenUrl: https://api.crexi.com/token
  - flow: switch_user
    note: Non-standard grant type advertised by CREXi (user impersonation / account switching).
    tokenUrl: https://api.crexi.com/token
  - flow: single_use_token_exchange
    note: Non-standard grant type advertised by CREXi.
    tokenUrl: https://api.crexi.com/token
  issuer: https://api.crexi.com/
  name: CrexiOAuth2
  source: well-known/crexi-oauth-authorization-server.json
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the authenticated subject.
  flows:
  - password
  - refresh_token
  scope: openid
- description: Requests a refresh token so the client can obtain new access tokens without the resource owner present.
  flows:
  - password
  - refresh_token
  scope: offline_access
slug: crexi-scopes
source_filename: crexi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://api.crexi.com/.well-known/oauth-authorization-server\nnote: 'CREXi publishes no OpenAPI with oauth2 securitySchemes and no public scopes/permissions\n  reference page. The scope list below is exactly what the authorization server''s\n  own discovery document advertises anonymously — nothing has been added or inferred.'\nschemes:\n- name: CrexiOAuth2\n  source: well-known/crexi-oauth-authorization-server.json\n  issuer: https://api.crexi.com/\n  flows:\n  - flow: password\n    tokenUrl: https://api.crexi.com/token\n  - flow: refresh_token\n    tokenUrl: https://api.crexi.com/token\n  - flow: switch_user\n    tokenUrl: https://api.crexi.com/token\n    note: Non-standard grant type advertised by CREXi (user impersonation / account\n      switching).\n  - flow: single_use_token_exchange\n    tokenUrl: https://api.crexi.com/token\n    note: Non-standard grant type advertised by CREXi.\nscopes:\n- scope: openid\n  description:\
  \ Standard OpenID Connect scope requesting an ID token for the authenticated\n    subject.\n  flows:\n  - password\n  - refresh_token\n  sources:\n  - well-known/crexi-oauth-authorization-server.json\n- scope: offline_access\n  description: Requests a refresh token so the client can obtain new access tokens\n    without the resource owner present.\n  flows:\n  - password\n  - refresh_token\n  sources:\n  - well-known/crexi-oauth-authorization-server.json\ncoverage:\n  scopes_published: 2\n  resource_scopes_published: 0\n  note: No resource- or product-level scopes (listings, search, intelligence, auctions)\n    are advertised publicly. Any finer-grained authorization model would only be visible\n    behind the gated Exchange API specification.\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://api.crexi.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json;charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crexi/refs/heads/main/scopes/crexi-scopes.yml
summary_line: 2 scopes · password/refresh_token/switch_user/single_use_token_exchange
tags:
- Real Estate
- Commercial Real Estate
- Marketplace
- Property Data
- Listings
- Auctions
- Market Intelligence
- Data Syndication
- RESO
- Company
token_urls:
- https://api.crexi.com/token
---
