---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Animal And Plant Health Inspection Service Scopes
name_suffix: OAuth Scopes
note: 'These 36 scopes are read verbatim from the scopes_supported array of the OpenID Connect Discovery documents APHIS serves on its three Salesforce Experience Cloud hosts. They are the Salesforce platform default scope set, not a permission model APHIS authored or documents: APHIS publishes no scope reference page, and no APHIS document maps any of these scopes to an APHIS operation. Recorded because the surface is genuinely served by APHIS-controlled issuers; descriptions below state what each platform scope grants and are derived from the OAuth/OIDC and Salesforce platform meanings, not from APHIS documentation.'
overview: 'Animal and Plant Health Inspection Service publishes 36 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Animal and Plant Health Inspection Service API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Animal and Plant Health Inspection Service
provider_slug: animal-and-plant-health-inspection-service
schemes: []
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
- description: Standard OIDC address claim.
  flows: []
  scope: address
- description: Access the Salesforce REST/SOAP data APIs of the org as the signed-in user.
  flows: []
  scope: api
- description: Data Cloud (CDP) API.
  flows: []
  scope: cdp_api
- description: Data Cloud calculated insights API.
  flows: []
  scope: cdp_calculated_insight_api
- description: Data Cloud identity resolution API.
  flows: []
  scope: cdp_identityresolution_api
- description: Data Cloud ingestion API.
  flows: []
  scope: cdp_ingest_api
- description: Data Cloud profile API.
  flows: []
  scope: cdp_profile_api
- description: Data Cloud query API.
  flows: []
  scope: cdp_query_api
- description: Data Cloud segmentation API.
  flows: []
  scope: cdp_segment_api
- description: Einstein Bots API.
  flows: []
  scope: chatbot_api
- description: Access the Connect (Chatter) REST API.
  flows: []
  scope: chatter_api
- description: Access Salesforce Files / ContentDocument.
  flows: []
  scope: content
- description: Return the org custom permissions granted to the user.
  flows: []
  scope: custom_permissions
- description: Data Cloud user claims in the id_token.
  flows: []
  scope: data_cloud_user_claims
- description: CRM Analytics chart/visualization API.
  flows: []
  scope: eclair_api
- description: Einstein GPT API.
  flows: []
  scope: einstein_gpt_api
- description: Standard OIDC email + email_verified claims.
  flows: []
  scope: email
- description: Password-reset API for Experience Cloud users.
  flows: []
  scope: forgot_password
- description: Full access to all data the signed-in user can reach (excludes refresh token).
  flows: []
  scope: full
- description: Salesforce identity URL access.
  flows: []
  scope: id
- description: Interaction/Flow runtime API.
  flows: []
  scope: interaction_api
- description: Access Lightning Experience pages.
  flows: []
  scope: lightning
- description: Salesforce Model Context Protocol API scope (platform capability; no APHIS MCP server is published).
  flows: []
  scope: mcp_api
- description: Issue a refresh token so the client can act after the access token expires.
  flows: []
  scope: offline_access
- description: OpenID Connect - return an id_token identifying the signed-in user.
  flows: []
  scope: openid
- description: Account Engagement (Pardot) API.
  flows: []
  scope: pardot_api
- description: Standard OIDC phone_number + phone_number_verified claims.
  flows: []
  scope: phone
- description: Standard OIDC profile claims (name, preferred_username, picture, locale).
  flows: []
  scope: profile
- description: Passwordless login API.
  flows: []
  scope: pwdless_login_api
- description: Legacy Salesforce alias for offline_access.
  flows: []
  scope: refresh_token
- description: Service Cloud Real-Time (Messaging) API.
  flows: []
  scope: scrt_api
- description: Salesforce AI platform (models) API.
  flows: []
  scope: sfap_api
- description: Self-registration API for Experience Cloud users.
  flows: []
  scope: user_registration_api
- description: Access Visualforce pages.
  flows: []
  scope: visualforce
- description: CRM Analytics (Wave) REST API.
  flows: []
  scope: wave_api
- description: Open a web session in the org using the access token.
  flows: []
  scope: web
slug: animal-and-plant-health-inspection-service-scopes
source_filename: animal-and-plant-health-inspection-service-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://efile.aphis.usda.gov/.well-known/openid-configuration (HTTP 200), identical scopes_supported\n  on acir.aphis.usda.gov and aphis.my.site.com\nspecification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Animal and Plant Health Inspection Service\nproviderId: animal-and-plant-health-inspection-service\ndocs: null\nnote: 'These 36 scopes are read verbatim from the scopes_supported array of the OpenID Connect Discovery\n  documents APHIS serves on its three Salesforce Experience Cloud hosts. They are the Salesforce platform\n  default scope set, not a permission model APHIS authored or documents: APHIS publishes no scope reference\n  page, and no APHIS document maps any of these scopes to an APHIS operation. Recorded because the surface\n  is genuinely served by APHIS-controlled issuers; descriptions below state what each platform scope grants\n  and are derived from the OAuth/OIDC and Salesforce platform\
  \ meanings, not from APHIS documentation.'\nissuers:\n- https://efile.aphis.usda.gov\n- https://acir.aphis.usda.gov\n- https://aphis.my.site.com\nscope_count: 36\nauthored_by_provider: false\nscopes:\n- name: address\n  description: Standard OIDC address claim.\n  source: scopes_supported\n- name: api\n  description: Access the Salesforce REST/SOAP data APIs of the org as the signed-in user.\n  source: scopes_supported\n- name: cdp_api\n  description: Data Cloud (CDP) API.\n  source: scopes_supported\n- name: cdp_calculated_insight_api\n  description: Data Cloud calculated insights API.\n  source: scopes_supported\n- name: cdp_identityresolution_api\n  description: Data Cloud identity resolution API.\n  source: scopes_supported\n- name: cdp_ingest_api\n  description: Data Cloud ingestion API.\n  source: scopes_supported\n- name: cdp_profile_api\n  description: Data Cloud profile API.\n  source: scopes_supported\n- name: cdp_query_api\n  description: Data Cloud query API.\n  source: scopes_supported\n\
  - name: cdp_segment_api\n  description: Data Cloud segmentation API.\n  source: scopes_supported\n- name: chatbot_api\n  description: Einstein Bots API.\n  source: scopes_supported\n- name: chatter_api\n  description: Access the Connect (Chatter) REST API.\n  source: scopes_supported\n- name: content\n  description: Access Salesforce Files / ContentDocument.\n  source: scopes_supported\n- name: custom_permissions\n  description: Return the org custom permissions granted to the user.\n  source: scopes_supported\n- name: data_cloud_user_claims\n  description: Data Cloud user claims in the id_token.\n  source: scopes_supported\n- name: eclair_api\n  description: CRM Analytics chart/visualization API.\n  source: scopes_supported\n- name: einstein_gpt_api\n  description: Einstein GPT API.\n  source: scopes_supported\n- name: email\n  description: Standard OIDC email + email_verified claims.\n  source: scopes_supported\n- name: forgot_password\n  description: Password-reset API for Experience\
  \ Cloud users.\n  source: scopes_supported\n- name: full\n  description: Full access to all data the signed-in user can reach (excludes refresh token).\n  source: scopes_supported\n- name: id\n  description: Salesforce identity URL access.\n  source: scopes_supported\n- name: interaction_api\n  description: Interaction/Flow runtime API.\n  source: scopes_supported\n- name: lightning\n  description: Access Lightning Experience pages.\n  source: scopes_supported\n- name: mcp_api\n  description: Salesforce Model Context Protocol API scope (platform capability; no APHIS MCP server is\n    published).\n  source: scopes_supported\n- name: offline_access\n  description: Issue a refresh token so the client can act after the access token expires.\n  source: scopes_supported\n- name: openid\n  description: OpenID Connect - return an id_token identifying the signed-in user.\n  source: scopes_supported\n- name: pardot_api\n  description: Account Engagement (Pardot) API.\n  source: scopes_supported\n\
  - name: phone\n  description: Standard OIDC phone_number + phone_number_verified claims.\n  source: scopes_supported\n- name: profile\n  description: Standard OIDC profile claims (name, preferred_username, picture, locale).\n  source: scopes_supported\n- name: pwdless_login_api\n  description: Passwordless login API.\n  source: scopes_supported\n- name: refresh_token\n  description: Legacy Salesforce alias for offline_access.\n  source: scopes_supported\n- name: scrt_api\n  description: Service Cloud Real-Time (Messaging) API.\n  source: scopes_supported\n- name: sfap_api\n  description: Salesforce AI platform (models) API.\n  source: scopes_supported\n- name: user_registration_api\n  description: Self-registration API for Experience Cloud users.\n  source: scopes_supported\n- name: visualforce\n  description: Access Visualforce pages.\n  source: scopes_supported\n- name: wave_api\n  description: CRM Analytics (Wave) REST API.\n  source: scopes_supported\n- name: web\n  description: Open\
  \ a web session in the org using the access token.\n  source: scopes_supported\nmaintainers:\n- FN: Kin Lane\n  email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/animal-and-plant-health-inspection-service/refs/heads/main/scopes/animal-and-plant-health-inspection-service-scopes.yml
summary_line: 36 scopes
tags:
- Agriculture
- Animal Health
- Animal Welfare
- Biotechnology
- Federal Government
- Import Export
- Permits
- Pest Control
- Plant Health
- Regulatory
- USDA
- Wildlife
token_bound: false
token_urls: []
---
