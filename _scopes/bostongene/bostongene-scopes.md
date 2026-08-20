---
authorization_urls:
- https://bostongene.my.site.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bostongene Scopes
name_suffix: OAuth Scopes
note: These are the `scopes_supported` advertised verbatim by the OpenID Connect discovery document on BostonGene's customer-portal host. They are the standard Salesforce Experience Cloud platform scope set, not a BostonGene-authored API permission model — BostonGene publishes no developer API and no scope reference page. Recorded because the document is genuinely served from a BostonGene host; do NOT read this list as a BostonGene API authorization design.
overview: 'BostonGene publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BostonGene API on a user''s behalf.


  Tokens are issued from https://bostongene.my.site.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BostonGene
provider_slug: bostongene
schemes:
- flows:
  - authorizationUrl: https://bostongene.my.site.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://bostongene.my.site.com/services/oauth2/token
  issuer: https://bostongene.my.site.com
  name: BostonGene Customer Portal (OIDC)
  source: well-known/bostongene-openid-configuration.json
scope_count: 36
scope_names:
- openid
- profile
- email
- address
- phone
- id
- api
- web
- full
- refresh_token
- offline_access
- custom_permissions
- lightning
- visualforce
- content
- chatter_api
- chatbot_api
- wave_api
- eclair_api
- pardot_api
- interaction_api
- user_registration_api
- pwdless_login_api
- forgot_password
- scrt_api
- sfap_api
- mcp_api
- einstein_gpt_api
- data_cloud_user_claims
- cdp_api
- cdp_query_api
- cdp_ingest_api
- cdp_profile_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
scopes:
- description: OpenID Connect — request an ID token
  flows: []
  scope: openid
- description: Standard OIDC profile claims
  flows: []
  scope: profile
- description: Standard OIDC email claims
  flows: []
  scope: email
- description: Standard OIDC address claim
  flows: []
  scope: address
- description: Standard OIDC phone claims
  flows: []
  scope: phone
- description: Identity URL access
  flows: []
  scope: id
- description: Access the platform REST/SOAP APIs on behalf of the user
  flows: []
  scope: api
- description: Web session access
  flows: []
  scope: web
- description: Full access to all data accessible to the user
  flows: []
  scope: full
- description: Issue a refresh token
  flows: []
  scope: refresh_token
- description: Offline access (refresh token equivalent)
  flows: []
  scope: offline_access
- description: Include the user's custom permissions in the token response
  flows: []
  scope: custom_permissions
- description: Access Lightning applications
  flows: []
  scope: lightning
- description: Access Visualforce pages
  flows: []
  scope: visualforce
- description: Access content/files
  flows: []
  scope: content
- description: Access the Chatter/Connect REST API
  flows: []
  scope: chatter_api
- description: Access the chatbot API
  flows: []
  scope: chatbot_api
- description: Access the analytics (Wave) API
  flows: []
  scope: wave_api
- description: Access the Eclair geodata API
  flows: []
  scope: eclair_api
- description: Access the Pardot marketing automation API
  flows: []
  scope: pardot_api
- description: Access the interaction/flow API
  flows: []
  scope: interaction_api
- description: Access the user registration API
  flows: []
  scope: user_registration_api
- description: Access the passwordless login API
  flows: []
  scope: pwdless_login_api
- description: Access the forgot-password API
  flows: []
  scope: forgot_password
- description: Access the service-cloud real-time API
  flows: []
  scope: scrt_api
- description: Access the platform agent API
  flows: []
  scope: sfap_api
- description: Access the platform Model Context Protocol API surface
  flows: []
  scope: mcp_api
- description: Access the Einstein GPT API
  flows: []
  scope: einstein_gpt_api
- description: Include Data Cloud user claims
  flows: []
  scope: data_cloud_user_claims
- description: Access the Customer Data Platform API
  flows: []
  scope: cdp_api
- description: Access the CDP query API
  flows: []
  scope: cdp_query_api
- description: Access the CDP ingestion API
  flows: []
  scope: cdp_ingest_api
- description: Access the CDP profile API
  flows: []
  scope: cdp_profile_api
- description: Access the CDP segmentation API
  flows: []
  scope: cdp_segment_api
- description: Access the CDP identity resolution API
  flows: []
  scope: cdp_identityresolution_api
- description: Access the CDP calculated insights API
  flows: []
  scope: cdp_calculated_insight_api
slug: bostongene-scopes
source_filename: bostongene-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://bostongene.my.site.com/.well-known/openid-configuration\nprovider_specific: false\nnote: >-\n  These are the `scopes_supported` advertised verbatim by the OpenID Connect\n  discovery document on BostonGene's customer-portal host. They are the standard\n  Salesforce Experience Cloud platform scope set, not a BostonGene-authored API\n  permission model — BostonGene publishes no developer API and no scope reference\n  page. Recorded because the document is genuinely served from a BostonGene host;\n  do NOT read this list as a BostonGene API authorization design.\nschemes:\n- name: BostonGene Customer Portal (OIDC)\n  source: well-known/bostongene-openid-configuration.json\n  issuer: https://bostongene.my.site.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://bostongene.my.site.com/services/oauth2/authorize\n    tokenUrl: https://bostongene.my.site.com/services/oauth2/token\nscopes:\n- scope: openid\n\
  \  description: OpenID Connect — request an ID token\n- scope: profile\n  description: Standard OIDC profile claims\n- scope: email\n  description: Standard OIDC email claims\n- scope: address\n  description: Standard OIDC address claim\n- scope: phone\n  description: Standard OIDC phone claims\n- scope: id\n  description: Identity URL access\n- scope: api\n  description: Access the platform REST/SOAP APIs on behalf of the user\n- scope: web\n  description: Web session access\n- scope: full\n  description: Full access to all data accessible to the user\n- scope: refresh_token\n  description: Issue a refresh token\n- scope: offline_access\n  description: Offline access (refresh token equivalent)\n- scope: custom_permissions\n  description: Include the user's custom permissions in the token response\n- scope: lightning\n  description: Access Lightning applications\n- scope: visualforce\n  description: Access Visualforce pages\n- scope: content\n  description: Access content/files\n- scope:\
  \ chatter_api\n  description: Access the Chatter/Connect REST API\n- scope: chatbot_api\n  description: Access the chatbot API\n- scope: wave_api\n  description: Access the analytics (Wave) API\n- scope: eclair_api\n  description: Access the Eclair geodata API\n- scope: pardot_api\n  description: Access the Pardot marketing automation API\n- scope: interaction_api\n  description: Access the interaction/flow API\n- scope: user_registration_api\n  description: Access the user registration API\n- scope: pwdless_login_api\n  description: Access the passwordless login API\n- scope: forgot_password\n  description: Access the forgot-password API\n- scope: scrt_api\n  description: Access the service-cloud real-time API\n- scope: sfap_api\n  description: Access the platform agent API\n- scope: mcp_api\n  description: Access the platform Model Context Protocol API surface\n- scope: einstein_gpt_api\n  description: Access the Einstein GPT API\n- scope: data_cloud_user_claims\n  description: Include\
  \ Data Cloud user claims\n- scope: cdp_api\n  description: Access the Customer Data Platform API\n- scope: cdp_query_api\n  description: Access the CDP query API\n- scope: cdp_ingest_api\n  description: Access the CDP ingestion API\n- scope: cdp_profile_api\n  description: Access the CDP profile API\n- scope: cdp_segment_api\n  description: Access the CDP segmentation API\n- scope: cdp_identityresolution_api\n  description: Access the CDP identity resolution API\n- scope: cdp_calculated_insight_api\n  description: Access the CDP calculated insights API\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://bostongene.my.site.com/.well-known/openid-configuration\n  http_status: 200\n  scope_count: 37\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bostongene/refs/heads/main/scopes/bostongene-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Company
- Healthcare
- Oncology
- Precision Medicine
- Genomics
- Bioinformatics
- Artificial Intelligence
- Diagnostics
- Life Sciences
- Clinical Laboratory
token_urls:
- https://bostongene.my.site.com/services/oauth2/token
---
