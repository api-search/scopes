---
api_specs:
- filename: picarro-sam-foup-asyncapi.yml
  format: yaml
  label: Picarro Edge — SAM FOUP gRPC API
  slug: picarro-edge-sam-foup-grpc-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/picarro/refs/heads/main/asyncapi/picarro-sam-foup-asyncapi.yml
authorization_urls:
- https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Picarro Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Picarro publishes 9 OAuth 2.0 scopes via the authorizationCode, implicit, password, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Picarro API on a user''s behalf.


  Tokens are issued from https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Picarro
provider_slug: picarro
schemes:
- flows:
  - authorizationUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token
  - authorizationUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/auth
    flow: implicit
  - flow: password
    tokenUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token
  issuer: https://identity-prod.picarro.com/auth/realms/picarro
  name: PicarroIdentityOIDC
  source: well-known/picarro-openid-configuration.json
scope_count: 9
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- web-origins
- microprofile-jwt
scopes:
- description: OpenID Connect authentication; requests an ID token.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Standard OIDC profile claims (name, given_name, family_name, preferred_username).
  flows:
  - authorizationCode
  - implicit
  - password
  scope: profile
- description: Standard OIDC email claim.
  flows:
  - authorizationCode
  - implicit
  - password
  scope: email
- description: Standard OIDC address claim.
  flows:
  - authorizationCode
  - implicit
  - password
  scope: address
- description: Standard OIDC phone_number claims.
  flows:
  - authorizationCode
  - implicit
  - password
  scope: phone
- description: Keycloak realm/client role mappings in the access token.
  flows:
  - authorizationCode
  - password
  - clientCredentials
  scope: roles
- description: Issues a refresh token usable while the user is offline.
  flows:
  - authorizationCode
  - password
  scope: offline_access
- description: Keycloak scope that injects allowed CORS web origins into the token.
  flows:
  - authorizationCode
  - implicit
  scope: web-origins
- description: Keycloak scope adding MicroProfile JWT claims (upn, groups).
  flows:
  - authorizationCode
  - clientCredentials
  scope: microprofile-jwt
slug: picarro-scopes
source_filename: picarro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://identity-prod.picarro.com/auth/realms/picarro/.well-known/openid-configuration\nnotes: >-\n  Picarro publishes no OpenAPI with oauth2 securitySchemes. These scopes are the\n  scopes_supported list advertised anonymously by the Keycloak realm that fronts the\n  P-Cubed cloud platform. They are the stock Keycloak/OIDC scope set — Picarro publishes\n  no product-specific API scope reference, and no public scopes documentation page was\n  found.\nschemes:\n  - name: PicarroIdentityOIDC\n    source: well-known/picarro-openid-configuration.json\n    issuer: https://identity-prod.picarro.com/auth/realms/picarro\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/auth\n        tokenUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token\n      - flow: implicit\n        authorizationUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/auth\n\
  \      - flow: password\n        tokenUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token\n      - flow: clientCredentials\n        tokenUrl: https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; requests an ID token.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/picarro-openid-configuration.json]\n  - scope: profile\n    description: Standard OIDC profile claims (name, given_name, family_name, preferred_username).\n    flows: [authorizationCode, implicit, password]\n    sources: [well-known/picarro-openid-configuration.json]\n  - scope: email\n    description: Standard OIDC email claim.\n    flows: [authorizationCode, implicit, password]\n    sources: [well-known/picarro-openid-configuration.json]\n  - scope: address\n    description: Standard OIDC address claim.\n    flows: [authorizationCode, implicit, password]\n    sources:\
  \ [well-known/picarro-openid-configuration.json]\n  - scope: phone\n    description: Standard OIDC phone_number claims.\n    flows: [authorizationCode, implicit, password]\n    sources: [well-known/picarro-openid-configuration.json]\n  - scope: roles\n    description: Keycloak realm/client role mappings in the access token.\n    flows: [authorizationCode, password, clientCredentials]\n    sources: [well-known/picarro-openid-configuration.json]\n  - scope: offline_access\n    description: Issues a refresh token usable while the user is offline.\n    flows: [authorizationCode, password]\n    sources: [well-known/picarro-openid-configuration.json]\n  - scope: web-origins\n    description: Keycloak scope that injects allowed CORS web origins into the token.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/picarro-openid-configuration.json]\n  - scope: microprofile-jwt\n    description: Keycloak scope adding MicroProfile JWT claims (upn, groups).\n    flows: [authorizationCode,\
  \ clientCredentials]\n    sources: [well-known/picarro-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://identity-prod.picarro.com/auth/realms/picarro/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picarro/refs/heads/main/scopes/picarro-scopes.yml
summary_line: 9 scopes · authorizationCode/implicit/password/clientCredentials
tags:
- Company
- Gas Detection
- Environmental Monitoring
- Emissions
- Methane
- Greenhouse Gas
- Scientific Instruments
- Semiconductors
- Industrial IoT
- Sensors
- Analytics
- gRPC
token_urls:
- https://identity-prod.picarro.com/auth/realms/picarro/protocol/openid-connect/token
---
