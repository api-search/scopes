---
authorization_urls: []
description: ''
docs: https://docs.proemion.com/docs/dataportal/organization_structure/#api-client-management
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Proemion Scopes
name_suffix: OAuth Scopes
note: OpenID Connect realm scopes advertised by the Proemion Keycloak authorization server (scopes_supported). These are the standard OIDC/service-account scopes; fine-grained DataPlatform permissions are governed by the API client's assigned role/organization in the DataPortal rather than by request scopes.
overview: 'Proemion publishes 12 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Proemion API on a user''s behalf.


  Tokens are issued from https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Proemion
provider_slug: proemion
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba/protocol/openid-connect/token
  name: OAuth2
scope_count: 12
scope_names:
- openid
- profile
- email
- roles
- offline_access
- service_account
- basic
- address
- phone
- microprofile-jwt
- web-origins
- acr
scopes:
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: Basic profile claims.
  flows: []
  scope: profile
- description: Email claim.
  flows: []
  scope: email
- description: Realm/client role claims.
  flows: []
  scope: roles
- description: Issue a refresh token for offline access.
  flows: []
  scope: offline_access
- description: Service-account (machine-to-machine) client-credentials access.
  flows: []
  scope: service_account
- description: Basic claim set.
  flows: []
  scope: basic
- description: Address claims.
  flows: []
  scope: address
- description: Phone claims.
  flows: []
  scope: phone
- description: MicroProfile JWT claims (groups/roles).
  flows: []
  scope: microprofile-jwt
- description: Allowed CORS web origins.
  flows: []
  scope: web-origins
- description: Authentication Context Class Reference.
  flows: []
  scope: acr
slug: proemion-scopes
source_filename: proemion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.proemion.com/.well-known/openid-configuration\ndocs: https://docs.proemion.com/docs/dataportal/organization_structure/#api-client-management\nnote: >-\n  OpenID Connect realm scopes advertised by the Proemion Keycloak authorization\n  server (scopes_supported). These are the standard OIDC/service-account scopes;\n  fine-grained DataPlatform permissions are governed by the API client's assigned\n  role/organization in the DataPortal rather than by request scopes.\nschemes:\n- name: OAuth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication.\n- scope: profile\n  description: Basic profile claims.\n- scope: email\n  description: Email claim.\n- scope: roles\n  description: Realm/client role claims.\n- scope: offline_access\n  description:\
  \ Issue a refresh token for offline access.\n- scope: service_account\n  description: Service-account (machine-to-machine) client-credentials access.\n- scope: basic\n  description: Basic claim set.\n- scope: address\n  description: Address claims.\n- scope: phone\n  description: Phone claims.\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims (groups/roles).\n- scope: web-origins\n  description: Allowed CORS web origins.\n- scope: acr\n  description: Authentication Context Class Reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proemion/refs/heads/main/scopes/proemion-scopes.yml
summary_line: 12 scopes · clientCredentials
tags:
- Company
- Telematics
- IoT
- Off-Highway Equipment
- CAN Bus
- Fleet Management
- Machine Data
- OEM
- AEMP
- Construction
- Agriculture
token_urls:
- https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba/protocol/openid-connect/token
---
