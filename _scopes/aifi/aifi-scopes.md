---
authorization_urls:
- https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Aifi Scopes
name_suffix: OAuth Scopes
note: These are the scopes advertised by AiFi's Keycloak realm `aifi` in its OIDC discovery document — the identity provider in front of docs.aifi.com and partners.aifi.com. They are the standard OIDC/Keycloak realm scopes, NOT application scopes for the OASIS retailer APIs. AiFi publishes no public scope or permission reference, and no OASIS API scope is asserted here. Recorded because they are the only authorization surface AiFi exposes anonymously.
overview: 'AiFi publishes 10 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AiFi API on a user''s behalf.


  Tokens are issued from https://auth.aifi.com/realms/aifi/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AiFi
provider_slug: aifi
schemes:
- flows:
  - authorizationUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth/device
    flow: deviceCode
    tokenUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token
  issuer: https://auth.aifi.com/realms/aifi
  name: aifi-keycloak
  source: well-known/aifi-openid-configuration.json
scope_count: 10
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- acr
- web-origins
- microprofile-jwt
scopes:
- description: Required OpenID Connect scope; requests an ID token.
  flows: []
  scope: openid
- description: Basic profile claims (name, given_name, family_name, preferred_username).
  flows: []
  scope: profile
- description: Email address and email_verified claim.
  flows: []
  scope: email
- description: Physical address claim.
  flows: []
  scope: address
- description: Phone number claims.
  flows: []
  scope: phone
- description: Realm and client role mappings for the subject.
  flows: []
  scope: roles
- description: Issues a refresh token usable while the user is offline.
  flows: []
  scope: offline_access
- description: Authentication context class reference; carries the acr claim.
  flows: []
  scope: acr
- description: Keycloak scope that adds allowed CORS web origins to the token.
  flows: []
  scope: web-origins
- description: MicroProfile JWT claim set (upn, groups) for Java service consumers.
  flows: []
  scope: microprofile-jwt
slug: aifi-scopes
source_filename: aifi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://auth.aifi.com/realms/aifi/.well-known/openid-configuration\ndocs: null\nscope: identity-provider-realm\nnote: >-\n  These are the scopes advertised by AiFi's Keycloak realm `aifi` in its OIDC\n  discovery document — the identity provider in front of docs.aifi.com and\n  partners.aifi.com. They are the standard OIDC/Keycloak realm scopes, NOT\n  application scopes for the OASIS retailer APIs. AiFi publishes no public scope or\n  permission reference, and no OASIS API scope is asserted here. Recorded because\n  they are the only authorization surface AiFi exposes anonymously.\nschemes:\n- name: aifi-keycloak\n  source: well-known/aifi-openid-configuration.json\n  issuer: https://auth.aifi.com/realms/aifi\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth\n    tokenUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token\n  - flow: clientCredentials\n\
  \    tokenUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/auth/device\n    tokenUrl: https://auth.aifi.com/realms/aifi/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope; requests an ID token.\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims (name, given_name, family_name, preferred_username).\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: email\n  description: Email address and email_verified claim.\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: address\n  description: Physical address claim.\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: phone\n  description: Phone number claims.\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: roles\n  description: Realm and client role mappings\
  \ for the subject.\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: offline_access\n  description: Issues a refresh token usable while the user is offline.\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: acr\n  description: Authentication context class reference; carries the acr claim.\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: web-origins\n  description: Keycloak scope that adds allowed CORS web origins to the token.\n  sources: [well-known/aifi-openid-configuration.json]\n- scope: microprofile-jwt\n  description: MicroProfile JWT claim set (upn, groups) for Java service consumers.\n  sources: [well-known/aifi-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://auth.aifi.com/realms/aifi/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aifi/refs/heads/main/scopes/aifi-scopes.yml
summary_line: 10 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Computer Vision
- Retail
- Autonomous Checkout
- Spatial Intelligence
- Artificial Intelligence
- Analytics
- Identity
- Fraud Prevention
- Point of Sale
token_urls:
- https://auth.aifi.com/realms/aifi/protocol/openid-connect/token
---
