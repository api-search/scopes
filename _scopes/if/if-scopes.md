---
authorization_urls: []
description: ''
docs: https://developer.integrated.finance/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: If Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'IF publishes 11 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the IF API on a user''s behalf.


  Tokens are issued from https://account.integrated.finance/auth/realms/ifp/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IF
provider_slug: if
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://account.integrated.finance/auth/realms/ifp/protocol/openid-connect/token
  name: OAuth2
  source: https://account.integrated.finance/auth/realms/ifp/.well-known/openid-configuration
scope_count: 11
scope_names:
- openid
- api
- profile
- email
- address
- phone
- roles
- offline_access
- microprofile-jwt
- acr
- web-origins
scopes:
- description: OpenID Connect authentication; required to receive an ID token.
  flows: []
  scope: openid
- description: Access to the Integrated Finance platform API surface.
  flows: []
  scope: api
- description: Basic profile claims for the authenticated subject.
  flows: []
  scope: profile
- description: Email address claim for the authenticated subject.
  flows: []
  scope: email
- description: Address claim for the authenticated subject.
  flows: []
  scope: address
- description: Phone-number claim for the authenticated subject.
  flows: []
  scope: phone
- description: Realm and client role memberships for the subject.
  flows: []
  scope: roles
- description: Issue a refresh token for offline / long-lived access.
  flows: []
  scope: offline_access
- description: MicroProfile JWT claims (groups, upn) for service-to-service tokens.
  flows: []
  scope: microprofile-jwt
- description: Authentication Context Class Reference claim.
  flows: []
  scope: acr
- description: Allowed CORS web origins for the client.
  flows: []
  scope: web-origins
slug: if-scopes
source_filename: if-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/if-openid-configuration.json\ndocs: https://developer.integrated.finance/docs/authentication\nschemes:\n- name: OAuth2\n  source: https://account.integrated.finance/auth/realms/ifp/.well-known/openid-configuration\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.integrated.finance/auth/realms/ifp/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required to receive an ID token.\n  sources: [well-known/if-openid-configuration.json]\n- scope: api\n  description: Access to the Integrated Finance platform API surface.\n  sources: [well-known/if-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims for the authenticated subject.\n  sources: [well-known/if-openid-configuration.json]\n- scope: email\n  description: Email address claim for the authenticated subject.\n  sources: [well-known/if-openid-configuration.json]\n\
  - scope: address\n  description: Address claim for the authenticated subject.\n  sources: [well-known/if-openid-configuration.json]\n- scope: phone\n  description: Phone-number claim for the authenticated subject.\n  sources: [well-known/if-openid-configuration.json]\n- scope: roles\n  description: Realm and client role memberships for the subject.\n  sources: [well-known/if-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token for offline / long-lived access.\n  sources: [well-known/if-openid-configuration.json]\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims (groups, upn) for service-to-service tokens.\n  sources: [well-known/if-openid-configuration.json]\n- scope: acr\n  description: Authentication Context Class Reference claim.\n  sources: [well-known/if-openid-configuration.json]\n- scope: web-origins\n  description: Allowed CORS web origins for the client.\n  sources: [well-known/if-openid-configuration.json]\nnotes: >-\n  Scopes\
  \ are the Keycloak realm (\"ifp\") supported scopes read from the live OIDC\n  discovery documents for the production and sandbox authorization servers. IF uses\n  a client-credentials (service-account) model; per-resource authorization is\n  carried by realm/client roles rather than fine-grained OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/if/refs/heads/main/scopes/if-scopes.yml
summary_line: 11 scopes · clientCredentials
tags:
- Company
- Financial Services
- Embedded Finance
- Banking as a Service
- Payments
- Cards
- Foreign Exchange
- Compliance
- Open Banking
- API
token_urls:
- https://account.integrated.finance/auth/realms/ifp/protocol/openid-connect/token
---
