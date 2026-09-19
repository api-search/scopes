---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Pearson Scopes
name_suffix: OAuth Scopes
note: 'Read verbatim from the scopes_supported array of the OpenID Connect discovery document Pearson serves at developer.pearson.com. IMPORTANT READING: this is the stock Salesforce Experience Cloud platform scope vocabulary exposed by the identity provider that gates the Pearson Developers Network portal. It is NOT a Pearson-authored scope surface for a Pearson API product, and no scope here grants access to a Pearson learning, assessment or certification API. Pearson publishes no public scopes or permissions reference — every documentation path under developer.pearson.com answers 401.'
overview: 'Pearson uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pearson
provider_slug: pearson
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: pearson-scopes
source_filename: pearson-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://developer.pearson.com/.well-known/openid-configuration\nnote: 'Read verbatim from the scopes_supported array of the OpenID Connect discovery document Pearson\n  serves at developer.pearson.com. IMPORTANT READING: this is the stock Salesforce Experience Cloud\n  platform scope vocabulary exposed by the identity provider that gates the Pearson Developers Network\n  portal. It is NOT a Pearson-authored scope surface for a Pearson API product, and no scope here\n  grants access to a Pearson learning, assessment or certification API. Pearson publishes no public\n  scopes or permissions reference — every documentation path under developer.pearson.com answers\n  401.'\nissuer: https://developer.pearson.com\nauthorization_endpoint: https://developer.pearson.com/services/oauth2/authorize\ntoken_endpoint: https://developer.pearson.com/services/oauth2/token\ndocs: null\ndocs_note: No anonymously reachable scopes/permissions reference\
  \ page exists; developer.pearson.com/*\n  returns 401.\nscope_vocabulary: salesforce-experience-cloud-platform\nscope_count: 36\nscopes:\n- name: address\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: cdp_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: cdp_calculated_insight_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: cdp_identityresolution_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: cdp_ingest_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: cdp_profile_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: cdp_query_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: cdp_segment_api\n  source: openid-configuration scopes_supported\n\
  \  pearson_authored: false\n- name: chatbot_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: chatter_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: content\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: custom_permissions\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: data_cloud_user_claims\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: eclair_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: einstein_gpt_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: email\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: forgot_password\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: full\n  source: openid-configuration scopes_supported\n  pearson_authored:\
  \ false\n- name: id\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: interaction_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: lightning\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: mcp_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: offline_access\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: openid\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: pardot_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: phone\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: profile\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: pwdless_login_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: refresh_token\n  source: openid-configuration\
  \ scopes_supported\n  pearson_authored: false\n- name: scrt_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: sfap_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: user_registration_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: visualforce\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: wave_api\n  source: openid-configuration scopes_supported\n  pearson_authored: false\n- name: web\n  source: openid-configuration scopes_supported\n  pearson_authored: false\nstandard_oidc_scopes:\n- openid\n- profile\n- email\n- address\n- phone\n- offline_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pearson/refs/heads/main/scopes/pearson-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Learning
- Assessment
- Certification
- Publishing
- EdTech
- Qualifications
- Testing
- Learning Management
- Workforce Skills
token_urls: []
---
