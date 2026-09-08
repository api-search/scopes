---
authorization_urls:
- https://support.cvent.com/services/oauth2/authorize
description: ''
docs: https://support.cvent.com/s/knowledgebase
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cvent Community Scopes
name_suffix: OAuth Scopes
note: These are the OAuth 2.0 / OIDC scopes advertised by the Cvent support + knowledge base portal at support.cvent.com, read verbatim from its OpenID Connect discovery document. They are Salesforce Experience Cloud's STANDARD scope vocabulary as exposed by Cvent's Salesforce org — not a scope taxonomy Cvent authored for a Cvent Community API. Cvent Community publishes no API contract; this file records the identity surface that actually answers, and nothing more. The scopes governing the callable Cvent Platform REST API are a different set and live at all/cvent/scopes/cvent-scopes.yml.
overview: 'Cvent Community publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cvent Community API on a user''s behalf.


  Tokens are issued from https://support.cvent.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cvent Community
provider_slug: cvent-community
schemes:
- flows:
  - authorizationUrl: https://support.cvent.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://support.cvent.com/services/oauth2/token
  issuer: https://support.cvent.com
  name: support-cvent-oidc
  source: well-known/cvent-community-openid-configuration.json
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
  flows:
  - authorizationCode
  scope: address
- description: ''
  flows:
  - authorizationCode
  scope: api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_calculated_insight_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_identityresolution_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_ingest_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_profile_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_query_api
- description: ''
  flows:
  - authorizationCode
  scope: cdp_segment_api
- description: ''
  flows:
  - authorizationCode
  scope: chatbot_api
- description: ''
  flows:
  - authorizationCode
  scope: chatter_api
- description: ''
  flows:
  - authorizationCode
  scope: content
- description: ''
  flows:
  - authorizationCode
  scope: custom_permissions
- description: ''
  flows:
  - authorizationCode
  scope: data_cloud_user_claims
- description: ''
  flows:
  - authorizationCode
  scope: eclair_api
- description: ''
  flows:
  - authorizationCode
  scope: einstein_gpt_api
- description: ''
  flows:
  - authorizationCode
  scope: email
- description: ''
  flows:
  - authorizationCode
  scope: forgot_password
- description: ''
  flows:
  - authorizationCode
  scope: full
- description: ''
  flows:
  - authorizationCode
  scope: id
- description: ''
  flows:
  - authorizationCode
  scope: interaction_api
- description: ''
  flows:
  - authorizationCode
  scope: lightning
- description: ''
  flows:
  - authorizationCode
  scope: mcp_api
- description: ''
  flows:
  - authorizationCode
  scope: offline_access
- description: ''
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: pardot_api
- description: ''
  flows:
  - authorizationCode
  scope: phone
- description: ''
  flows:
  - authorizationCode
  scope: profile
- description: ''
  flows:
  - authorizationCode
  scope: pwdless_login_api
- description: ''
  flows:
  - authorizationCode
  scope: refresh_token
- description: ''
  flows:
  - authorizationCode
  scope: scrt_api
- description: ''
  flows:
  - authorizationCode
  scope: sfap_api
- description: ''
  flows:
  - authorizationCode
  scope: user_registration_api
- description: ''
  flows:
  - authorizationCode
  scope: visualforce
- description: ''
  flows:
  - authorizationCode
  scope: wave_api
- description: ''
  flows:
  - authorizationCode
  scope: web
slug: cvent-community-scopes
source_filename: cvent-community-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://support.cvent.com/.well-known/openid-configuration (HTTP 200, fetched 2026-09-07)\ndocs: https://support.cvent.com/s/knowledgebase\nnote: >-\n  These are the OAuth 2.0 / OIDC scopes advertised by the Cvent support + knowledge base portal at\n  support.cvent.com, read verbatim from its OpenID Connect discovery document. They are Salesforce\n  Experience Cloud's STANDARD scope vocabulary as exposed by Cvent's Salesforce org — not a scope\n  taxonomy Cvent authored for a Cvent Community API. Cvent Community publishes no API contract; this\n  file records the identity surface that actually answers, and nothing more. The scopes governing the\n  callable Cvent Platform REST API are a different set and live at all/cvent/scopes/cvent-scopes.yml.\nschemes:\n  - name: support-cvent-oidc\n    source: well-known/cvent-community-openid-configuration.json\n    issuer: https://support.cvent.com\n    flows:\n      - flow: authorizationCode\n\
  \        authorizationUrl: https://support.cvent.com/services/oauth2/authorize\n        tokenUrl: https://support.cvent.com/services/oauth2/token\nscope_count: 36\nscopes:\n  - scope: address\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: cdp_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: cdp_calculated_insight_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: cdp_identityresolution_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: cdp_ingest_api\n    description: null\n    flows: [authorizationCode]\n\
  \    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: cdp_profile_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: cdp_query_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: cdp_segment_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: chatbot_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: chatter_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: content\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: custom_permissions\n    description:\
  \ null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: data_cloud_user_claims\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: eclair_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: einstein_gpt_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: email\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: forgot_password\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: full\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n\
  \  - scope: id\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: interaction_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: lightning\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: mcp_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: offline_access\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: openid\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: pardot_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n\
  \  - scope: phone\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: profile\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: pwdless_login_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: refresh_token\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: scrt_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: sfap_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: user_registration_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n\
  \  - scope: visualforce\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: wave_api\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n  - scope: web\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cvent-community-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-community/refs/heads/main/scopes/cvent-community-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Certification
- Community
- Customer-Support
- Cvent Academy
- Education
- Forums
- Knowledge Base
- Learning Centers
- Software-as-a-Service
- Training
token_urls:
- https://support.cvent.com/services/oauth2/token
---
