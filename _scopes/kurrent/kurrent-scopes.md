---
api_specs:
- filename: kurrent-kurrentdb-http-api-openapi.yml
  format: yaml
  label: KurrentDB HTTP API
  slug: kurrentdb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-kurrentdb-http-api-openapi.yml
authorization_urls:
- https://identity.eventstore.com/authorize
description: ''
docs: https://docs.kurrent.io/cloud/ops/account-security.html
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Kurrent Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kurrent publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kurrent API on a user''s behalf.


  Tokens are issued from https://identity.eventstore.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kurrent
provider_slug: kurrent
schemes:
- discovery:
  - https://identity.eventstore.com/.well-known/openid-configuration
  - https://identity.eventstore.com/.well-known/oauth-authorization-server
  endpoints:
    jwks: https://identity.eventstore.com/.well-known/jwks.json
    registration: https://identity.eventstore.com/oidc/register
    revocation: https://identity.eventstore.com/oauth/revoke
    userinfo: https://identity.eventstore.com/userinfo
  flows:
  - authorizationUrl: https://identity.eventstore.com/authorize
    flow: authorizationCode
    tokenUrl: https://identity.eventstore.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://identity.eventstore.com/oauth/token
  - deviceAuthorizationUrl: https://identity.eventstore.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://identity.eventstore.com/oauth/token
  issuer: https://identity.eventstore.com/
  name: KurrentCloudOIDC
  pkce_methods:
  - S256
  - plain
  source: well-known/kurrent-openid-configuration.json
  type: openIdConnect
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- email
- email_verified
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Request an ID token and authenticate the end user via OpenID Connect.
  flows: []
  scope: openid
- description: Access the end user's default profile claims.
  flows: []
  scope: profile
- description: Request a refresh token so the client can obtain new access tokens without the user present.
  flows: []
  scope: offline_access
- description: Access the end user's email address claim.
  flows: []
  scope: email
- description: Access whether the end user's email address has been verified.
  flows: []
  scope: email_verified
- description: Access the end user's full name claim.
  flows: []
  scope: name
- description: Access the end user's given name claim.
  flows: []
  scope: given_name
- description: Access the end user's family name claim.
  flows: []
  scope: family_name
- description: Access the end user's nickname claim.
  flows: []
  scope: nickname
- description: Access the end user's profile picture claim.
  flows: []
  scope: picture
- description: Access the timestamp at which the end user's account was created.
  flows: []
  scope: created_at
- description: Access the linked identity providers associated with the end user's account.
  flows: []
  scope: identities
- description: Access the end user's phone number claim.
  flows: []
  scope: phone
- description: Access the end user's address claim.
  flows: []
  scope: address
slug: kurrent-scopes
source_filename: kurrent-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://identity.eventstore.com/.well-known/openid-configuration\ndocs: https://docs.kurrent.io/cloud/ops/account-security.html\nnotes: >-\n  The KurrentDB HTTP API itself is not OAuth-protected — it uses HTTP Basic authentication with\n  per-stream access control lists, so it declares no oauth2 security scheme and therefore no\n  scopes. The OAuth surface Kurrent operates belongs to Kurrent Cloud, whose identity provider at\n  identity.eventstore.com publishes OpenID Connect discovery and RFC 8414 authorization-server\n  metadata. The scopes below are the scopes_supported advertised by that discovery document; they\n  are the standard OpenID Connect and profile-claim scopes rather than a Kurrent-specific\n  permission taxonomy. Kurrent does not publish a product-level scope reference.\nschemes:\n- name: KurrentCloudOIDC\n  type: openIdConnect\n  issuer: https://identity.eventstore.com/\n  source: well-known/kurrent-openid-configuration.json\n\
  \  discovery:\n  - https://identity.eventstore.com/.well-known/openid-configuration\n  - https://identity.eventstore.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.eventstore.com/authorize\n    tokenUrl: https://identity.eventstore.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://identity.eventstore.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://identity.eventstore.com/oauth/device/code\n    tokenUrl: https://identity.eventstore.com/oauth/token\n  endpoints:\n    userinfo: https://identity.eventstore.com/userinfo\n    jwks: https://identity.eventstore.com/.well-known/jwks.json\n    revocation: https://identity.eventstore.com/oauth/revoke\n    registration: https://identity.eventstore.com/oidc/register\n  pkce_methods: [S256, plain]\nscopes:\n- scope: openid\n  description: Request an ID token and authenticate the end user via OpenID Connect.\n  standard: openid-connect\n\
  - scope: profile\n  description: Access the end user's default profile claims.\n  standard: openid-connect\n- scope: offline_access\n  description: Request a refresh token so the client can obtain new access tokens without the user present.\n  standard: openid-connect\n- scope: email\n  description: Access the end user's email address claim.\n  standard: openid-connect\n- scope: email_verified\n  description: Access whether the end user's email address has been verified.\n- scope: name\n  description: Access the end user's full name claim.\n- scope: given_name\n  description: Access the end user's given name claim.\n- scope: family_name\n  description: Access the end user's family name claim.\n- scope: nickname\n  description: Access the end user's nickname claim.\n- scope: picture\n  description: Access the end user's profile picture claim.\n- scope: created_at\n  description: Access the timestamp at which the end user's account was created.\n- scope: identities\n  description: Access\
  \ the linked identity providers associated with the end user's account.\n- scope: phone\n  description: Access the end user's phone number claim.\n- scope: address\n  description: Access the end user's address claim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/scopes/kurrent-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Database
- Event Sourcing
- Event Streaming
- Event Driven Architecture
- CQRS
- Data Infrastructure
- Developer Tools
- Cloud
- Open Source
- gRPC
- Agentic AI
token_urls:
- https://identity.eventstore.com/oauth/token
---
