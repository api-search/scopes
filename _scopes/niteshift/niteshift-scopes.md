---
authorization_urls:
- https://auth.niteshift.dev/oauth2/authorize
description: ''
docs: https://auth.niteshift.dev/.well-known/openid-configuration
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Niteshift Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Niteshift publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Niteshift API on a user''s behalf.


  Tokens are issued from https://auth.niteshift.dev/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Niteshift
provider_slug: niteshift
schemes:
- flows:
  - authorizationUrl: https://auth.niteshift.dev/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.niteshift.dev/oauth2/token
  - deviceAuthorizationUrl: https://auth.niteshift.dev/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://auth.niteshift.dev/oauth2/token
  issuer: https://auth.niteshift.dev
  name: OAuth2
  source: well-known/niteshift-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access to the end user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the end user's email address claim.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived, offline access.
  flows: []
  scope: offline_access
slug: niteshift-scopes
source_filename: niteshift-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://niteshift.dev/.well-known/oauth-authorization-server\ndocs: https://auth.niteshift.dev/.well-known/openid-configuration\nschemes:\n  - name: OAuth2\n    source: well-known/niteshift-oauth-authorization-server.json\n    issuer: https://auth.niteshift.dev\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.niteshift.dev/oauth2/authorize\n        tokenUrl: https://auth.niteshift.dev/oauth2/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://auth.niteshift.dev/oauth2/device_authorization\n        tokenUrl: https://auth.niteshift.dev/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token.\n    sources: [well-known/niteshift-oauth-authorization-server.json]\n  - scope: profile\n    description: Access to the end user's basic profile claims.\n    sources: [well-known/niteshift-oauth-authorization-server.json]\n  - scope:\
  \ email\n    description: Access to the end user's email address claim.\n    sources: [well-known/niteshift-oauth-authorization-server.json]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived, offline access.\n    sources: [well-known/niteshift-oauth-authorization-server.json]\nnotes: >-\n  Scopes are the standard OIDC set advertised by scopes_supported in the\n  published RFC 8414 authorization-server metadata. No resource-specific\n  scope taxonomy is published (no provider OpenAPI/API reference exists).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niteshift/refs/heads/main/scopes/niteshift-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Company
- Infrastructure
- Coding Agents
- AI Agents
- Developer Tools
- Cloud Development Environments
- DevOps
- Automation
token_urls:
- https://auth.niteshift.dev/oauth2/token
---
