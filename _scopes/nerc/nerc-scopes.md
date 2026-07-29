---
authorization_urls:
- https://www.eisac.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Nerc Scopes
name_suffix: OAuth Scopes
note: NERC itself publishes no OAuth surface and no scope reference - there is no developer portal, no API documentation and no scopes page anywhere on nerc.com. The only OAuth2 authorization server in NERC's estate is the one fronting the Electricity Information Sharing and Analysis Center (E-ISAC), which NERC operates on Salesforce Experience Cloud. The scope list below is transcribed VERBATIM from that issuer's anonymous OIDC discovery document; it is the Salesforce platform's stock scope set advertised by the E-ISAC issuer, NOT a NERC-defined or NERC-documented permission model. No NERC page documents any of these scopes, there is no self-serve client registration for outside developers, and every resource they would authorize is membership-gated (https://www.eisac.com/services/data/v62.0 -> HTTP 401 INVALID_SESSION_ID). Descriptions are supplied only for the scopes defined by OpenID Connect Core 1.0 / RFC 6749; platform scopes are left undescribed rather than glossed.
overview: 'NERC publishes 36 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the NERC API on a user''s behalf.


  Tokens are issued from https://www.eisac.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NERC
provider_slug: nerc
schemes:
- flows:
  - authorizationUrl: https://www.eisac.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.eisac.com/services/oauth2/token
  - authorizationUrl: https://www.eisac.com/services/oauth2/authorize
    flow: implicit
  gated: true
  issuer: https://www.eisac.com
  name: E-ISAC OpenID Connect
  platform: Salesforce Experience Cloud
  source: https://www.eisac.com/.well-known/openid-configuration
scope_count: 36
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- refresh_token
- id
- api
- web
- full
- content
- lightning
- visualforce
- custom_permissions
- chatter_api
- chatbot_api
- interaction_api
- wave_api
- eclair_api
- pardot_api
- scrt_api
- sfap_api
- einstein_gpt_api
- mcp_api
- user_registration_api
- pwdless_login_api
- forgot_password
- data_cloud_user_claims
- cdp_api
- cdp_ingest_api
- cdp_query_api
- cdp_profile_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
scopes:
- description: Request an ID Token (OpenID Connect Core 1.0).
  flows: []
  scope: openid
- description: Access to the end-user's default profile claims (OpenID Connect Core 1.0).
  flows: []
  scope: profile
- description: Access to the email and email_verified claims (OpenID Connect Core 1.0).
  flows: []
  scope: email
- description: Access to the address claim (OpenID Connect Core 1.0).
  flows: []
  scope: address
- description: Access to the phone_number and phone_number_verified claims (OpenID Connect Core 1.0).
  flows: []
  scope: phone
- description: Request a refresh token for access when the user is not present (OpenID Connect Core 1.0).
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: refresh_token
- description: ''
  flows: []
  scope: id
- description: ''
  flows: []
  scope: api
- description: ''
  flows: []
  scope: web
- description: ''
  flows: []
  scope: full
- description: ''
  flows: []
  scope: content
- description: ''
  flows: []
  scope: lightning
- description: ''
  flows: []
  scope: visualforce
- description: ''
  flows: []
  scope: custom_permissions
- description: ''
  flows: []
  scope: chatter_api
- description: ''
  flows: []
  scope: chatbot_api
- description: ''
  flows: []
  scope: interaction_api
- description: ''
  flows: []
  scope: wave_api
- description: ''
  flows: []
  scope: eclair_api
- description: ''
  flows: []
  scope: pardot_api
- description: ''
  flows: []
  scope: scrt_api
- description: ''
  flows: []
  scope: sfap_api
- description: ''
  flows: []
  scope: einstein_gpt_api
- description: ''
  flows: []
  scope: mcp_api
- description: ''
  flows: []
  scope: user_registration_api
- description: ''
  flows: []
  scope: pwdless_login_api
- description: ''
  flows: []
  scope: forgot_password
- description: ''
  flows: []
  scope: data_cloud_user_claims
- description: ''
  flows: []
  scope: cdp_api
- description: ''
  flows: []
  scope: cdp_ingest_api
- description: ''
  flows: []
  scope: cdp_query_api
- description: ''
  flows: []
  scope: cdp_profile_api
- description: ''
  flows: []
  scope: cdp_segment_api
- description: ''
  flows: []
  scope: cdp_identityresolution_api
- description: ''
  flows: []
  scope: cdp_calculated_insight_api
slug: nerc-scopes
source_filename: nerc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://www.eisac.com/.well-known/openid-configuration\ncaptured: well-known/nerc-eisac-openid-configuration.json\ndocs: null\nnote: >-\n  NERC itself publishes no OAuth surface and no scope reference - there is no\n  developer portal, no API documentation and no scopes page anywhere on\n  nerc.com. The only OAuth2 authorization server in NERC's estate is the one\n  fronting the Electricity Information Sharing and Analysis Center (E-ISAC),\n  which NERC operates on Salesforce Experience Cloud. The scope list below is\n  transcribed VERBATIM from that issuer's anonymous OIDC discovery document; it\n  is the Salesforce platform's stock scope set advertised by the E-ISAC issuer,\n  NOT a NERC-defined or NERC-documented permission model. No NERC page documents\n  any of these scopes, there is no self-serve client registration for outside\n  developers, and every resource they would authorize is membership-gated\n  (https://www.eisac.com/services/data/v62.0\
  \ -> HTTP 401 INVALID_SESSION_ID).\n  Descriptions are supplied only for the scopes defined by OpenID Connect Core\n  1.0 / RFC 6749; platform scopes are left undescribed rather than glossed.\nschemes:\n- name: E-ISAC OpenID Connect\n  issuer: https://www.eisac.com\n  source: https://www.eisac.com/.well-known/openid-configuration\n  platform: Salesforce Experience Cloud\n  gated: true\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.eisac.com/services/oauth2/authorize\n    tokenUrl: https://www.eisac.com/services/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://www.eisac.com/services/oauth2/authorize\nscope_count: 36\nscopes:\n- scope: openid\n  description: Request an ID Token (OpenID Connect Core 1.0).\n  standard: openid-connect\n- scope: profile\n  description: Access to the end-user's default profile claims (OpenID Connect Core\n    1.0).\n  standard: openid-connect\n- scope: email\n  description: Access to the email and email_verified claims\
  \ (OpenID Connect Core 1.0).\n  standard: openid-connect\n- scope: address\n  description: Access to the address claim (OpenID Connect Core 1.0).\n  standard: openid-connect\n- scope: phone\n  description: Access to the phone_number and phone_number_verified claims (OpenID\n    Connect Core 1.0).\n  standard: openid-connect\n- scope: offline_access\n  description: Request a refresh token for access when the user is not present (OpenID\n    Connect Core 1.0).\n  standard: openid-connect\n- scope: refresh_token\n  standard: salesforce-platform\n- scope: id\n  standard: salesforce-platform\n- scope: api\n  standard: salesforce-platform\n- scope: web\n  standard: salesforce-platform\n- scope: full\n  standard: salesforce-platform\n- scope: content\n  standard: salesforce-platform\n- scope: lightning\n  standard: salesforce-platform\n- scope: visualforce\n  standard: salesforce-platform\n- scope: custom_permissions\n  standard: salesforce-platform\n- scope: chatter_api\n  standard: salesforce-platform\n\
  - scope: chatbot_api\n  standard: salesforce-platform\n- scope: interaction_api\n  standard: salesforce-platform\n- scope: wave_api\n  standard: salesforce-platform\n- scope: eclair_api\n  standard: salesforce-platform\n- scope: pardot_api\n  standard: salesforce-platform\n- scope: scrt_api\n  standard: salesforce-platform\n- scope: sfap_api\n  standard: salesforce-platform\n- scope: einstein_gpt_api\n  standard: salesforce-platform\n- scope: mcp_api\n  standard: salesforce-platform\n- scope: user_registration_api\n  standard: salesforce-platform\n- scope: pwdless_login_api\n  standard: salesforce-platform\n- scope: forgot_password\n  standard: salesforce-platform\n- scope: data_cloud_user_claims\n  standard: salesforce-platform\n- scope: cdp_api\n  standard: salesforce-platform\n- scope: cdp_ingest_api\n  standard: salesforce-platform\n- scope: cdp_query_api\n  standard: salesforce-platform\n- scope: cdp_profile_api\n  standard: salesforce-platform\n- scope: cdp_segment_api\n  standard:\
  \ salesforce-platform\n- scope: cdp_identityresolution_api\n  standard: salesforce-platform\n- scope: cdp_calculated_insight_api\n  standard: salesforce-platform\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nerc/refs/heads/main/scopes/nerc-scopes.yml
summary_line: 36 scopes · authorizationCode/implicit
tags:
- Energy
- United States
- Canada
- Electricity
- Grid
- Regulator
- Government
- Reliability
- Bulk Power System
- Critical Infrastructure
- Cyber Security
- Energy Markets
- Compliance
token_urls:
- https://www.eisac.com/services/oauth2/token
---
