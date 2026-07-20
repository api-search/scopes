---
api_specs:
- filename: calyptia-cloud-openapi-original.yml
  format: yaml
  label: Calyptia Cloud API
  slug: calyptia-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calyptia/refs/heads/main/openapi/calyptia-cloud-openapi-original.yml
authorization_urls:
- https://sso.calyptia.com/authorize
description: ''
docs: https://sso.calyptia.com/.well-known/openid-configuration
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Calyptia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Calyptia publishes 6 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Calyptia API on a user''s behalf.


  Tokens are issued from https://sso.calyptia.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Calyptia
provider_slug: calyptia
schemes:
- flows:
  - flow: clientCredentials
    scopes: []
    tokenUrl: https://sso.calyptia.com/oauth/token
  - authorizationUrl: https://sso.calyptia.com/authorize
    flow: authorizationCode
    tokenUrl: https://sso.calyptia.com/oauth/token
  name: auth0
  source: openapi/calyptia-cloud-openapi-original.yml
scope_count: 6
scope_names:
- openid
- profile
- email
- offline_access
- address
- phone
scopes:
- description: OIDC authentication (issue an ID token).
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, nickname, picture, etc.).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived sessions.
  flows:
  - authorizationCode
  scope: offline_access
- description: Postal address claim.
  flows:
  - authorizationCode
  scope: address
- description: Phone number claim.
  flows:
  - authorizationCode
  scope: phone
slug: calyptia-scopes
source_filename: calyptia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/calyptia-cloud-openapi-original.yml\ndocs: https://sso.calyptia.com/.well-known/openid-configuration\nnotes: >-\n  The Calyptia Cloud OpenAPI declares the auth0 oauth2 scheme with EMPTY scope\n  maps on both flows (clientCredentials + authorizationCode) — the API does not\n  define resource scopes; authorization is coarse-grained via project tokens\n  (X-Project-Token) and user bearer JWTs. The scopes below are the OIDC identity\n  scopes advertised by the Auth0 tenant's published openid-configuration\n  (scopes_supported), used for the authorizationCode / login flow only. They are\n  identity/profile scopes, not API-resource permissions.\nschemes:\n  - name: auth0\n    source: openapi/calyptia-cloud-openapi-original.yml\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://sso.calyptia.com/oauth/token\n        scopes: []\n      - flow: authorizationCode\n        authorizationUrl: https://sso.calyptia.com/authorize\n\
  \        tokenUrl: https://sso.calyptia.com/oauth/token\nscopes:\n  - scope: openid\n    description: OIDC authentication (issue an ID token).\n    flows: [authorizationCode]\n    source: sso openid-configuration scopes_supported\n  - scope: profile\n    description: Basic profile claims (name, nickname, picture, etc.).\n    flows: [authorizationCode]\n    source: sso openid-configuration scopes_supported\n  - scope: email\n    description: Email address and email_verified claim.\n    flows: [authorizationCode]\n    source: sso openid-configuration scopes_supported\n  - scope: offline_access\n    description: Issue a refresh token for long-lived sessions.\n    flows: [authorizationCode]\n    source: sso openid-configuration scopes_supported\n  - scope: address\n    description: Postal address claim.\n    flows: [authorizationCode]\n    source: sso openid-configuration scopes_supported\n  - scope: phone\n    description: Phone number claim.\n    flows: [authorizationCode]\n    source: sso\
  \ openid-configuration scopes_supported\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calyptia/refs/heads/main/scopes/calyptia-scopes.yml
summary_line: 6 scopes · clientCredentials/authorizationCode
tags:
- Company
- Infrastructure
- Observability
- Telemetry
- Logging
- Fluent Bit
- Data Pipeline
- Kubernetes
- DevOps
token_urls:
- https://sso.calyptia.com/oauth/token
---
