---
authorization_urls:
- https://access.kymeta.io/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Kymeta Scopes
name_suffix: OAuth Scopes
note: 'The eleven scopes below are published verbatim in scopes_supported by Kymeta''s own identity provider. Kymeta publishes no scope/permission reference page, so the descriptions are limited to what can be stated from first-party evidence — the scope name itself and, where corroborated, the matching service name in the api.kymeta.io /status roll-up. Nothing here is inferred beyond that; scopes with no corroborating evidence are marked description: null rather than guessed.'
overview: 'Kymeta publishes 11 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kymeta API on a user''s behalf.


  Tokens are issued from https://access.kymeta.io/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kymeta
provider_slug: kymeta
schemes:
- flows:
  - authorizationUrl: https://access.kymeta.io/connect/authorize
    flow: authorizationCode
    tokenUrl: https://access.kymeta.io/connect/token
  - flow: clientCredentials
    tokenUrl: https://access.kymeta.io/connect/token
  - deviceAuthorizationUrl: https://access.kymeta.io/connect/deviceauthorization
    flow: deviceCode
    tokenUrl: https://access.kymeta.io/connect/token
  issuer: https://access.kymeta.io
  name: KymetaAccessOIDC
  source: well-known/kymeta-access-openid-configuration.json
scope_count: 11
scope_names:
- openid
- profile
- email
- offline_access
- partners-api
- enterprisebroker
- ksn
- kpp
- grapevine
- live-stream
- absorblms
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope; profile claims.
  flows: []
  scope: profile
- description: Standard OpenID Connect scope; email and email_verified claims.
  flows: []
  scope: email
- description: Standard OpenID Connect scope; issues a refresh token.
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: partners-api
- description: ''
  flows: []
  scope: enterprisebroker
- description: ''
  flows: []
  scope: ksn
- description: ''
  flows: []
  scope: kpp
- description: ''
  flows: []
  scope: grapevine
- description: ''
  flows: []
  scope: live-stream
- description: ''
  flows: []
  scope: absorblms
slug: kymeta-scopes
source_filename: kymeta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://access.kymeta.io/.well-known/openid-configuration\nnote: >-\n  The eleven scopes below are published verbatim in scopes_supported by Kymeta's own identity\n  provider. Kymeta publishes no scope/permission reference page, so the descriptions are limited\n  to what can be stated from first-party evidence — the scope name itself and, where corroborated,\n  the matching service name in the api.kymeta.io /status roll-up. Nothing here is inferred beyond\n  that; scopes with no corroborating evidence are marked description: null rather than guessed.\ndocs: null\ndocs_note: No public scopes or permissions reference is published by Kymeta.\nschemes:\n  - name: KymetaAccessOIDC\n    source: well-known/kymeta-access-openid-configuration.json\n    issuer: https://access.kymeta.io\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://access.kymeta.io/connect/authorize\n        tokenUrl: https://access.kymeta.io/connect/token\n\
  \      - flow: clientCredentials\n        tokenUrl: https://access.kymeta.io/connect/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://access.kymeta.io/connect/deviceauthorization\n        tokenUrl: https://access.kymeta.io/connect/token\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n    standard: oidc-core\n    sources: [well-known/kymeta-access-openid-configuration.json]\n  - scope: profile\n    description: Standard OpenID Connect scope; profile claims.\n    standard: oidc-core\n    sources: [well-known/kymeta-access-openid-configuration.json]\n  - scope: email\n    description: Standard OpenID Connect scope; email and email_verified claims.\n    standard: oidc-core\n    sources: [well-known/kymeta-access-openid-configuration.json]\n  - scope: offline_access\n    description: Standard OpenID Connect scope; issues a refresh token.\n    standard: oidc-core\n    sources: [well-known/kymeta-access-openid-configuration.json]\n\
  \  - scope: partners-api\n    description: null\n    description_note: >-\n      Named partner API scope. This is the clearest published evidence that Kymeta operates a\n      partner-facing API, but no reference documents what it grants.\n    sources: [well-known/kymeta-access-openid-configuration.json]\n  - scope: enterprisebroker\n    description: null\n    description_note: >-\n      Corresponds to the enterpriseBroker service reported by https://api.kymeta.io/status.\n    sources: [well-known/kymeta-access-openid-configuration.json, 'probe:https://api.kymeta.io/status']\n  - scope: ksn\n    description: null\n    sources: [well-known/kymeta-access-openid-configuration.json]\n  - scope: kpp\n    description: null\n    sources: [well-known/kymeta-access-openid-configuration.json]\n  - scope: grapevine\n    description: null\n    description_note: >-\n      Corresponds to https://grapevine.kymeta.io, which redirects into the access.kymeta.io\n      sign-in flow (observed 200 after redirect\
  \ to login.microsoftonline.com with\n      redirect_uri https://access.kymeta.io/signin-microsoft).\n    sources: [well-known/kymeta-access-openid-configuration.json, 'probe:https://grapevine.kymeta.io/']\n  - scope: live-stream\n    description: null\n    sources: [well-known/kymeta-access-openid-configuration.json]\n  - scope: absorblms\n    description: null\n    description_note: >-\n      Federation scope for the Absorb LMS tenant at academy.kymeta.io (vendor-operated).\n    sources: [well-known/kymeta-access-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kymeta/refs/heads/main/scopes/kymeta-scopes.yml
summary_line: 11 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Satellite
- Satellite Communications
- Connectivity
- Telecommunications
- Networking
- Antennas
- Metamaterials
- Aerospace and Defense
- Maritime
- Remote Monitoring
- Hardware
token_urls:
- https://access.kymeta.io/connect/token
---
