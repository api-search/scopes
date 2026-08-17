---
api_specs:
- filename: pardot-objects-api-openapi.yml
  format: yaml
  label: Salesforce Marketing Cloud Account Engagement (Pardot) Objects API
  slug: pardot-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pardot/refs/heads/main/openapi/pardot-objects-api-openapi.yml
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: https://help.salesforce.com/s/articleView?id=sf.remoteaccess_oauth_tokens_scopes.htm&type=5
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Pardot Scopes
name_suffix: OAuth Scopes
note: 'Account Engagement exposes exactly ONE product scope: pardot_api. It is not a granular permission model — the scope grants access to the API, and what a caller may actually do is decided by the Account Engagement user role abilities on the authenticating user (each object reference page names the ability required per operation, e.g. "Prospect > Prospects > Create"). The scope list below is the live scopes_supported array from the Salesforce authorization server, which is the authoritative source; the entries after pardot_api are Salesforce-platform scopes commonly paired with it, not Account Engagement scopes.'
overview: 'Salesforce Marketing Cloud Account Engagement (Pardot) publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Marketing Cloud Account Engagement (Pardot) API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Marketing Cloud Account Engagement (Pardot)
provider_slug: pardot
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: BearerAuth
scope_count: 1
scope_names:
- pardot_api
scopes:
- description: Access the Marketing Cloud Account Engagement (Pardot) API. Required on the connected app or no OAuth flow other than username/password can be used with the Account Engagement API.
  flows:
  - authorizationCode
  scope: pardot_api
slug: pardot-scopes
source_filename: pardot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.salesforce.com/docs/marketing/pardot/guide/authentication.md\ndocs: https://help.salesforce.com/s/articleView?id=sf.remoteaccess_oauth_tokens_scopes.htm&type=5\nnote: 'Account Engagement exposes exactly ONE product scope: pardot_api. It is not a granular permission model\n  — the scope grants access to the API, and what a caller may actually do is decided by the Account Engagement\n  user role abilities on the authenticating user (each object reference page names the ability required per\n  operation, e.g. \"Prospect > Prospects > Create\"). The scope list below is the live scopes_supported array\n  from the Salesforce authorization server, which is the authoritative source; the entries after pardot_api\n  are Salesforce-platform scopes commonly paired with it, not Account Engagement scopes.'\nauthorization_server: https://login.salesforce.com\ndiscovery: https://login.salesforce.com/.well-known/openid-configuration\n\
  schemes:\n- name: BearerAuth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\nscope_count: 1\nscopes:\n- scope: pardot_api\n  description: Access the Marketing Cloud Account Engagement (Pardot) API. Required on the connected app or\n    no OAuth flow other than username/password can be used with the Account Engagement API.\n  flows:\n  - authorizationCode\n  product: Account Engagement\n  sources:\n  - https://developer.salesforce.com/docs/marketing/pardot/guide/authentication.md\n  - https://login.salesforce.com/.well-known/openid-configuration\ncompanion_platform_scopes:\n- scope: refresh_token\n  description: Issue a refresh token so the integration can renew access without re-consent.\n- scope: offline_access\n  description: Equivalent to refresh_token; keeps the grant alive between sessions.\n- scope: api\n  description: Salesforce Platform API access\
  \ — needed when the same connected app also calls Salesforce REST/SOAP\n    objects for Account Engagement development.\n- scope: openid\n  description: OpenID Connect sign-in; returns an id_token.\nauthorization_model:\n  style: coarse scope + per-object role abilities\n  note: Object reference pages publish the required ability per operation (for example Prospect Create requires\n    \"Prospect > Prospects > Create\", and reading prospects not assigned to the API user requires \"Prospects\n    > Prospects > View prospects not assigned to self\").\n  source: https://developer.salesforce.com/docs/marketing/pardot/guide/prospect-v5.md\nall_authorization_server_scopes:\n- address\n- api\n- cdp_api\n- cdp_calculated_insight_api\n- cdp_identityresolution_api\n- cdp_ingest_api\n- cdp_profile_api\n- cdp_query_api\n- cdp_segment_api\n- chatbot_api\n- chatter_api\n- content\n- custom_permissions\n- data_cloud_user_claims\n- eclair_api\n- einstein_gpt_api\n- email\n- forgot_password\n- full\n-\
  \ id\n- interaction_api\n- lightning\n- mcp_api\n- offline_access\n- openid\n- pardot_api\n- phone\n- profile\n- pwdless_login_api\n- refresh_token\n- scrt_api\n- sfap_api\n- user_registration_api\n- visualforce\n- wave_api\n- web\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pardot/refs/heads/main/scopes/pardot-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Marketing Automation
- B2B Marketing
- Lead Generation
- Email Marketing
- Salesforce
- Account Engagement
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
