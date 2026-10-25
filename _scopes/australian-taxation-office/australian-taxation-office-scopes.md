---
api_specs:
- filename: australian-taxation-office-apiinfo-api-openapi.yml
  format: yaml
  label: Australian Taxation Office API Info API
  slug: australian-taxation-office-apiinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-apiinfo-api-openapi.yml
- filename: australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Combined Global and Domestic Group Entity Tax Return API
  slug: australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api-openapi.yml
- filename: australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Combined Global and Domestic Minimum Tax Return API
  slug: australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api-openapi.yml
- filename: australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Get Payee Stapled Super Fund for Receipt API
  slug: australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api-openapi.yml
- filename: australian-taxation-office-get-payment-reference-number-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Get Payment Reference Number API
  slug: australian-taxation-office-get-payment-reference-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-get-payment-reference-number-api-openapi.yml
- filename: australian-taxation-office-gst-property-settlement-date-confirmation-api-openapi.yml
  format: yaml
  label: Australian Taxation Office GST Property Settlement Date Confirmation API
  slug: australian-taxation-office-gst-property-settlement-date-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-gst-property-settlement-date-confirmation-api-openapi.yml
- filename: australian-taxation-office-gst-property-settlement-withholding-notification-api-openapi.yml
  format: yaml
  label: Australian Taxation Office GST Property Settlement Withholding Notification API
  slug: australian-taxation-office-gst-property-settlement-withholding-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-gst-property-settlement-withholding-notification-api-openapi.yml
- filename: australian-taxation-office-heartbeat-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Heartbeat API
  slug: australian-taxation-office-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-heartbeat-api-openapi.yml
- filename: australian-taxation-office-providers-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Providers API
  slug: australian-taxation-office-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-providers-api-openapi.yml
- filename: australian-taxation-office-register-a-new-software-application-instance-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Register a new software application instance API
  slug: australian-taxation-office-register-a-new-software-application-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-register-a-new-software-application-instance-api-openapi.yml
- filename: australian-taxation-office-request-stapled-super-fund-for-payee-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Request Stapled Super Fund for Payee API
  slug: australian-taxation-office-request-stapled-super-fund-for-payee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-request-stapled-super-fund-for-payee-api-openapi.yml
- filename: australian-taxation-office-spec-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Spec API
  slug: australian-taxation-office-spec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-spec-api-openapi.yml
authorization_urls: []
description: ''
docs: https://apiportal.ato.gov.au/client-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Australian Taxation Office Scopes
name_suffix: OAuth Scopes
note: '"Scopes will vary for each API and will be available in the corresponding API documentation of each API" and "Scopes will be the same for sandbox testing and production use." Product pages confirm ato.healthcheck.*.* (Health Check) and ato.idp.relyingParties.c (OAuth DCR).'
overview: 'Australian Taxation Office publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Australian Taxation Office API on a user''s behalf.


  Tokens are issued from {env}/core2/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Australian Taxation Office
provider_slug: australian-taxation-office
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: '{env}/core2/connect/token'
  name: ScopeAuth
  source: openapi/australian-taxation-office-gst-property-settlement-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.ato.gov.au/core2/connect/token
  name: ScopeAuth
  source: openapi/australian-taxation-office-health-check-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.ato.gov.au/core2/connect/token
  name: ScopeAuth
  source: openapi/australian-taxation-office-oauth-dynamic-client-registration-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.evte.ato.gov.au/core2/connect/token
  name: ScopeAuth
  source: openapi/australian-taxation-office-stapled-super-fund-openapi.yml
scope_count: 4
scope_names:
- ato.apGSTPropertySettlement
- ato.healthcheck.*.*
- ato.idp.relyingParties.c
- ato.super.stapledsuperfund.c,r
scopes:
- description: Grants ability to lodge GST on Property Settlement Forms
  flows:
  - clientCredentials
  scope: ato.apGSTPropertySettlement
- description: Grants ability to access the Healthcheck API
  flows:
  - clientCredentials
  scope: ato.healthcheck.*.*
- description: Grants ability to register (POST) a new software application
  flows:
  - clientCredentials
  scope: ato.idp.relyingParties.c
- description: Grants ability to POST and GET a Stapled Super Fund
  flows:
  - clientCredentials
  scope: ato.super.stapledsuperfund.c,r
slug: australian-taxation-office-scopes
source_filename: australian-taxation-office-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://apiportal.ato.gov.au/client-authentication\nschemes:\n- name: ScopeAuth\n  source: openapi/australian-taxation-office-gst-property-settlement-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: '{env}/core2/connect/token'\n- name: ScopeAuth\n  source: openapi/australian-taxation-office-health-check-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.ato.gov.au/core2/connect/token\n- name: ScopeAuth\n  source: openapi/australian-taxation-office-oauth-dynamic-client-registration-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.ato.gov.au/core2/connect/token\n- name: ScopeAuth\n  source: openapi/australian-taxation-office-stapled-super-fund-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.evte.ato.gov.au/core2/connect/token\nscopes:\n- scope: ato.apGSTPropertySettlement\n  description: Grants ability to lodge GST on Property\
  \ Settlement Forms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/australian-taxation-office-gst-property-settlement-openapi.yml\n- scope: ato.healthcheck.*.*\n  description: Grants ability to access the Healthcheck API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/australian-taxation-office-health-check-openapi.yml\n- scope: ato.idp.relyingParties.c\n  description: Grants ability to register (POST) a new software application\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/australian-taxation-office-oauth-dynamic-client-registration-openapi.yml\n- scope: ato.super.stapledsuperfund.c,r\n  description: Grants ability to POST and GET a Stapled Super Fund\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/australian-taxation-office-stapled-super-fund-openapi.yml\ndocs: https://apiportal.ato.gov.au/client-authentication\nnote: '\"Scopes will vary for each API and will be available in the corresponding API documentation of each API\" and \"Scopes will\
  \ be the same for sandbox testing and production use.\" Product pages confirm\n  ato.healthcheck.*.* (Health Check) and ato.idp.relyingParties.c (OAuth DCR).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/scopes/australian-taxation-office-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Company
- Government
- Taxation
- Superannuation
- Australia
- Digital Service Providers
- Public Sector
token_bound: false
token_urls:
- '{env}/core2/connect/token'
- https://auth.ato.gov.au/core2/connect/token
- https://auth.evte.ato.gov.au/core2/connect/token
---
