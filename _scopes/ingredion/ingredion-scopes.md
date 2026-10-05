---
authorization_urls:
- https://myingredion.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorization_code
kind: oauth-scopes
layout: scope
method: probed
name: Ingredion Scopes
name_suffix: OAuth Scopes
note: Read verbatim from scopes_supported in the OpenID Connect discovery document Ingredion serves on its MyIngredion customer portal. Ingredion publishes no OpenAPI and no scope reference page, so there is nothing to derive from and nothing to cross-check against. These are the SALESFORCE PLATFORM scope names advertised by Ingredion's Experience Cloud org (00D30000000MNMR) — they are not an Ingredion-authored permission model, and the descriptions below are the standard Salesforce meanings, not Ingredion copy. grant_types_supported offers only authorization_code and refresh_token, so every scope here requires an interactive customer sign-in.
overview: 'Ingredion publishes 36 OAuth 2.0 scopes via the authorization_code flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ingredion API on a user''s behalf.


  Tokens are issued from https://myingredion.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ingredion
provider_slug: ingredion
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
- description: Address claim.
  flows: []
  scope: address
- description: Access the Salesforce REST/SOAP data API as the signed-in user.
  flows: []
  scope: api
- description: Data Cloud (CDP) API access.
  flows: []
  scope: cdp_api
- description: Data Cloud calculated insights API access.
  flows: []
  scope: cdp_calculated_insight_api
- description: Data Cloud identity resolution API access.
  flows: []
  scope: cdp_identityresolution_api
- description: Data Cloud ingestion API access.
  flows: []
  scope: cdp_ingest_api
- description: Data Cloud profile API access.
  flows: []
  scope: cdp_profile_api
- description: Data Cloud query API access.
  flows: []
  scope: cdp_query_api
- description: Data Cloud segmentation API access.
  flows: []
  scope: cdp_segment_api
- description: Einstein Bots API access.
  flows: []
  scope: chatbot_api
- description: Connect REST (Chatter) API access.
  flows: []
  scope: chatter_api
- description: Salesforce CMS / content access.
  flows: []
  scope: content
- description: Return the custom permissions granted to the user.
  flows: []
  scope: custom_permissions
- description: Data Cloud user claims.
  flows: []
  scope: data_cloud_user_claims
- description: Einstein Analytics chart (Eclair) API access.
  flows: []
  scope: eclair_api
- description: Einstein GPT API access.
  flows: []
  scope: einstein_gpt_api
- description: Email address and email_verified claim.
  flows: []
  scope: email
- description: Password reset API access.
  flows: []
  scope: forgot_password
- description: Full access to all data the signed-in user can reach.
  flows: []
  scope: full
- description: Identity URL access.
  flows: []
  scope: id
- description: Marketing Cloud interaction API access.
  flows: []
  scope: interaction_api
- description: Lightning Experience application access.
  flows: []
  scope: lightning
- description: Salesforce-declared MCP API scope (platform capability; no Ingredion MCP endpoint is published).
  flows: []
  scope: mcp_api
- description: Issue a refresh token.
  flows: []
  scope: offline_access
- description: Issue an ID token (OpenID Connect core scope).
  flows: []
  scope: openid
- description: Account Engagement (Pardot) API access.
  flows: []
  scope: pardot_api
- description: phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Basic profile claims (name, nickname, picture, zoneinfo, locale, updated_at).
  flows: []
  scope: profile
- description: Passwordless login API access.
  flows: []
  scope: pwdless_login_api
- description: Issue a refresh token (Salesforce alias of offline_access).
  flows: []
  scope: refresh_token
- description: Service Cloud real-time (Messaging) API access.
  flows: []
  scope: scrt_api
- description: Salesforce agent/AI platform API access.
  flows: []
  scope: sfap_api
- description: Self-registration API access.
  flows: []
  scope: user_registration_api
- description: Visualforce page access.
  flows: []
  scope: visualforce
- description: CRM Analytics (Wave) API access.
  flows: []
  scope: wave_api
- description: Open a web session on the user behalf.
  flows: []
  scope: web
slug: ingredion-scopes
source_filename: ingredion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://myingredion.com/.well-known/openid-configuration\nnote: Read verbatim from scopes_supported in the OpenID Connect discovery document Ingredion serves on\n  its MyIngredion customer portal. Ingredion publishes no OpenAPI and no scope reference page, so there\n  is nothing to derive from and nothing to cross-check against. These are the SALESFORCE PLATFORM scope\n  names advertised by Ingredion's Experience Cloud org (00D30000000MNMR) — they are not an Ingredion-authored\n  permission model, and the descriptions below are the standard Salesforce meanings, not Ingredion copy.\n  grant_types_supported offers only authorization_code and refresh_token, so every scope here requires\n  an interactive customer sign-in.\nflow: authorization_code\nauthorization_endpoint: https://myingredion.com/services/oauth2/authorize\ntoken_endpoint: https://myingredion.com/services/oauth2/token\ndocs: null\ndocs_note: No public scope or permissions\
  \ reference is published by Ingredion.\nscope_count: 36\nscopes:\n- name: address\n  description: Address claim.\n- name: api\n  description: Access the Salesforce REST/SOAP data API as the signed-in user.\n- name: cdp_api\n  description: Data Cloud (CDP) API access.\n- name: cdp_calculated_insight_api\n  description: Data Cloud calculated insights API access.\n- name: cdp_identityresolution_api\n  description: Data Cloud identity resolution API access.\n- name: cdp_ingest_api\n  description: Data Cloud ingestion API access.\n- name: cdp_profile_api\n  description: Data Cloud profile API access.\n- name: cdp_query_api\n  description: Data Cloud query API access.\n- name: cdp_segment_api\n  description: Data Cloud segmentation API access.\n- name: chatbot_api\n  description: Einstein Bots API access.\n- name: chatter_api\n  description: Connect REST (Chatter) API access.\n- name: content\n  description: Salesforce CMS / content access.\n- name: custom_permissions\n  description: Return\
  \ the custom permissions granted to the user.\n- name: data_cloud_user_claims\n  description: Data Cloud user claims.\n- name: eclair_api\n  description: Einstein Analytics chart (Eclair) API access.\n- name: einstein_gpt_api\n  description: Einstein GPT API access.\n- name: email\n  description: Email address and email_verified claim.\n- name: forgot_password\n  description: Password reset API access.\n- name: full\n  description: Full access to all data the signed-in user can reach.\n- name: id\n  description: Identity URL access.\n- name: interaction_api\n  description: Marketing Cloud interaction API access.\n- name: lightning\n  description: Lightning Experience application access.\n- name: mcp_api\n  description: Salesforce-declared MCP API scope (platform capability; no Ingredion MCP endpoint is published).\n- name: offline_access\n  description: Issue a refresh token.\n- name: openid\n  description: Issue an ID token (OpenID Connect core scope).\n- name: pardot_api\n  description:\
  \ Account Engagement (Pardot) API access.\n- name: phone\n  description: phone_number and phone_number_verified claims.\n- name: profile\n  description: Basic profile claims (name, nickname, picture, zoneinfo, locale, updated_at).\n- name: pwdless_login_api\n  description: Passwordless login API access.\n- name: refresh_token\n  description: Issue a refresh token (Salesforce alias of offline_access).\n- name: scrt_api\n  description: Service Cloud real-time (Messaging) API access.\n- name: sfap_api\n  description: Salesforce agent/AI platform API access.\n- name: user_registration_api\n  description: Self-registration API access.\n- name: visualforce\n  description: Visualforce page access.\n- name: wave_api\n  description: CRM Analytics (Wave) API access.\n- name: web\n  description: Open a web session on the user behalf.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingredion/refs/heads/main/scopes/ingredion-scopes.yml
summary_line: 36 scopes · authorization_code
tags:
- Fortune 500
- Food and Beverage
- Ingredients
- Food Manufacturing
- Agriculture
- Plant-Based Proteins
- Specialty Chemicals
- Consumer Packaged Goods
token_bound: false
token_urls:
- https://myingredion.com/services/oauth2/token
---
