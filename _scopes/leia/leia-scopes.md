---
api_specs:
- filename: leia-immersity-cloud-api-openapi.yml
  format: yaml
  label: Immersity Cloud API
  slug: immersity-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-immersity-cloud-api-openapi.yml
- filename: leia-immersity-authentication-openapi.yml
  format: yaml
  label: Immersity AI Authentication API
  slug: immersity-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-immersity-authentication-openapi.yml
authorization_urls:
- https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/auth
description: ''
docs: https://docs-api.immersity.ai/docs/getting-started
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Leia Scopes
name_suffix: OAuth Scopes
note: The published Immersity OpenAPI documents declare a plain bearer scheme and carry no oauth2 flow object, so no scopes could be derived from the specs. These scopes were read from the live OIDC discovery document of the Immersity Keycloak realm (scopes_supported), which is served anonymously. Descriptions are our own reading of each scope name against the platform's documented services; Immersity does not publish a scope reference page. Which scopes a given client-credentials client is actually granted is set per client in the Immersity account console.
overview: 'Leia publishes 20 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Leia API on a user''s behalf.


  Tokens are issued from https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Leia
provider_slug: leia
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/token
  - authorizationUrl: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/token
  issuer: https://auth.immersity.ai/auth/realms/immersity
  name: immersity-keycloak
  source: well-known/leia-openid-configuration.json
scope_count: 20
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- web-origins
- acr
- basic
- microprofile-jwt
- service_account
- leia-api-gateway
- leia-storage-service
- product-price-service
- payment-entitlement-service
- immersity-sdk-developer
- immersity-ai-mobile-backend
- device-management
- user-created-timestamp
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticated subject.
  flows: []
  scope: profile
- description: Email address claim for the authenticated subject.
  flows: []
  scope: email
- description: Address claims for the authenticated subject.
  flows: []
  scope: address
- description: Phone number claims for the authenticated subject.
  flows: []
  scope: phone
- description: Realm and client role claims.
  flows: []
  scope: roles
- description: Issue a refresh token usable while the user is offline.
  flows: []
  scope: offline_access
- description: CORS allowed-origins claim (Keycloak built-in).
  flows: []
  scope: web-origins
- description: Authentication context class reference (Keycloak built-in).
  flows: []
  scope: acr
- description: Baseline token claims (Keycloak built-in).
  flows: []
  scope: basic
- description: MicroProfile JWT claim mapping (Keycloak built-in).
  flows: []
  scope: microprofile-jwt
- description: Marks a machine-to-machine client-credentials service account token.
  flows: []
  scope: service_account
- description: Access to the Leia/Immersity API gateway fronting the Immersity Cloud API.
  flows: []
  scope: leia-api-gateway
- description: Access to Leia Storage, the presigned-URL upload/download service.
  flows: []
  scope: leia-storage-service
- description: Access to the product pricing service backing GET /api/v1/prices.
  flows: []
  scope: product-price-service
- description: Access to the credit/entitlement service that meters API consumption.
  flows: []
  scope: payment-entitlement-service
- description: Developer entitlement for the gated Immersity SDK portal (support.immersity.ai/sdk).
  flows: []
  scope: immersity-sdk-developer
- description: Backend access used by the Immersity AI mobile applications.
  flows: []
  scope: immersity-ai-mobile-backend
- description: Device registration and management for Immersity-enabled hardware.
  flows: []
  scope: device-management
- description: Exposes the account creation timestamp as a token claim.
  flows: []
  scope: user-created-timestamp
slug: leia-scopes
source_filename: leia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://auth.immersity.ai/auth/realms/immersity/.well-known/openid-configuration\ndocs: https://docs-api.immersity.ai/docs/getting-started\nnote: >-\n  The published Immersity OpenAPI documents declare a plain bearer scheme and carry no oauth2 flow object,\n  so no scopes could be derived from the specs. These scopes were read from the live OIDC discovery document\n  of the Immersity Keycloak realm (scopes_supported), which is served anonymously. Descriptions are our own\n  reading of each scope name against the platform's documented services; Immersity does not publish a scope\n  reference page. Which scopes a given client-credentials client is actually granted is set per client in\n  the Immersity account console.\nschemes:\n- name: immersity-keycloak\n  issuer: https://auth.immersity.ai/auth/realms/immersity\n  source: well-known/leia-openid-configuration.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/token\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/auth\n    tokenUrl: https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  kind: standard\n- scope: profile\n  description: Basic profile claims for the authenticated subject.\n  kind: standard\n- scope: email\n  description: Email address claim for the authenticated subject.\n  kind: standard\n- scope: address\n  description: Address claims for the authenticated subject.\n  kind: standard\n- scope: phone\n  description: Phone number claims for the authenticated subject.\n  kind: standard\n- scope: roles\n  description: Realm and client role claims.\n  kind: standard\n- scope: offline_access\n  description: Issue a refresh token usable while the user is offline.\n  kind: standard\n- scope: web-origins\n  description: CORS allowed-origins claim (Keycloak\
  \ built-in).\n  kind: standard\n- scope: acr\n  description: Authentication context class reference (Keycloak built-in).\n  kind: standard\n- scope: basic\n  description: Baseline token claims (Keycloak built-in).\n  kind: standard\n- scope: microprofile-jwt\n  description: MicroProfile JWT claim mapping (Keycloak built-in).\n  kind: standard\n- scope: service_account\n  description: Marks a machine-to-machine client-credentials service account token.\n  kind: platform\n- scope: leia-api-gateway\n  description: Access to the Leia/Immersity API gateway fronting the Immersity Cloud API.\n  kind: platform\n- scope: leia-storage-service\n  description: Access to Leia Storage, the presigned-URL upload/download service.\n  kind: platform\n- scope: product-price-service\n  description: Access to the product pricing service backing GET /api/v1/prices.\n  kind: platform\n- scope: payment-entitlement-service\n  description: Access to the credit/entitlement service that meters API consumption.\n\
  \  kind: platform\n- scope: immersity-sdk-developer\n  description: Developer entitlement for the gated Immersity SDK portal (support.immersity.ai/sdk).\n  kind: platform\n- scope: immersity-ai-mobile-backend\n  description: Backend access used by the Immersity AI mobile applications.\n  kind: platform\n- scope: device-management\n  description: Device registration and management for Immersity-enabled hardware.\n  kind: platform\n- scope: user-created-timestamp\n  description: Exposes the account creation timestamp as a token claim.\n  kind: platform\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://auth.immersity.ai/auth/realms/immersity/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n  scope_count: 20\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/scopes/leia-scopes.yml
summary_line: 20 scopes · clientCredentials/authorizationCode
tags:
- 3d
- spatial-computing
- computer-vision
- depth-estimation
- image-processing
- video-processing
- generative-ai
- displays
- media-transformation
- immersive-experiences
token_urls:
- https://auth.immersity.ai/auth/realms/immersity/protocol/openid-connect/token
---
