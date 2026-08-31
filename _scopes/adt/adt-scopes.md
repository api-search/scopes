---
api_specs:
- filename: adt-access-codes-api-openapi.yml
  format: yaml
  label: ADT Access Codes API
  slug: adt-access-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-access-codes-api-openapi.yml
- filename: adt-access-control-api-openapi.yml
  format: yaml
  label: ADT Access Control API
  slug: adt-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-access-control-api-openapi.yml
- filename: adt-automation-api-openapi.yml
  format: yaml
  label: ADT Automation API
  slug: adt-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-automation-api-openapi.yml
- filename: adt-devices-api-openapi.yml
  format: yaml
  label: ADT Devices API
  slug: adt-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-devices-api-openapi.yml
- filename: adt-events-api-openapi.yml
  format: yaml
  label: ADT Events API
  slug: adt-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-events-api-openapi.yml
- filename: adt-reports-api-openapi.yml
  format: yaml
  label: ADT Reports API
  slug: adt-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-reports-api-openapi.yml
- filename: adt-security-systems-api-openapi.yml
  format: yaml
  label: ADT Security Systems API
  slug: adt-security-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-security-systems-api-openapi.yml
- filename: adt-sites-api-openapi.yml
  format: yaml
  label: ADT Sites API
  slug: adt-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-sites-api-openapi.yml
- filename: adt-users-api-openapi.yml
  format: yaml
  label: ADT Users API
  slug: adt-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-users-api-openapi.yml
- filename: adt-video-api-openapi.yml
  format: yaml
  label: ADT Video API
  slug: adt-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-video-api-openapi.yml
authorization_urls:
- https://auth.adt.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Adt Scopes
name_suffix: OAuth Scopes
note: These are the scopes ADT's own OpenID Connect issuer (https://auth.adt.com) advertises in scopes_supported. They are the Salesforce Experience Cloud platform scope catalog as exposed by ADT's tenant, not scopes ADT designed for a developer API — ADT publishes no developer API. Recorded because they are what ADT actually serves. This supersedes the 2026-07-11 file, whose scopes were derived from OpenAPI documents API Evangelist authored (openapi/_ae-authored/) and which ADT never published.
overview: 'ADT publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ADT API on a user''s behalf.


  Tokens are issued from https://auth.adt.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ADT
provider_slug: adt
schemes:
- flows:
  - authorizationUrl: https://auth.adt.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.adt.com/services/oauth2/token
  issuer: https://auth.adt.com
  name: openIdConnect
  source: well-known/adt-openid-configuration.json
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
  flows: []
  scope: address
- description: ''
  flows: []
  scope: api
- description: ''
  flows: []
  scope: cdp_api
- description: ''
  flows: []
  scope: cdp_calculated_insight_api
- description: ''
  flows: []
  scope: cdp_identityresolution_api
- description: ''
  flows: []
  scope: cdp_ingest_api
- description: ''
  flows: []
  scope: cdp_profile_api
- description: ''
  flows: []
  scope: cdp_query_api
- description: ''
  flows: []
  scope: cdp_segment_api
- description: ''
  flows: []
  scope: chatbot_api
- description: ''
  flows: []
  scope: chatter_api
- description: ''
  flows: []
  scope: content
- description: ''
  flows: []
  scope: custom_permissions
- description: ''
  flows: []
  scope: data_cloud_user_claims
- description: ''
  flows: []
  scope: eclair_api
- description: ''
  flows: []
  scope: einstein_gpt_api
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: forgot_password
- description: ''
  flows: []
  scope: full
- description: ''
  flows: []
  scope: id
- description: ''
  flows: []
  scope: interaction_api
- description: ''
  flows: []
  scope: lightning
- description: ''
  flows: []
  scope: mcp_api
- description: ''
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: pardot_api
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: pwdless_login_api
- description: ''
  flows: []
  scope: refresh_token
- description: ''
  flows: []
  scope: scrt_api
- description: ''
  flows: []
  scope: sfap_api
- description: ''
  flows: []
  scope: user_registration_api
- description: ''
  flows: []
  scope: visualforce
- description: ''
  flows: []
  scope: wave_api
- description: ''
  flows: []
  scope: web
slug: adt-scopes
source_filename: adt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://auth.adt.com/.well-known/openid-configuration (HTTP 200, fetched 2026-08-30; saved to\n  well-known/adt-openid-configuration.json)\nprovider: ADT\nproviderId: adt\nnote: These are the scopes ADT's own OpenID Connect issuer (https://auth.adt.com) advertises in scopes_supported.\n  They are the Salesforce Experience Cloud platform scope catalog as exposed by ADT's tenant, not scopes\n  ADT designed for a developer API — ADT publishes no developer API. Recorded because they are what ADT\n  actually serves. This supersedes the 2026-07-11 file, whose scopes were derived from OpenAPI documents\n  API Evangelist authored (openapi/_ae-authored/) and which ADT never published.\nschemes:\n- name: openIdConnect\n  issuer: https://auth.adt.com\n  source: well-known/adt-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.adt.com/services/oauth2/authorize\n    tokenUrl: https://auth.adt.com/services/oauth2/token\n\
  scope_count: 36\nscopes:\n- scope: address\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: cdp_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: cdp_calculated_insight_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: cdp_identityresolution_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: cdp_ingest_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: cdp_profile_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: cdp_query_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: cdp_segment_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: chatbot_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: chatter_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: content\n  sources:\n  - well-known/adt-openid-configuration.json\n\
  - scope: custom_permissions\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: data_cloud_user_claims\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: eclair_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: einstein_gpt_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: email\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: forgot_password\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: full\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: id\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: interaction_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: lightning\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: mcp_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: offline_access\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: openid\n  sources:\n  - well-known/adt-openid-configuration.json\n\
  - scope: pardot_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: phone\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: profile\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: pwdless_login_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: refresh_token\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: scrt_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: sfap_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: user_registration_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: visualforce\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: wave_api\n  sources:\n  - well-known/adt-openid-configuration.json\n- scope: web\n  sources:\n  - well-known/adt-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/scopes/adt-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
- Fortune 1000
token_urls:
- https://auth.adt.com/services/oauth2/token
---
