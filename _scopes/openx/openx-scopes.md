---
authorization_urls:
- https://api.openx.com/oauth2/v1/authorize
description: ''
docs: https://docs.openx.com/developers/api-authentication/
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Openx Scopes
name_suffix: OAuth Scopes
note: OpenX publishes no OpenAPI, so these scopes are read from the live OIDC discovery document and the RFC 9728 protected-resource metadata served at api.openx.com, cross-checked against the scope string the published authentication guide tells integrators to send ("openid email profile api"). OpenX documents no per-resource or per-object scopes — `api` is a single coarse grant covering the whole Platform API; object-level access is controlled by the OpenX user's role/ACL inside the instance, not by scope.
overview: 'OpenX publishes 5 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the OpenX API on a user''s behalf.


  Tokens are issued from https://api.openx.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OpenX
provider_slug: openx
schemes:
- flows:
  - authorizationUrl: https://api.openx.com/oauth2/v1/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://api.openx.com/oauth2/v1/token
  - flow: refreshToken
    tokenUrl: https://api.openx.com/oauth2/v1/token
  issuer: https://api.openx.com
  name: OpenXPlatformOAuth2
  source: https://api.openx.com/.well-known/openid-configuration
scope_count: 5
scope_names:
- api
- openid
- email
- profile
- offline_access
scopes:
- description: Access the OpenX Platform API and Reporting API on the authenticated user's behalf. Coarse-grained — there is no read/write or per-object split.
  flows:
  - authorizationCode
  - refreshToken
  scope: api
- description: OpenID Connect authentication; requests an id_token.
  flows:
  - authorizationCode
  scope: openid
- description: Release the email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Release the name and user_id profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh_token so the client can mint new access tokens without re-authenticating. Advertised in discovery but not named in the published authentication guide, which nonetheless documents the refresh_token grant.
  flows:
  - authorizationCode
  scope: offline_access
slug: openx-scopes
source_filename: openx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.openx.com/.well-known/openid-configuration\ndocs: https://docs.openx.com/developers/api-authentication/\nnote: >-\n  OpenX publishes no OpenAPI, so these scopes are read from the live OIDC\n  discovery document and the RFC 9728 protected-resource metadata served at\n  api.openx.com, cross-checked against the scope string the published\n  authentication guide tells integrators to send (\"openid email profile api\").\n  OpenX documents no per-resource or per-object scopes — `api` is a single\n  coarse grant covering the whole Platform API; object-level access is\n  controlled by the OpenX user's role/ACL inside the instance, not by scope.\nschemes:\n  - name: OpenXPlatformOAuth2\n    source: https://api.openx.com/.well-known/openid-configuration\n    issuer: https://api.openx.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.openx.com/oauth2/v1/authorize\n        tokenUrl: https://api.openx.com/oauth2/v1/token\n\
  \        code_challenge_methods: [S256]\n      - flow: refreshToken\n        tokenUrl: https://api.openx.com/oauth2/v1/token\nscopes:\n  - scope: api\n    description: >-\n      Access the OpenX Platform API and Reporting API on the authenticated\n      user's behalf. Coarse-grained — there is no read/write or per-object split.\n    flows: [authorizationCode, refreshToken]\n    sources: [https://api.openx.com/.well-known/openid-configuration]\n  - scope: openid\n    description: OpenID Connect authentication; requests an id_token.\n    flows: [authorizationCode]\n    sources: [https://api.openx.com/.well-known/openid-configuration]\n  - scope: email\n    description: Release the email and email_verified claims.\n    flows: [authorizationCode]\n    sources: [https://api.openx.com/.well-known/openid-configuration]\n  - scope: profile\n    description: Release the name and user_id profile claims.\n    flows: [authorizationCode]\n    sources: [https://api.openx.com/.well-known/openid-configuration]\n\
  \  - scope: offline_access\n    description: >-\n      Issue a refresh_token so the client can mint new access tokens without\n      re-authenticating. Advertised in discovery but not named in the published\n      authentication guide, which nonetheless documents the refresh_token grant.\n    flows: [authorizationCode]\n    sources: [https://api.openx.com/.well-known/openid-configuration]\nprotected_resource:\n  resource: https://api.openx.com\n  resource_name: OpenX Platform API\n  authorization_servers: [https://api.openx.com]\n  bearer_methods_supported: [header]\n  source: https://api.openx.com/.well-known/oauth-protected-resource\nclaims_supported: [aud, email, email_verified, exp, iat, iss, name, sub, user_id]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openx/refs/heads/main/scopes/openx-scopes.yml
summary_line: 5 scopes · authorizationCode/refreshToken
tags:
- Advertising
- Programmatic Advertising
- Ad Exchange
- Supply Side Platform
- SSP
- Real Time Bidding
- OpenRTB
- Header Bidding
- Prebid
- AdTech
- CTV
- Video Advertising
- Display Advertising
- Curation
- Identity
- GraphQL
- gRPC
- MCP
- Reporting
- Audience Targeting
token_urls:
- https://api.openx.com/oauth2/v1/token
---
