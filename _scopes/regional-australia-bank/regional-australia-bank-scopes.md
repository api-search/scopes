---
api_specs:
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Product Reference Data API
  slug: regional-australia-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Accounts & Balances API
  slug: regional-australia-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Transactions API
  slug: regional-australia-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Direct Debits & Scheduled Payments API
  slug: regional-australia-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
- filename: regional-australia-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Regional Australia Bank CDR Payees API
  slug: regional-australia-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/openapi/regional-australia-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Regional Australia Bank Scopes
name_suffix: OAuth Scopes
note: Regional Australia Bank participates in Australia's Consumer Data Right (CDR) as an accredited data holder. The public Product Reference Data (PRD) surface is unauthenticated and requires NO scope. The authenticated consumer data sharing operations defined by the shared CDS Banking API contract are secured under the CDR security profile (OAuth2 / OpenID Connect, FAPI-aligned) and are accessible only to accredited data recipients registered on the CDR Register. The scopes below are the CDR banking authorisation scopes carried as `x-scopes` extensions on the operations in the harvested CDS spec; they are the DSB standard scopes, not a Regional-Australia-Bank-proprietary set.
overview: 'Regional Australia Bank publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Regional Australia Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Regional Australia Bank
provider_slug: regional-australia-bank
schemes:
- flows:
  - flow: authorizationCode
    note: Authorization Code with PKCE; issuer/authorization/token endpoints are published per data holder via OIDC discovery at the data holder's CDR InfoSec baseURI (not exposed on the public PRD host).
  name: CDR-OAuth2-OIDC
  profile: CDR security profile (FAPI 1.0 Advanced-aligned)
  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  type: oauth2
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Read basic banking account information (account list and summary).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed banking account information for a specific account.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read banking transactions for authorised accounts.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read scheduled payments and direct debits for authorised accounts.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Read saved payees for authorised accounts.
  flows:
  - authorizationCode
  scope: bank:payees:read
slug: regional-australia-bank-scopes
source_filename: regional-australia-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/regional-australia-bank-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  Regional Australia Bank participates in Australia's Consumer Data Right (CDR)\n  as an accredited data holder. The public Product Reference Data (PRD) surface\n  is unauthenticated and requires NO scope. The authenticated consumer data\n  sharing operations defined by the shared CDS Banking API contract are secured\n  under the CDR security profile (OAuth2 / OpenID Connect, FAPI-aligned) and are\n  accessible only to accredited data recipients registered on the CDR Register.\n  The scopes below are the CDR banking authorisation scopes carried as `x-scopes`\n  extensions on the operations in the harvested CDS spec; they are the DSB\n  standard scopes, not a Regional-Australia-Bank-proprietary set.\nschemes:\n  - name: CDR-OAuth2-OIDC\n    type: oauth2\n    profile:\
  \ CDR security profile (FAPI 1.0 Advanced-aligned)\n    source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n    flows:\n      - flow: authorizationCode\n        note: >-\n          Authorization Code with PKCE; issuer/authorization/token endpoints are\n          published per data holder via OIDC discovery at the data holder's\n          CDR InfoSec baseURI (not exposed on the public PRD host).\nscopes:\n  - scope: bank:accounts.basic:read\n    description: Read basic banking account information (account list and summary).\n    flows: [authorizationCode]\n    sources: [openapi/regional-australia-bank-cds-banking-products-openapi.yml]\n  - scope: bank:accounts.detail:read\n    description: Read detailed banking account information for a specific account.\n    flows: [authorizationCode]\n    sources: [openapi/regional-australia-bank-cds-banking-products-openapi.yml]\n  - scope: bank:transactions:read\n    description: Read banking transactions for authorised\
  \ accounts.\n    flows: [authorizationCode]\n    sources: [openapi/regional-australia-bank-cds-banking-products-openapi.yml]\n  - scope: bank:regular_payments:read\n    description: Read scheduled payments and direct debits for authorised accounts.\n    flows: [authorizationCode]\n    sources: [openapi/regional-australia-bank-cds-banking-products-openapi.yml]\n  - scope: bank:payees:read\n    description: Read saved payees for authorised accounts.\n    flows: [authorizationCode]\n    sources: [openapi/regional-australia-bank-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regional-australia-bank/refs/heads/main/scopes/regional-australia-bank-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Customer-Owned
- Product Reference Data
- Mutual Bank
token_urls: []
---
