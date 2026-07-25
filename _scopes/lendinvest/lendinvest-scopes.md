---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Lendinvest Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LendInvest uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LendInvest
provider_slug: lendinvest
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: lendinvest-scopes
source_filename: lendinvest-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://customerportal.lendinvest.com/.well-known/openid-configuration\nissuer: https://customerportal.lendinvest.com\nnotes: >-\n  Captured verbatim from the scopes_supported array of the OpenID Connect discovery\n  document served by the LendInvest broker / borrower portal. IMPORTANT PROVENANCE CAVEAT:\n  that portal is a Salesforce Experience Cloud community, so this is the standard Salesforce\n  platform scope set advertised by the tenant, not a LendInvest-authored product scope\n  vocabulary. LendInvest publishes no public API and no scopes/permissions reference page\n  of its own. Only the OIDC core scopes and the general-purpose Salesforce API scopes are\n  likely to be grantable to a partner connected app; the Data Cloud (cdp_*), Marketing\n  (pardot_api) and Einstein (einstein_gpt_api, sfap_api) scopes are advertised by the\n  platform whether or not the tenant licenses those products.\nscope_source: salesforce-platform-advertised\n\
  oidc_core_scopes:\n- name: openid\n  description: Request an OpenID Connect ID token for the authenticated portal user.\n- name: profile\n  description: Access the user's basic profile claims (name, username, picture, locale).\n- name: email\n  description: Access the user's email address and email_verified claim.\n- name: phone\n  description: Access the user's phone number and phone_number_verified claim.\n- name: address\n  description: Access the user's address claim.\n- name: id\n  description: Salesforce identity URL scope; returns the identity service endpoint for the user.\n- name: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without user interaction.\n- name: refresh_token\n  description: Salesforce alias for offline_access; permits refresh-token issuance.\nplatform_api_scopes:\n- name: api\n  description: Access Salesforce data via the tenant's REST and SOAP APIs on behalf of the user.\n- name: full\n  description: Full access\
  \ to all data the authenticated user can reach; does not by itself grant refresh tokens.\n- name: web\n  description: Permit use of the access token in a web browser session (frontdoor).\n- name: lightning\n  description: Access Lightning Experience application resources.\n- name: visualforce\n  description: Access Visualforce pages.\n- name: content\n  description: Access Salesforce Files / content resources.\n- name: chatter_api\n  description: Access the Chatter / Connect REST API.\n- name: custom_permissions\n  description: Return the tenant's custom permissions for the authenticated user in the token response.\n- name: user_registration_api\n  description: Access the self-registration API used for portal / community account creation.\n- name: pwdless_login_api\n  description: Access the passwordless login API for portal users.\n- name: forgot_password\n  description: Access the forgot-password / credential-reset API for portal users.\n- name: wave_api\n  description: Access CRM Analytics\
  \ (Wave) APIs.\n- name: eclair_api\n  description: Access CRM Analytics chart / Eclair APIs.\n- name: interaction_api\n  description: Access the interaction (flow orchestration) API.\n- name: chatbot_api\n  description: Access the Einstein Bots runtime API.\n- name: scrt_api\n  description: Access the Service Cloud real-time messaging API.\n- name: mcp_api\n  description: Access the Salesforce Model Context Protocol API surface advertised by the platform.\ndata_cloud_and_ai_scopes:\n- name: cdp_api\n  description: Access Salesforce Data Cloud (CDP) APIs.\n- name: cdp_ingest_api\n  description: Ingest records into Data Cloud.\n- name: cdp_query_api\n  description: Query Data Cloud data.\n- name: cdp_profile_api\n  description: Read unified Data Cloud customer profiles.\n- name: cdp_segment_api\n  description: Manage Data Cloud segments.\n- name: cdp_identityresolution_api\n  description: Access Data Cloud identity-resolution rulesets.\n- name: cdp_calculated_insight_api\n  description:\
  \ Access Data Cloud calculated insights.\n- name: data_cloud_user_claims\n  description: Include Data Cloud user claims in the token.\n- name: einstein_gpt_api\n  description: Access Einstein generative AI APIs.\n- name: sfap_api\n  description: Access the Salesforce AI platform API.\n- name: pardot_api\n  description: Access Account Engagement (Pardot) marketing automation APIs.\nrelated:\n  authentication: authentication/lendinvest-authentication.yml\n  well_known: well-known/lendinvest-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendinvest/refs/heads/main/scopes/lendinvest-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Fintech
- Lending
- Mortgages
- Property Finance
- Real Estate
- Financial Services
- United Kingdom
token_urls: []
---
