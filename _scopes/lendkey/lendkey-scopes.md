---
api_specs:
- filename: lendkey-application-contracts-api-openapi.yml
  format: yaml
  label: LendKey Application Contracts API
  slug: lendkey-application-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-application-contracts-api-openapi.yml
- filename: lendkey-applications-api-openapi.yml
  format: yaml
  label: LendKey applications API
  slug: lendkey-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-applications-api-openapi.yml
- filename: lendkey-auth-api-openapi.yml
  format: yaml
  label: LendKey auth API
  slug: lendkey-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-auth-api-openapi.yml
- filename: lendkey-authentication-api-openapi.yml
  format: yaml
  label: LendKey Authentication API
  slug: lendkey-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-authentication-api-openapi.yml
- filename: lendkey-credit-risk-api-openapi.yml
  format: yaml
  label: LendKey Credit Risk API
  slug: lendkey-credit-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-credit-risk-api-openapi.yml
- filename: lendkey-disbursements-api-openapi.yml
  format: yaml
  label: LendKey Disbursements API
  slug: lendkey-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-disbursements-api-openapi.yml
- filename: lendkey-email-api-openapi.yml
  format: yaml
  label: LendKey email API
  slug: lendkey-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-email-api-openapi.yml
- filename: lendkey-internal-api-openapi.yml
  format: yaml
  label: LendKey internal API
  slug: lendkey-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-internal-api-openapi.yml
- filename: lendkey-leads-api-openapi.yml
  format: yaml
  label: LendKey leads API
  slug: lendkey-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-leads-api-openapi.yml
- filename: lendkey-ledger-management-api-openapi.yml
  format: yaml
  label: LendKey Ledger Management API
  slug: lendkey-ledger-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-ledger-management-api-openapi.yml
- filename: lendkey-lender-templates-api-openapi.yml
  format: yaml
  label: LendKey Lender Templates API
  slug: lendkey-lender-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-lender-templates-api-openapi.yml
- filename: lendkey-loans-api-openapi.yml
  format: yaml
  label: LendKey Loans API
  slug: lendkey-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-loans-api-openapi.yml
- filename: lendkey-onboarding-api-openapi.yml
  format: yaml
  label: LendKey onboarding API
  slug: lendkey-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-onboarding-api-openapi.yml
- filename: lendkey-payments-api-openapi.yml
  format: yaml
  label: LendKey Payments API
  slug: lendkey-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-payments-api-openapi.yml
- filename: lendkey-webhooks-api-openapi.yml
  format: yaml
  label: LendKey Webhooks API
  slug: lendkey-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/openapi/lendkey-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Lendkey Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LendKey uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LendKey
provider_slug: lendkey
schemes:
- description: OAuth2 client credentials flow via Kong Gateway
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: oauth2
  source: openapi/lendkey-esign-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.lendkey.com/lo_partnerintegrationinternalapi/oauth2/token
  name: oauth2
  source: openapi/lendkey-partner-integration-internal-openapi.yml
- description: OAuth2 client credentials flow via Kong Gateway
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: oauth2
  source: openapi/lendkey-treasury-management-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: lendkey-scopes
source_filename: lendkey-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lendkey-esign-openapi.yml, openapi/lendkey-partner-integration-internal-openapi.yml,\n  openapi/lendkey-treasury-management-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/lendkey-esign-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  description: OAuth2 client credentials flow via Kong Gateway\n- name: oauth2\n  source: openapi/lendkey-partner-integration-internal-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.lendkey.com/lo_partnerintegrationinternalapi/oauth2/token\n- name: oauth2\n  source: openapi/lendkey-treasury-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\n  description: OAuth2 client credentials flow via Kong Gateway\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendkey/refs/heads/main/scopes/lendkey-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Fintech
- Lending
- Loans
- Student Loans
- Credit Unions
- Banking
- Loan Origination
- Financial-Services
- Payments
- E-Signature
- Treasury
token_urls:
- /oauth2/token
- https://api.lendkey.com/lo_partnerintegrationinternalapi/oauth2/token
---
