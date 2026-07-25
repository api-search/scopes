---
authorization_urls:
- https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Onetick Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OneTick (OneMarketData) publishes 28 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the OneTick (OneMarketData) API on a user''s behalf.


  Tokens are issued from https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OneTick (OneMarketData)
provider_slug: onetick
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token
  - authorizationUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token
  name: OneTickCloudOAuth2
  source: well-known/onetick-openid-configuration.json
scope_count: 28
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- roles
- acr
- basic
- web-origins
- microprofile-jwt
- service_account
- OMDKeyScope
- truetick
- client_group
- aws-integration
- acf_test_app_1_aud
- ccf_test_app_1_aud
- ccf_test_app_2_aud
- ccf_test_app_3_aud
- ccf_test_app_4_aud
- ccf_test_app_5_aud
- ccf_axos_app_1_aud
- ccf_alphadyne_app_1_aud
- ccf_sigma_logic_inc_app_1_aud
- ccf_omd_monitor_app_1_aud
- ccf_omd_ps_app_1_aud
- ccf_omd_mngd_svc_app_1_aud
scopes:
- description: OpenID Connect authentication (standard OIDC scope)
  flows: []
  scope: openid
- description: Access to profile claims (standard OIDC scope)
  flows: []
  scope: profile
- description: Access to email claims (standard OIDC scope)
  flows: []
  scope: email
- description: Access to address claims (standard OIDC scope)
  flows: []
  scope: address
- description: Access to phone claims (standard OIDC scope)
  flows: []
  scope: phone
- description: Request a refresh token for offline access (standard OAuth2/OIDC scope)
  flows: []
  scope: offline_access
- description: Keycloak realm/client role claims
  flows: []
  scope: roles
- description: Keycloak authentication context class reference claim
  flows: []
  scope: acr
- description: Keycloak basic claim set
  flows: []
  scope: basic
- description: Keycloak allowed web origins
  flows: []
  scope: web-origins
- description: MicroProfile JWT claim mapping (Keycloak built-in)
  flows: []
  scope: microprofile-jwt
- description: Keycloak service-account (client-credentials) scope
  flows: []
  scope: service_account
- description: ''
  flows: []
  scope: OMDKeyScope
- description: ''
  flows: []
  scope: truetick
- description: ''
  flows: []
  scope: client_group
- description: ''
  flows: []
  scope: aws-integration
- description: ''
  flows: []
  scope: acf_test_app_1_aud
- description: ''
  flows: []
  scope: ccf_test_app_1_aud
- description: ''
  flows: []
  scope: ccf_test_app_2_aud
- description: ''
  flows: []
  scope: ccf_test_app_3_aud
- description: ''
  flows: []
  scope: ccf_test_app_4_aud
- description: ''
  flows: []
  scope: ccf_test_app_5_aud
- description: ''
  flows: []
  scope: ccf_axos_app_1_aud
- description: ''
  flows: []
  scope: ccf_alphadyne_app_1_aud
- description: ''
  flows: []
  scope: ccf_sigma_logic_inc_app_1_aud
- description: ''
  flows: []
  scope: ccf_omd_monitor_app_1_aud
- description: ''
  flows: []
  scope: ccf_omd_ps_app_1_aud
- description: ''
  flows: []
  scope: ccf_omd_mngd_svc_app_1_aud
slug: onetick-scopes
source_filename: onetick-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://cloud-auth.parent.onetick.com/realms/OMD/.well-known/openid-configuration\nnotes: OneTick publishes no public scopes reference page; this list is the\n  scopes_supported advertised by the Keycloak OMD realm OIDC discovery document\n  that issues OneTick Cloud WebAPI tokens. Standard OIDC scopes are described per\n  the OpenID Connect specification; realm-specific scopes (OMDKeyScope, truetick,\n  per-customer ccf_*_aud audience scopes) are listed verbatim without invented\n  descriptions.\nschemes:\n- name: OneTickCloudOAuth2\n  source: well-known/onetick-openid-configuration.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/auth\n    tokenUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token\n\
  scopes:\n- scope: openid\n  description: OpenID Connect authentication (standard OIDC scope)\n- scope: profile\n  description: Access to profile claims (standard OIDC scope)\n- scope: email\n  description: Access to email claims (standard OIDC scope)\n- scope: address\n  description: Access to address claims (standard OIDC scope)\n- scope: phone\n  description: Access to phone claims (standard OIDC scope)\n- scope: offline_access\n  description: Request a refresh token for offline access (standard OAuth2/OIDC scope)\n- scope: roles\n  description: Keycloak realm/client role claims\n- scope: acr\n  description: Keycloak authentication context class reference claim\n- scope: basic\n  description: Keycloak basic claim set\n- scope: web-origins\n  description: Keycloak allowed web origins\n- scope: microprofile-jwt\n  description: MicroProfile JWT claim mapping (Keycloak built-in)\n- scope: service_account\n  description: Keycloak service-account (client-credentials) scope\n- scope: OMDKeyScope\n\
  \  description: null\n- scope: truetick\n  description: null\n- scope: client_group\n  description: null\n- scope: aws-integration\n  description: null\n- scope: acf_test_app_1_aud\n  description: null\n- scope: ccf_test_app_1_aud\n  description: null\n- scope: ccf_test_app_2_aud\n  description: null\n- scope: ccf_test_app_3_aud\n  description: null\n- scope: ccf_test_app_4_aud\n  description: null\n- scope: ccf_test_app_5_aud\n  description: null\n- scope: ccf_axos_app_1_aud\n  description: null\n- scope: ccf_alphadyne_app_1_aud\n  description: null\n- scope: ccf_sigma_logic_inc_app_1_aud\n  description: null\n- scope: ccf_omd_monitor_app_1_aud\n  description: null\n- scope: ccf_omd_ps_app_1_aud\n  description: null\n- scope: ccf_omd_mngd_svc_app_1_aud\n  description: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onetick/refs/heads/main/scopes/onetick-scopes.yml
summary_line: 28 scopes · clientCredentials/authorizationCode
tags:
- Financial
- Market Data
- Tick Data
- Historical Data
- Trading
- Analytics
- Surveillance
- Time Series
- Equities
- Options
token_urls:
- https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token
---
