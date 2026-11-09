---
api_specs:
- filename: swift-payment-pre-validation-api-openapi.yml
  format: yaml
  label: Payment Pre-validation API
  slug: payment-pre-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-payment-pre-validation-api-openapi.yml
- filename: swift-account-numbers-api-openapi.yml
  format: yaml
  label: SWIFT Account Numbers API
  slug: swift-account-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-account-numbers-api-openapi.yml
- filename: swift-bbans-api-openapi.yml
  format: yaml
  label: SWIFT BBANs API
  slug: swift-bbans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-bbans-api-openapi.yml
- filename: swift-bics-api-openapi.yml
  format: yaml
  label: SWIFT BICs API
  slug: swift-bics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-bics-api-openapi.yml
- filename: swift-country-codes-api-openapi.yml
  format: yaml
  label: SWIFT Country Codes API
  slug: swift-country-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-country-codes-api-openapi.yml
- filename: swift-currency-codes-api-openapi.yml
  format: yaml
  label: SWIFT Currency Codes API
  slug: swift-currency-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-currency-codes-api-openapi.yml
- filename: swift-leis-api-openapi.yml
  format: yaml
  label: SWIFT LEIs API
  slug: swift-leis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-leis-api-openapi.yml
- filename: swift-national-ids-api-openapi.yml
  format: yaml
  label: SWIFT National IDs API
  slug: swift-national-ids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-national-ids-api-openapi.yml
- filename: swift-ibans-api-openapi.yml
  format: yaml
  label: SWIFT IBANs API
  slug: swift-ibans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-ibans-api-openapi.yml
- filename: swift-account-information-api-openapi.yml
  format: yaml
  label: SWIFT Account Information API
  slug: swift-account-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-account-information-api-openapi.yml
- filename: swift-distributions-api-openapi.yml
  format: yaml
  label: SWIFT Distributions API
  slug: swift-distributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-distributions-api-openapi.yml
- filename: swift-fileact-api-openapi.yml
  format: yaml
  label: SWIFT Fileact API
  slug: swift-fileact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-fileact-api-openapi.yml
- filename: swift-fin-api-openapi.yml
  format: yaml
  label: SWIFT Fin API
  slug: swift-fin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-fin-api-openapi.yml
- filename: swift-get-changed-payment-transactions-api-openapi.yml
  format: yaml
  label: SWIFT Get Changed Payment Transactions API
  slug: swift-get-changed-payment-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-get-changed-payment-transactions-api-openapi.yml
- filename: swift-get-payment-transaction-details-api-openapi.yml
  format: yaml
  label: SWIFT Get Payment Transaction Details API
  slug: swift-get-payment-transaction-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-get-payment-transaction-details-api-openapi.yml
- filename: swift-iban-national-ids-api-openapi.yml
  format: yaml
  label: SWIFT Iban National IDs API
  slug: swift-iban-national-ids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-iban-national-ids-api-openapi.yml
- filename: swift-interact-api-openapi.yml
  format: yaml
  label: SWIFT Interact API
  slug: swift-interact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-interact-api-openapi.yml
- filename: swift-pmis-api-openapi.yml
  format: yaml
  label: SWIFT Pmis API
  slug: swift-pmis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-pmis-api-openapi.yml
- filename: swift-reporting-api-openapi.yml
  format: yaml
  label: SWIFT Reporting API
  slug: swift-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-reporting-api-openapi.yml
- filename: swift-status-confirmations-api-openapi.yml
  format: yaml
  label: SWIFT Status Confirmations API
  slug: swift-status-confirmations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-status-confirmations-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Swift Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SWIFT publishes 2 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the SWIFT API on a user''s behalf.


  Tokens are issued from https://api.swift.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SWIFT
provider_slug: swift
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-account-numbers-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-bbans-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-bics-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-country-codes-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-currency-codes-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-ibans-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-leis-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-national-ids-api-openapi.yml
- description: 'This API uses OAuth2 with the client credentials grant type.


    Please visit [SWIFT OAuth Token API](https://developer.swift.com/swift-oauth-token-api) for more information and examples.'
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: oauthClientCredentials
  source: openapi/swift-payment-pre-validation-api-openapi.yml
scope_count: 2
scope_names:
- urn:swiftref:external
- urn:swiftref:internal
scopes:
- description: External customer access to SwiftRef data
  flows:
  - password
  scope: urn:swiftref:external
- description: Internal payment validation access
  flows:
  - password
  scope: urn:swiftref:internal
slug: swift-scopes
source_filename: swift-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/swift-account-numbers-api-openapi.yml, openapi/swift-bbans-api-openapi.yml,\n  openapi/swift-bics-api-openapi.yml, openapi/swift-country-codes-api-openapi.yml, openapi/swift-currency-codes-api-openapi.yml,\n  openapi/swift-ibans-api-openapi.yml, openapi/swift-leis-api-openapi.yml, openapi/swift-national-ids-api-openapi.yml,\n  openapi/swift-payment-pre-validation-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/swift-account-numbers-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n- name: OAuth2\n  source: openapi/swift-bbans-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n- name: OAuth2\n  source: openapi/swift-bics-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n- name: OAuth2\n  source: openapi/swift-country-codes-api-openapi.yml\n  flows:\n  - flow:\
  \ password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n- name: OAuth2\n  source: openapi/swift-currency-codes-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n- name: OAuth2\n  source: openapi/swift-ibans-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n- name: OAuth2\n  source: openapi/swift-leis-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n- name: OAuth2\n  source: openapi/swift-national-ids-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n- name: oauthClientCredentials\n  source: openapi/swift-payment-pre-validation-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: |-\n    This API uses OAuth2 with the client credentials grant type.\n\n    Please visit [SWIFT OAuth Token API](https://developer.swift.com/swift-oauth-token-api)\
  \ for more information and examples.\nscopes:\n- scope: urn:swiftref:external\n  description: External customer access to SwiftRef data\n  flows:\n  - password\n  sources:\n  - openapi/swift-account-numbers-api-openapi.yml\n  - openapi/swift-bbans-api-openapi.yml\n  - openapi/swift-bics-api-openapi.yml\n  - openapi/swift-country-codes-api-openapi.yml\n  - openapi/swift-currency-codes-api-openapi.yml\n  - openapi/swift-ibans-api-openapi.yml\n  - openapi/swift-leis-api-openapi.yml\n  - openapi/swift-national-ids-api-openapi.yml\n- scope: urn:swiftref:internal\n  description: Internal payment validation access\n  flows:\n  - password\n  sources:\n  - openapi/swift-account-numbers-api-openapi.yml\n  - openapi/swift-bbans-api-openapi.yml\n  - openapi/swift-bics-api-openapi.yml\n  - openapi/swift-country-codes-api-openapi.yml\n  - openapi/swift-currency-codes-api-openapi.yml\n  - openapi/swift-ibans-api-openapi.yml\n  - openapi/swift-leis-api-openapi.yml\n  - openapi/swift-national-ids-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/swift/scopes/swift-scopes.yml
summary_line: 2 scopes · password/clientCredentials
tags:
- Banking
- Cross-Border Payments
- Financial Messaging
- Financial Services
- GPI
- ISO 20022
- Payments
- SWIFT
token_bound: false
token_urls:
- https://api.swift.com/oauth2/v1/token
- /v1/oauth2/token
---
