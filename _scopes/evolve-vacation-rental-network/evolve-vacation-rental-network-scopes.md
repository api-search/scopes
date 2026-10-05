---
authorization_urls:
- https://help.evolve.com/services/oauth2/authorize
description: The scopes_supported list advertised by the OpenID Connect provider on help.evolve.com. Read verbatim from the live discovery document — nothing is derived from an OpenAPI, because Evolve publishes none.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Evolve Vacation Rental Network Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Evolve publishes 36 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Evolve API on a user''s behalf.


  Tokens are issued from https://help.evolve.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Evolve
provider_slug: evolve-vacation-rental-network
schemes: []
scope_count: 36
scope_names:
- openid
- profile
- email
- address
- phone
- id
- offline_access
- refresh_token
- api
- full
- web
- lightning
- visualforce
- content
- custom_permissions
- chatter_api
- wave_api
- eclair_api
- pardot_api
- interaction_api
- chatbot_api
- scrt_api
- sfap_api
- einstein_gpt_api
- mcp_api
- cdp_api
- cdp_query_api
- cdp_ingest_api
- cdp_profile_api
- cdp_segment_api
- cdp_calculated_insight_api
- cdp_identityresolution_api
- data_cloud_user_claims
- user_registration_api
- pwdless_login_api
- forgot_password
scopes:
- description: Return an OpenID Connect ID token.
  flows: []
  scope: openid
- description: Standard OIDC profile claims.
  flows: []
  scope: profile
- description: Email address and email_verified claim.
  flows: []
  scope: email
- description: Address claim.
  flows: []
  scope: address
- description: Phone number and phone_number_verified claim.
  flows: []
  scope: phone
- description: Salesforce identity URL access.
  flows: []
  scope: id
- description: Long-lived access without the user present.
  flows: []
  scope: offline_access
- description: Issue a refresh token.
  flows: []
  scope: refresh_token
- description: Salesforce REST/SOAP data API access.
  flows: []
  scope: api
- description: All permissions the user holds. Broad — the platform's widest grant.
  flows: []
  scope: full
- description: Web/session access via the access token.
  flows: []
  scope: web
- description: Lightning application access.
  flows: []
  scope: lightning
- description: Visualforce page access.
  flows: []
  scope: visualforce
- description: Salesforce Files/Content access.
  flows: []
  scope: content
- description: Return the connected app's custom permissions for the user.
  flows: []
  scope: custom_permissions
- description: Connect (Chatter) REST API access.
  flows: []
  scope: chatter_api
- description: CRM Analytics (Wave) REST API access.
  flows: []
  scope: wave_api
- description: CRM Analytics chart/Eclair API access.
  flows: []
  scope: eclair_api
- description: Account Engagement (Pardot) API access.
  flows: []
  scope: pardot_api
- description: Marketing Cloud interaction/journey API access.
  flows: []
  scope: interaction_api
- description: Einstein Bots API access.
  flows: []
  scope: chatbot_api
- description: Service Cloud real-time (Messaging for In-App and Web) API access.
  flows: []
  scope: scrt_api
- description: Salesforce AI platform (Models/Agent) API access.
  flows: []
  scope: sfap_api
- description: Einstein GPT / generative AI API access.
  flows: []
  scope: einstein_gpt_api
- description: Salesforce Model Context Protocol API access. Platform-advertised only — no MCP endpoint was reachable on any Evolve host during this pass.
  flows: []
  scope: mcp_api
- description: Data Cloud API access.
  flows: []
  scope: cdp_api
- description: Data Cloud query API.
  flows: []
  scope: cdp_query_api
- description: Data Cloud ingestion API.
  flows: []
  scope: cdp_ingest_api
- description: Data Cloud profile API.
  flows: []
  scope: cdp_profile_api
- description: Data Cloud segmentation API.
  flows: []
  scope: cdp_segment_api
- description: Data Cloud calculated insights API.
  flows: []
  scope: cdp_calculated_insight_api
- description: Data Cloud identity resolution API.
  flows: []
  scope: cdp_identityresolution_api
- description: Data Cloud user claims in the token.
  flows: []
  scope: data_cloud_user_claims
- description: Self-registration API for external identity users.
  flows: []
  scope: user_registration_api
- description: Passwordless login API.
  flows: []
  scope: pwdless_login_api
- description: Forgot-password flow API.
  flows: []
  scope: forgot_password
slug: evolve-vacation-rental-network-scopes
source_filename: evolve-vacation-rental-network-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://help.evolve.com/.well-known/openid-configuration\nname: Evolve — OAuth scopes\ndescription: >-\n  The scopes_supported list advertised by the OpenID Connect provider on\n  help.evolve.com. Read verbatim from the live discovery document — nothing is derived\n  from an OpenAPI, because Evolve publishes none.\nimportant_note: >-\n  READ THIS BEFORE USING THIS FILE. These are the Salesforce Experience Cloud standard\n  platform scopes, advertised by Evolve's own tenant at issuer https://help.evolve.com.\n  They are NOT a scope vocabulary Evolve authored for a product API, and the presence\n  of a scope here says only that the platform can mint it — not that Evolve exposes the\n  matching surface to third parties. Do not read cdp_*/einstein_gpt_api/mcp_api as\n  evidence that Evolve ships a Data Cloud, Einstein or MCP integration.\nissuer: https://help.evolve.com\nauthorization_endpoint: https://help.evolve.com/services/oauth2/authorize\n\
  token_endpoint: https://help.evolve.com/services/oauth2/token\nscope_count: 36\ndocs: null\ndocs_note: >-\n  Evolve publishes no scopes or permissions reference page. Searched evolve.com,\n  help.evolve.com and owner.evolve.com; nothing found.\nscopes:\n- name: openid\n  family: oidc\n  description: Return an OpenID Connect ID token.\n- name: profile\n  family: oidc\n  description: Standard OIDC profile claims.\n- name: email\n  family: oidc\n  description: Email address and email_verified claim.\n- name: address\n  family: oidc\n  description: Address claim.\n- name: phone\n  family: oidc\n  description: Phone number and phone_number_verified claim.\n- name: id\n  family: oidc\n  description: Salesforce identity URL access.\n- name: offline_access\n  family: oidc\n  description: Long-lived access without the user present.\n- name: refresh_token\n  family: oidc\n  description: Issue a refresh token.\n- name: api\n  family: platform\n  description: Salesforce REST/SOAP data API access.\n\
  - name: full\n  family: platform\n  description: All permissions the user holds. Broad — the platform's widest grant.\n- name: web\n  family: platform\n  description: Web/session access via the access token.\n- name: lightning\n  family: platform\n  description: Lightning application access.\n- name: visualforce\n  family: platform\n  description: Visualforce page access.\n- name: content\n  family: platform\n  description: Salesforce Files/Content access.\n- name: custom_permissions\n  family: platform\n  description: Return the connected app's custom permissions for the user.\n- name: chatter_api\n  family: platform\n  description: Connect (Chatter) REST API access.\n- name: wave_api\n  family: analytics\n  description: CRM Analytics (Wave) REST API access.\n- name: eclair_api\n  family: analytics\n  description: CRM Analytics chart/Eclair API access.\n- name: pardot_api\n  family: marketing\n  description: Account Engagement (Pardot) API access.\n- name: interaction_api\n  family: marketing\n\
  \  description: Marketing Cloud interaction/journey API access.\n- name: chatbot_api\n  family: service\n  description: Einstein Bots API access.\n- name: scrt_api\n  family: service\n  description: Service Cloud real-time (Messaging for In-App and Web) API access.\n- name: sfap_api\n  family: ai\n  description: Salesforce AI platform (Models/Agent) API access.\n- name: einstein_gpt_api\n  family: ai\n  description: Einstein GPT / generative AI API access.\n- name: mcp_api\n  family: ai\n  description: >-\n    Salesforce Model Context Protocol API access. Platform-advertised only — no MCP\n    endpoint was reachable on any Evolve host during this pass.\n- name: cdp_api\n  family: data-cloud\n  description: Data Cloud API access.\n- name: cdp_query_api\n  family: data-cloud\n  description: Data Cloud query API.\n- name: cdp_ingest_api\n  family: data-cloud\n  description: Data Cloud ingestion API.\n- name: cdp_profile_api\n  family: data-cloud\n  description: Data Cloud profile API.\n-\
  \ name: cdp_segment_api\n  family: data-cloud\n  description: Data Cloud segmentation API.\n- name: cdp_calculated_insight_api\n  family: data-cloud\n  description: Data Cloud calculated insights API.\n- name: cdp_identityresolution_api\n  family: data-cloud\n  description: Data Cloud identity resolution API.\n- name: data_cloud_user_claims\n  family: data-cloud\n  description: Data Cloud user claims in the token.\n- name: user_registration_api\n  family: identity\n  description: Self-registration API for external identity users.\n- name: pwdless_login_api\n  family: identity\n  description: Passwordless login API.\n- name: forgot_password\n  family: identity\n  description: Forgot-password flow API.\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://help.evolve.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json;charset=UTF-8\nchecked: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolve-vacation-rental-network/refs/heads/main/scopes/evolve-vacation-rental-network-scopes.yml
summary_line: 36 scopes
tags:
- Company
- Travel
- Hospitality
- Vacation Rentals
- Short-Term Rental
- Property Management
- Real Estate
- Booking
token_bound: false
token_urls:
- https://help.evolve.com/services/oauth2/token
---
