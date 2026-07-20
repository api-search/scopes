---
authorization_urls:
- https://developer.gene.com/services/oauth2/authorize
description: ''
docs: https://developer.gene.com/s/api-library
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Genentech Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Genentech publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Genentech API on a user''s behalf.


  Tokens are issued from https://developer.gene.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Genentech
provider_slug: genentech
schemes:
- flows:
  - authorizationUrl: https://developer.gene.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.gene.com/services/oauth2/token
  name: oauth2
  source: well-known/genentech-openid-configuration.json
scope_count: 36
scope_names:
- openid
- profile
- email
- address
- phone
- api
- web
- full
- id
- refresh_token
- offline_access
- lightning
- visualforce
- content
- chatter_api
- user_registration_api
- pwdless_login_api
- forgot_password
- custom_permissions
- interaction_api
- cdp_api
- cdp_ingest_api
- cdp_query_api
- cdp_profile_api
- cdp_segment_api
- cdp_identityresolution_api
- cdp_calculated_insight_api
- data_cloud_user_claims
- einstein_gpt_api
- sfap_api
- mcp_api
- chatbot_api
- wave_api
- eclair_api
- pardot_api
- scrt_api
scopes:
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the user's email address.
  flows: []
  scope: email
- description: Access to the user's address claim.
  flows: []
  scope: address
- description: Access to the user's phone number claim.
  flows: []
  scope: phone
- description: Access to platform REST/SOAP API resources.
  flows: []
  scope: api
- description: Web access to the org on behalf of the user.
  flows: []
  scope: web
- description: Full access to all resources the user can access.
  flows: []
  scope: full
- description: Access to the identity URL service.
  flows: []
  scope: id
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: refresh_token
- description: Maintain access when the user is offline.
  flows: []
  scope: offline_access
- description: Access to Lightning Experience resources.
  flows: []
  scope: lightning
- description: Access to Visualforce pages.
  flows: []
  scope: visualforce
- description: Access to content/file resources.
  flows: []
  scope: content
- description: Access to Chatter REST API resources.
  flows: []
  scope: chatter_api
- description: Self-registration handler API.
  flows: []
  scope: user_registration_api
- description: Passwordless login API.
  flows: []
  scope: pwdless_login_api
- description: Forgot-password flow.
  flows: []
  scope: forgot_password
- description: Access to the user's custom permissions.
  flows: []
  scope: custom_permissions
- description: Interaction Studio / interaction API.
  flows: []
  scope: interaction_api
- description: Data Cloud (CDP) API.
  flows: []
  scope: cdp_api
- description: Data Cloud ingestion API.
  flows: []
  scope: cdp_ingest_api
- description: Data Cloud query API.
  flows: []
  scope: cdp_query_api
- description: Data Cloud profile API.
  flows: []
  scope: cdp_profile_api
- description: Data Cloud segmentation API.
  flows: []
  scope: cdp_segment_api
- description: Data Cloud identity resolution API.
  flows: []
  scope: cdp_identityresolution_api
- description: Data Cloud calculated insights API.
  flows: []
  scope: cdp_calculated_insight_api
- description: Data Cloud user claims.
  flows: []
  scope: data_cloud_user_claims
- description: Einstein GPT / generative AI API.
  flows: []
  scope: einstein_gpt_api
- description: Salesforce AI platform API.
  flows: []
  scope: sfap_api
- description: Model Context Protocol API scope.
  flows: []
  scope: mcp_api
- description: Einstein Bots / chatbot API.
  flows: []
  scope: chatbot_api
- description: CRM Analytics (Wave) API.
  flows: []
  scope: wave_api
- description: CRM Analytics Eclair charting API.
  flows: []
  scope: eclair_api
- description: Account Engagement (Pardot) API.
  flows: []
  scope: pardot_api
- description: Service Cloud real-time (SCRT) API.
  flows: []
  scope: scrt_api
slug: genentech-scopes
source_filename: genentech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.gene.com/.well-known/openid-configuration\ndocs: https://developer.gene.com/s/api-library\nnotes: >-\n  Scopes are taken verbatim from the `scopes_supported` array advertised by the\n  Genentech Developer Portal OpenID Connect discovery document. The portal runs\n  on Salesforce Experience Cloud, so these are the platform's standard OAuth2\n  scopes exposed by the identity provider, not per-resource FHIR UAPI business\n  scopes (the UAPI itself is gated by registration + per-organization API keys\n  through the Integration Marketplace). Captured for auth-clarity signal.\nschemes:\n- name: oauth2\n  source: well-known/genentech-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.gene.com/services/oauth2/authorize\n    tokenUrl: https://developer.gene.com/services/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication.\n- scope:\
  \ profile\n  description: Access to the user's basic profile claims.\n- scope: email\n  description: Access to the user's email address.\n- scope: address\n  description: Access to the user's address claim.\n- scope: phone\n  description: Access to the user's phone number claim.\n- scope: api\n  description: Access to platform REST/SOAP API resources.\n- scope: web\n  description: Web access to the org on behalf of the user.\n- scope: full\n  description: Full access to all resources the user can access.\n- scope: id\n  description: Access to the identity URL service.\n- scope: refresh_token\n  description: Issue a refresh token for long-lived access.\n- scope: offline_access\n  description: Maintain access when the user is offline.\n- scope: lightning\n  description: Access to Lightning Experience resources.\n- scope: visualforce\n  description: Access to Visualforce pages.\n- scope: content\n  description: Access to content/file resources.\n- scope: chatter_api\n  description: Access\
  \ to Chatter REST API resources.\n- scope: user_registration_api\n  description: Self-registration handler API.\n- scope: pwdless_login_api\n  description: Passwordless login API.\n- scope: forgot_password\n  description: Forgot-password flow.\n- scope: custom_permissions\n  description: Access to the user's custom permissions.\n- scope: interaction_api\n  description: Interaction Studio / interaction API.\n- scope: cdp_api\n  description: Data Cloud (CDP) API.\n- scope: cdp_ingest_api\n  description: Data Cloud ingestion API.\n- scope: cdp_query_api\n  description: Data Cloud query API.\n- scope: cdp_profile_api\n  description: Data Cloud profile API.\n- scope: cdp_segment_api\n  description: Data Cloud segmentation API.\n- scope: cdp_identityresolution_api\n  description: Data Cloud identity resolution API.\n- scope: cdp_calculated_insight_api\n  description: Data Cloud calculated insights API.\n- scope: data_cloud_user_claims\n  description: Data Cloud user claims.\n- scope: einstein_gpt_api\n\
  \  description: Einstein GPT / generative AI API.\n- scope: sfap_api\n  description: Salesforce AI platform API.\n- scope: mcp_api\n  description: Model Context Protocol API scope.\n- scope: chatbot_api\n  description: Einstein Bots / chatbot API.\n- scope: wave_api\n  description: CRM Analytics (Wave) API.\n- scope: eclair_api\n  description: CRM Analytics Eclair charting API.\n- scope: pardot_api\n  description: Account Engagement (Pardot) API.\n- scope: scrt_api\n  description: Service Cloud real-time (SCRT) API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genentech/refs/heads/main/scopes/genentech-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Healthcare
- Life Sciences
- FHIR
- Patient Support Services
- Drug Discovery
- Genomics
token_urls:
- https://developer.gene.com/services/oauth2/token
---
