---
api_specs:
- filename: marriott-tip-internet-portal-api-openapi.json
  format: json
  label: Marriott TIP Internet Portal API
  slug: marriott-tip-internet-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-tip-internet-portal-api-openapi.json
- filename: marriott-loyalty-account-merge-api-openapi.json
  format: json
  label: Marriott Loyalty Account Merge API
  slug: marriott-loyalty-account-merge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-loyalty-account-merge-api-openapi.json
- filename: marriott-data-collection-api-openapi.json
  format: json
  label: Marriott Data Collection API
  slug: marriott-data-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-collection-api-openapi.json
- filename: marriott-commerce-payment-processor-api-openapi.json
  format: json
  label: Marriott Commerce Payment Processor API
  slug: marriott-commerce-payment-processor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-commerce-payment-processor-api-openapi.json
- filename: marriott-finance-status-notifier-api-openapi.json
  format: json
  label: Marriott Finance Status Notifier API
  slug: marriott-finance-status-notifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-finance-status-notifier-api-openapi.json
- filename: marriott-hotel-operations-ara-api-openapi.json
  format: json
  label: Marriott Hotel Operations ARA Preview Submit API
  slug: marriott-hotel-operations-ara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-hotel-operations-ara-api-openapi.json
authorization_urls:
- /v3/ent-auth/sso/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Marriott Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Marriott International publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Marriott International API on a user''s behalf.


  Tokens are issued from /v3/ent-auth/sso/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Marriott International
provider_slug: marriott
schemes:
- flows:
  - authorizationUrl: /v3/ent-auth/sso/authorize
    flow: authorizationCode
    tokenUrl: /v3/ent-auth/sso/token
  name: OAuth2
  source: openapi/marriott-commerce-payment-processor-api-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: http://example.com/oauth/token
  name: application
  source: openapi/marriott-finance-status-notifier-api-openapi.json
scope_count: 2
scope_names:
- MANAGE_ACCT_AUTH_E
- write
scopes:
- description: Grants access to High Risk Transaction to update
  flows:
  - authorizationCode
  scope: MANAGE_ACCT_AUTH_E
- description: allows modifying resources
  flows:
  - clientCredentials
  scope: write
slug: marriott-scopes
source_filename: marriott-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: openapi/marriott-commerce-payment-processor-api-openapi.json, openapi/marriott-finance-status-notifier-api-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/marriott-commerce-payment-processor-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v3/ent-auth/sso/authorize\n    tokenUrl: /v3/ent-auth/sso/token\n- name: application\n  source: openapi/marriott-finance-status-notifier-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: http://example.com/oauth/token\nscopes:\n- scope: MANAGE_ACCT_AUTH_E\n  description: Grants access to High Risk Transaction to update\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/marriott-commerce-payment-processor-api-openapi.json\n- scope: write\n  description: allows modifying resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/marriott-finance-status-notifier-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/scopes/marriott-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Distribution
- Loyalty
- Short-Term Rental
- Corporate Travel
token_urls:
- /v3/ent-auth/sso/token
- http://example.com/oauth/token
---
