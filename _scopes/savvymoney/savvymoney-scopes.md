---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Savvymoney Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SavvyMoney uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SavvyMoney
provider_slug: savvymoney
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: savvymoney-scopes
source_filename: savvymoney-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://hub.savvymoney.com/.well-known/openid-configuration\nscope_note: 'SCOPE OF THIS FILE: these scopes govern sign-in to the SavvyMoney Partner Hub (hub.savvymoney.com),\n  NOT the credit/SSO REST API on creditscore.savvymoney.com. The Partner Hub runs on Salesforce Experience\n  Cloud and the advertised scopes are Salesforce platform scopes (pardot_api, cdp_*, visualforce, lightning,\n  wave_api, einstein_gpt_api), served under SavvyMoney''s own issuer. They are recorded verbatim because\n  they are what SavvyMoney''s host actually advertises, but a partner integrating the credit API will\n  never request any of them - that API uses a proprietary authId/authKey JWT exchange with no scope parameter\n  at all.'\nissuer: https://hub.savvymoney.com\nauthorization_endpoint: https://hub.savvymoney.com/services/oauth2/authorize\ntoken_endpoint: https://hub.savvymoney.com/services/oauth2/token\nscope_count: 36\nscopes:\n- name:\
  \ address\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: cdp_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: cdp_calculated_insight_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: cdp_identityresolution_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: cdp_ingest_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: cdp_profile_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: cdp_query_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: cdp_segment_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name:\
  \ chatbot_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: chatter_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: content\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: custom_permissions\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: data_cloud_user_claims\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: eclair_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: einstein_gpt_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: email\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: forgot_password\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: full\n  description:\
  \ Advertised in scopes_supported; no per-scope description is published.\n- name: id\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: interaction_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: lightning\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: mcp_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: offline_access\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: openid\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: pardot_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: phone\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: profile\n  description: Advertised in scopes_supported; no per-scope description\
  \ is published.\n- name: pwdless_login_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: refresh_token\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: scrt_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: sfap_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: user_registration_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: visualforce\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: wave_api\n  description: Advertised in scopes_supported; no per-scope description is published.\n- name: web\n  description: Advertised in scopes_supported; no per-scope description is published.\ncredit_api_scopes:\n  present: false\n  note: The documented credit/SSO API has no scope model. Authorisation is bounded\
  \ instead by the API\n    user's Audience Domains and Partner ID List, configured by SavvyMoney at credential issuance rather\n    than requested per call.\n  source: authentication/savvymoney-authentication.yml\nevidence:\n- url: https://hub.savvymoney.com/.well-known/openid-configuration\n  status: 200\n- url: https://creditscore.savvymoney.com/.well-known/oauth-authorization-server\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savvymoney/refs/heads/main/scopes/savvymoney-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Financial-Services
- Credit Scores
- Credit Monitoring
- Financial Wellness
- Banking
- Credit Unions
- Fintech
- Single Sign-On
- Embedded Finance
- Lending
- Account Opening
token_urls: []
---
