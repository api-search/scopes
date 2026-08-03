---
authorization_urls:
- https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/auth
- https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Chromacode Scopes
name_suffix: OAuth Scopes
note: ChromaCode publishes no scopes or permissions reference page. These scopes are the scopes_supported values advertised by the provider's own Keycloak OpenID Connect discovery documents for the two ChromaCode Cloud realms. The two application-specific scopes (chromacloud, chromacloud:service_account) exist only on the "apps" realm; the rest are Keycloak's standard OIDC client scopes. No scope-level documentation is published, so descriptions below are the standard OIDC/Keycloak meanings and are marked as such — none are ChromaCode-authored.
overview: 'ChromaCode publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ChromaCode API on a user''s behalf.


  Tokens are issued from https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ChromaCode
provider_slug: chromacode
schemes:
- flows:
  - authorizationUrl: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token
  name: ChromaCodeCloudOIDC
  realm: apps
  source: well-known/chromacode-openid-configuration-apps.json
- flows:
  - authorizationUrl: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/token
  name: ChromaCodeCloudUserRealmOIDC
  realm: cloud
  source: well-known/chromacode-openid-configuration-cloud.json
scope_count: 12
scope_names:
- chromacloud
- chromacloud:service_account
- openid
- profile
- email
- address
- phone
- offline_access
- roles
- web-origins
- microprofile-jwt
- acr
scopes:
- description: ChromaCode Cloud application scope (provider-specific; no published definition).
  flows: []
  scope: chromacloud
- description: ChromaCode Cloud service-account scope for machine clients (provider-specific; no published definition).
  flows: []
  scope: chromacloud:service_account
- description: Standard OIDC scope requesting an ID token.
  flows: []
  scope: openid
- description: Standard OIDC scope for basic profile claims (name, given_name, family_name, preferred_username).
  flows: []
  scope: profile
- description: Standard OIDC scope for the email and email_verified claims.
  flows: []
  scope: email
- description: Standard OIDC scope for the address claim.
  flows: []
  scope: address
- description: Standard OIDC scope for phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Standard OIDC scope requesting a refresh token usable while the user is offline.
  flows: []
  scope: offline_access
- description: Keycloak client scope adding realm and client role mappings to the token.
  flows: []
  scope: roles
- description: Keycloak client scope adding allowed CORS web origins to the token.
  flows: []
  scope: web-origins
- description: Keycloak client scope emitting MicroProfile JWT claims (upn, groups).
  flows: []
  scope: microprofile-jwt
- description: Keycloak client scope carrying the authentication context class reference.
  flows: []
  scope: acr
slug: chromacode-scopes
source_filename: chromacode-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://openid.chromacodecloud.com/auth/realms/apps/.well-known/openid-configuration\nnote: >-\n  ChromaCode publishes no scopes or permissions reference page. These scopes are the\n  scopes_supported values advertised by the provider's own Keycloak OpenID Connect\n  discovery documents for the two ChromaCode Cloud realms. The two application-specific\n  scopes (chromacloud, chromacloud:service_account) exist only on the \"apps\" realm;\n  the rest are Keycloak's standard OIDC client scopes. No scope-level documentation\n  is published, so descriptions below are the standard OIDC/Keycloak meanings and are\n  marked as such — none are ChromaCode-authored.\nschemes:\n- name: ChromaCodeCloudOIDC\n  realm: apps\n  source: well-known/chromacode-openid-configuration-apps.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/auth\n    tokenUrl:\
  \ https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token\n- name: ChromaCodeCloudUserRealmOIDC\n  realm: cloud\n  source: well-known/chromacode-openid-configuration-cloud.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/auth\n    tokenUrl: https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/token\nscopes:\n- scope: chromacloud\n  description: ChromaCode Cloud application scope (provider-specific; no published definition).\n  provider_specific: true\n  realms:\n  - apps\n  sources:\n  - well-known/chromacode-openid-configuration-apps.json\n- scope: chromacloud:service_account\n  description: ChromaCode Cloud service-account scope for machine clients (provider-specific;\n    no published definition).\n  provider_specific:\
  \ true\n  realms:\n  - apps\n  sources:\n  - well-known/chromacode-openid-configuration-apps.json\n- scope: openid\n  description: Standard OIDC scope requesting an ID token.\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: profile\n  description: Standard OIDC scope for basic profile claims (name, given_name, family_name,\n    preferred_username).\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: email\n  description: Standard OIDC scope for the email and email_verified claims.\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: address\n  description: Standard OIDC scope for the address claim.\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: phone\n  description: Standard OIDC scope for phone_number and phone_number_verified claims.\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: offline_access\n  description: Standard OIDC scope requesting a refresh token usable while the user\n   \
  \ is offline.\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: roles\n  description: Keycloak client scope adding realm and client role mappings to the token.\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: web-origins\n  description: Keycloak client scope adding allowed CORS web origins to the token.\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: microprofile-jwt\n  description: Keycloak client scope emitting MicroProfile JWT claims (upn, groups).\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\n- scope: acr\n  description: Keycloak client scope carrying the authentication context class reference.\n  provider_specific: false\n  realms:\n  - apps\n  - cloud\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://openid.chromacodecloud.com/auth/realms/apps/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chromacode/refs/heads/main/scopes/chromacode-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Company
- Molecular Diagnostics
- Genomics
- Oncology
- PCR
- Life Sciences
- Healthcare
- Bioinformatics
- Clinical Diagnostics
- Cloud Software
token_urls:
- https://openid.chromacodecloud.com/auth/realms/apps/protocol/openid-connect/token
- https://openid.chromacodecloud.com/auth/realms/cloud/protocol/openid-connect/token
---
