---
api_specs:
- filename: spare-account-api-openapi.yml
  format: yaml
  label: Spare Account API
  slug: spare-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-account-api-openapi.yml
- filename: spare-accountinformationreport-api-openapi.yml
  format: yaml
  label: Spare AccountInformationReport API
  slug: spare-accountinformationreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-accountinformationreport-api-openapi.yml
- filename: spare-balance-api-openapi.yml
  format: yaml
  label: Spare Balance API
  slug: spare-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-balance-api-openapi.yml
- filename: spare-beneficiary-api-openapi.yml
  format: yaml
  label: Spare Beneficiary API
  slug: spare-beneficiary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-beneficiary-api-openapi.yml
- filename: spare-cert-api-openapi.yml
  format: yaml
  label: Spare Cert API
  slug: spare-cert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-cert-api-openapi.yml
- filename: spare-connection-api-openapi.yml
  format: yaml
  label: Spare Connection API
  slug: spare-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-connection-api-openapi.yml
- filename: spare-consent-api-openapi.yml
  format: yaml
  label: Spare Consent API
  slug: spare-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-consent-api-openapi.yml
- filename: spare-customer-api-openapi.yml
  format: yaml
  label: Spare Customer API
  slug: spare-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-customer-api-openapi.yml
- filename: spare-directdebit-api-openapi.yml
  format: yaml
  label: Spare DirectDebit API
  slug: spare-directdebit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-directdebit-api-openapi.yml
- filename: spare-parties-api-openapi.yml
  format: yaml
  label: Spare Parties API
  slug: spare-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-parties-api-openapi.yml
- filename: spare-payment-api-openapi.yml
  format: yaml
  label: Spare Payment API
  slug: spare-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-payment-api-openapi.yml
- filename: spare-provider-api-openapi.yml
  format: yaml
  label: Spare Provider API
  slug: spare-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-provider-api-openapi.yml
- filename: spare-request-api-openapi.yml
  format: yaml
  label: Spare Request API
  slug: spare-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-request-api-openapi.yml
- filename: spare-riskreport-api-openapi.yml
  format: yaml
  label: Spare RiskReport API
  slug: spare-riskreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-riskreport-api-openapi.yml
- filename: spare-statement-api-openapi.yml
  format: yaml
  label: Spare Statement API
  slug: spare-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-statement-api-openapi.yml
- filename: spare-token-api-openapi.yml
  format: yaml
  label: Spare Token API
  slug: spare-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-token-api-openapi.yml
- filename: spare-transaction-api-openapi.yml
  format: yaml
  label: Spare Transaction API
  slug: spare-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-transaction-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.tryspare.com/docs/consent-1
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Spare Scopes
name_suffix: OAuth Scopes
note: Spare authenticates with OAuth2 client-credentials (see authentication/), but data access is governed by an open-banking CONSENT permission model rather than token scopes. When creating a Consent the client requests a set of AccountInformationPermission values; the end user authorises them in their bank app, and each AIS operation requires specific permissions on the active consent (the API reference lists the required permissions per endpoint). These consent permissions are the effective scope surface and are enumerated verbatim below.
overview: 'Spare uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spare
provider_slug: spare
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: spare-scopes
source_filename: spare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi AccountInformationPermission + ConsentScope enums (all AIS/PIS specs)\ndocs: https://docs.tryspare.com/docs/consent-1\nnote: >-\n  Spare authenticates with OAuth2 client-credentials (see authentication/), but\n  data access is governed by an open-banking CONSENT permission model rather than\n  token scopes. When creating a Consent the client requests a set of\n  AccountInformationPermission values; the end user authorises them in their bank\n  app, and each AIS operation requires specific permissions on the active consent\n  (the API reference lists the required permissions per endpoint). These consent\n  permissions are the effective scope surface and are enumerated verbatim below.\nconsent_scopes:\n- scope: Accounts\n  description: Account Information Services consent scope.\n- scope: Payments\n  description: Payment Initiation Services consent scope.\naccount_information_permissions:\n- ReadAccountsBasic\n- ReadAccountsDetail\n\
  - ReadBalances\n- ReadBeneficiariesBasic\n- ReadBeneficiariesDetail\n- ReadDirectDebits\n- ReadTransactionsBasic\n- ReadTransactionsDetail\n- ReadTransactionsCredits\n- ReadTransactionsDebits\n- ReadStatementsBasic\n- ReadStatementsDetail\n- ReadSupplementaryAccountInfo\n- ReadOffers\n- ReadParty\n- ReadPartyCustomer\n- ReadFutureDatedPaymentsBasic\n- ReadFutureDatedPaymentsDetail\n- ReadPAN\n- ReadPartyPSU\n- ReadPartyPSUIdentity\n- ReadScheduledPaymentsBasic\n- ReadScheduledPaymentsDetail\n- ReadStandingOrdersBasic\n- ReadStandingOrdersDetail\nexample_required_permissions:\n- operation: GET /api/v1.0/ais/Account/List\n  permissions: [ReadAccountsBasic, ReadAccountsDetail]\n- operation: GET /api/v1.0/ais/Balance/Get\n  permissions: [ReadAccountsBasic, ReadAccountsDetail, ReadBalances]\n- operation: GET /api/v1.0/ais/Balance/History\n  permissions: [ReadAccountsBasic, ReadAccountsDetail, ReadBalances, ReadTransactionsBasic, ReadTransactionsDetail, ReadTransactionsDebits, ReadTransactionsCredits]\n\
  - operation: GET /api/v1.0/ais/Beneficiary/Get\n  permissions: [ReadBeneficiariesBasic, ReadBeneficiariesDetail]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/scopes/spare-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Open Banking
- Open Finance
- Account Information
- Payment Initiation
- AISP
- PISP
- Consent
- Bank Data
- Transaction
- Balances
- Payments
- Fintech
- MENA
- Saudi Arabia
- Bahrain
- UAE
token_urls: []
---
