---
api_specs:
- filename: grubhub-delivery-status-api-openapi.yml
  format: yaml
  label: grubhub Delivery Status API
  slug: grubhub-delivery-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-status-api-openapi.yml
- filename: grubhub-driver-communication-api-openapi.yml
  format: yaml
  label: grubhub Driver Communication API
  slug: grubhub-driver-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-driver-communication-api-openapi.yml
- filename: grubhub-issue-reporting-api-openapi.yml
  format: yaml
  label: grubhub Issue Reporting API
  slug: grubhub-issue-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-issue-reporting-api-openapi.yml
- filename: grubhub-menu-ingestion-api-openapi.yml
  format: yaml
  label: grubhub Menu Ingestion API
  slug: grubhub-menu-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-ingestion-api-openapi.yml
- filename: grubhub-menu-retrieval-api-openapi.yml
  format: yaml
  label: grubhub Menu Retrieval API
  slug: grubhub-menu-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-retrieval-api-openapi.yml
- filename: grubhub-menu-schedule-overrides-api-openapi.yml
  format: yaml
  label: grubhub Menu Schedule Overrides API
  slug: grubhub-menu-schedule-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-schedule-overrides-api-openapi.yml
- filename: grubhub-merchant-eligibility-api-openapi.yml
  format: yaml
  label: grubhub Merchant Eligibility API
  slug: grubhub-merchant-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-eligibility-api-openapi.yml
- filename: grubhub-merchant-onboarding-api-openapi.yml
  format: yaml
  label: grubhub Merchant Onboarding API
  slug: grubhub-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-onboarding-api-openapi.yml
- filename: grubhub-merchant-properties-api-openapi.yml
  format: yaml
  label: grubhub Merchant Properties API
  slug: grubhub-merchant-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-properties-api-openapi.yml
- filename: grubhub-merchant-status-api-openapi.yml
  format: yaml
  label: grubhub Merchant Status API
  slug: grubhub-merchant-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-status-api-openapi.yml
- filename: grubhub-merchants-api-openapi.yml
  format: yaml
  label: grubhub Merchants API
  slug: grubhub-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchants-api-openapi.yml
- filename: grubhub-order-change-requests-api-openapi.yml
  format: yaml
  label: grubhub Order Change Requests API
  slug: grubhub-order-change-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-order-change-requests-api-openapi.yml
- filename: grubhub-order-polling-api-openapi.yml
  format: yaml
  label: grubhub Order Polling API
  slug: grubhub-order-polling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-order-polling-api-openapi.yml
- filename: grubhub-order-status-api-openapi.yml
  format: yaml
  label: grubhub Order Status API
  slug: grubhub-order-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-order-status-api-openapi.yml
- filename: grubhub-orders-api-openapi.yml
  format: yaml
  label: grubhub Orders API
  slug: grubhub-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-api-openapi.yml
- filename: grubhub-schedule-overrides-api-openapi.yml
  format: yaml
  label: grubhub Schedule Overrides API
  slug: grubhub-schedule-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-schedule-overrides-api-openapi.yml
- filename: grubhub-schedules-api-openapi.yml
  format: yaml
  label: grubhub Schedules API
  slug: grubhub-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-schedules-api-openapi.yml
authorization_urls: []
description: ''
docs: https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Grubhub Scopes
name_suffix: OAuth Scopes
note: Grubhub's partner Onboarding/Menu/Orders APIs use OAuth client credentials without published named scopes; the only documented scope values ("anonymous" and "openid diner") appear in the Grubhub Developers Open ID Authentication guide for diner-facing ordering integrations.
overview: 'grubhub publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the grubhub API on a user''s behalf.


  Tokens are issued from /oauth2/direct/auth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: grubhub
provider_slug: grubhub
schemes:
- description: OAuth 2.0 authentication for the Onboarding API. Partners use OAuth to authenticate merchant onboarding operations.
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/direct/auth
  name: oauthAuth
  source: openapi/grubhub-onboarding-openapi.yml
scope_count: 2
scope_names:
- anonymous
- openid diner
scopes:
- description: Anonymous authentication via POST /oauth2/direct/auth (grant_type token). Returns an access token that can be used to browse restaurant information and begin an order without a logged-in diner; any call except checkout is permitted until the session is connected to an authenticated diner.
  flows: []
  scope: anonymous
- description: Required scope value when authenticating a diner via POST /oauth2/direct/auth with a signed OpenID token (grant_type token). Links the partner application's user to a Grubhub diner record and returns an access token for making Grubhub API calls on that diner's behalf, including checkout.
  flows: []
  scope: openid diner
slug: grubhub-scopes
source_filename: grubhub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/grubhub-onboarding-openapi.yml\ndocs: https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication\nschemes:\n- name: oauthAuth\n  source: openapi/grubhub-onboarding-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/direct/auth\n  description: OAuth 2.0 authentication for the Onboarding API. Partners use OAuth to authenticate\n    merchant onboarding operations.\nscopes:\n- scope: anonymous\n  description: Anonymous authentication via POST /oauth2/direct/auth (grant_type token). Returns\n    an access token that can be used to browse restaurant information and begin an order without\n    a logged-in diner; any call except checkout is permitted until the session is connected to\n    an authenticated diner.\n  sources:\n  - https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication\n- scope: openid diner\n  description: Required\
  \ scope value when authenticating a diner via POST /oauth2/direct/auth with\n    a signed OpenID token (grant_type token). Links the partner application's user to a Grubhub\n    diner record and returns an access token for making Grubhub API calls on that diner's behalf,\n    including checkout.\n  sources:\n  - https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication\nnote: Grubhub's partner Onboarding/Menu/Orders APIs use OAuth client credentials without published\n  named scopes; the only documented scope values (\"anonymous\" and \"openid diner\") appear in the\n  Grubhub Developers Open ID Authentication guide for diner-facing ordering integrations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/scopes/grubhub-scopes.yml
summary_line: 2 scopes · clientCredentials
tags: []
token_urls:
- /oauth2/direct/auth
---
