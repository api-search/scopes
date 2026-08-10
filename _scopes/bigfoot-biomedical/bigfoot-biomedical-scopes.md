---
authorization_urls:
- https://clinichub.bigfootbiomedical.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Bigfoot Biomedical Scopes
name_suffix: OAuth Scopes
note: Bigfoot Biomedical publishes no OAuth scope reference and no API. These scopes are the scopes_supported list advertised by the Salesforce Experience Cloud identity provider behind the Bigfoot Clinic Hub healthcare-professional portal, captured verbatim from that org's OIDC discovery document. They are Salesforce PLATFORM scopes, not scopes of a Bigfoot product API, and no Bigfoot documentation describes them. Recorded for completeness with their provenance stated; do not read this as a Bigfoot authorization model.
overview: 'Bigfoot Biomedical publishes 36 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bigfoot Biomedical API on a user''s behalf.


  Tokens are issued from https://clinichub.bigfootbiomedical.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bigfoot Biomedical
provider_slug: bigfoot-biomedical
schemes:
- flows:
  - authorizationUrl: https://clinichub.bigfootbiomedical.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://clinichub.bigfootbiomedical.com/services/oauth2/token
  - authorizationUrl: https://clinichub.bigfootbiomedical.com/services/oauth2/authorize
    flow: implicit
  name: bigfoot-clinic-hub-oidc
  platform: Salesforce Experience Cloud
  source: well-known/bigfoot-biomedical-openid-configuration.json
scope_count: 36
scope_names:
- address
- api
- cdp_api
- cdp_calculated_insight_api
- cdp_identityresolution_api
- cdp_ingest_api
- cdp_profile_api
- cdp_query_api
- cdp_segment_api
- chatbot_api
- chatter_api
- content
- custom_permissions
- data_cloud_user_claims
- eclair_api
- einstein_gpt_api
- email
- forgot_password
- full
- id
- interaction_api
- lightning
- mcp_api
- offline_access
- openid
- pardot_api
- phone
- profile
- pwdless_login_api
- refresh_token
- scrt_api
- sfap_api
- user_registration_api
- visualforce
- wave_api
- web
scopes:
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: address
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: cdp_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: cdp_calculated_insight_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: cdp_identityresolution_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: cdp_ingest_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: cdp_profile_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: cdp_query_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: cdp_segment_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: chatbot_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: chatter_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: content
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: custom_permissions
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: data_cloud_user_claims
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: eclair_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: einstein_gpt_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: forgot_password
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: full
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: id
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: interaction_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: lightning
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: mcp_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: offline_access
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: pardot_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: pwdless_login_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: refresh_token
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: scrt_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: sfap_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: user_registration_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: visualforce
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: wave_api
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: web
slug: bigfoot-biomedical-scopes
source_filename: bigfoot-biomedical-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://clinichub.bigfootbiomedical.com/.well-known/openid-configuration\nnote: Bigfoot Biomedical publishes no OAuth scope reference and no API. These scopes are the scopes_supported\n  list advertised by the Salesforce Experience Cloud identity provider behind the Bigfoot Clinic Hub healthcare-professional\n  portal, captured verbatim from that org's OIDC discovery document. They are Salesforce PLATFORM scopes,\n  not scopes of a Bigfoot product API, and no Bigfoot documentation describes them. Recorded for completeness\n  with their provenance stated; do not read this as a Bigfoot authorization model.\ndocs: null\nschemes:\n- name: bigfoot-clinic-hub-oidc\n  source: well-known/bigfoot-biomedical-openid-configuration.json\n  platform: Salesforce Experience Cloud\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clinichub.bigfootbiomedical.com/services/oauth2/authorize\n    tokenUrl: https://clinichub.bigfootbiomedical.com/services/oauth2/token\n\
  \  - flow: implicit\n    authorizationUrl: https://clinichub.bigfootbiomedical.com/services/oauth2/authorize\nscopes:\n- scope: address\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: cdp_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: cdp_calculated_insight_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: cdp_identityresolution_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: cdp_ingest_api\n  description: null\n  flows:\n\
  \  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: cdp_profile_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: cdp_query_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: cdp_segment_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: chatbot_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: chatter_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: content\n  description: null\n  flows:\n  - authorizationCode\n\
  \  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: custom_permissions\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: data_cloud_user_claims\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: eclair_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: einstein_gpt_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: email\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: forgot_password\n  description: null\n  flows:\n  - authorizationCode\n\
  \  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: full\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: id\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: interaction_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: lightning\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: mcp_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: offline_access\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n\
  - scope: openid\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: pardot_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: phone\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: profile\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: pwdless_login_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: refresh_token\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: scrt_api\n  description:\
  \ null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: sfap_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: user_registration_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: visualforce\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: wave_api\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\n- scope: web\n  description: null\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\nx-evidence:\n- url: https://clinichub.bigfootbiomedical.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  fetched: '2026-08-07'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigfoot-biomedical/refs/heads/main/scopes/bigfoot-biomedical-scopes.yml
summary_line: 36 scopes · authorizationCode/implicit
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Diabetes
- Insulin Management
- Continuous Glucose Monitoring
- Connected Devices
- Acquired
token_urls:
- https://clinichub.bigfootbiomedical.com/services/oauth2/token
---
