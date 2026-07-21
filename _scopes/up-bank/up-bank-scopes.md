---
api_specs:
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Product Reference Data API
  slug: up-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Accounts & Balances API
  slug: up-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Transactions API
  slug: up-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Direct Debits & Scheduled Payments API
  slug: up-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Up CDR Payees API
  slug: up-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-cds-banking-products-openapi.yml
- filename: up-bank-openapi.json
  format: json
  label: Up Personal Banking API
  slug: up-personal-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/openapi/up-bank-openapi.json
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Up Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Up publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Up API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Up
provider_slug: up-bank
schemes:
- authorizationUrl: https://api.up.com.au/oidc/authorize
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  issuer: https://api.up.com.au
  name: CDR-OIDC
  openIdConnectUrl: https://api.up.com.au/.well-known/openid-configuration
  source: https://api.up.com.au/.well-known/openid-configuration
  tokenUrl: https://secure.api.up.com.au/oidc/token
  type: openIdConnect
scope_count: 10
scope_names:
- openid
- profile
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
- common:customer.basic:read
- common:customer.detail:read
- cdr:registration
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorization_code
  scope: openid
- description: Access to basic OpenID profile claims (name, given_name, etc.).
  flows:
  - authorization_code
  scope: profile
- description: CDR — read basic banking account data (masked account numbers, balances).
  flows:
  - authorization_code
  scope: bank:accounts.basic:read
- description: CDR — read detailed banking account data (full account numbers, features).
  flows:
  - authorization_code
  scope: bank:accounts.detail:read
- description: CDR — read banking transaction data.
  flows:
  - authorization_code
  scope: bank:transactions:read
- description: CDR — read saved payees.
  flows:
  - authorization_code
  scope: bank:payees:read
- description: CDR — read direct debits and scheduled/regular payments.
  flows:
  - authorization_code
  scope: bank:regular_payments:read
- description: CDR — read basic customer data (name, occupation / organisation basics).
  flows:
  - authorization_code
  scope: common:customer.basic:read
- description: CDR — read detailed customer data (contact details).
  flows:
  - authorization_code
  scope: common:customer.detail:read
- description: CDR dynamic client registration management.
  flows:
  - client_credentials
  scope: cdr:registration
slug: up-bank-scopes
source_filename: up-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.up.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ncontext: >-\n  These OAuth2 / OpenID Connect scopes are advertised by Up's Consumer Data\n  Right (CDR) OpenID Provider metadata at\n  https://api.up.com.au/.well-known/openid-configuration. They govern the CDR\n  data-sharing flow used by ACCREDITED DATA RECIPIENTS (not the personal\n  developer API, which uses a Personal Access Token). Access follows the CDR /\n  FAPI security profile: pushed authorization requests (required),\n  private_key_jwt client authentication, mTLS-bound access tokens, and the\n  authorization_code + client_credentials grants. The scope semantics are the\n  Australian CDR standard scopes defined by the Data Standards Body.\nschemes:\n  - name: CDR-OIDC\n    type: openIdConnect\n    openIdConnectUrl: https://api.up.com.au/.well-known/openid-configuration\n    issuer:\
  \ https://api.up.com.au\n    authorizationUrl: https://api.up.com.au/oidc/authorize\n    tokenUrl: https://secure.api.up.com.au/oidc/token\n    grant_types: [authorization_code, refresh_token, client_credentials]\n    source: https://api.up.com.au/.well-known/openid-configuration\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token.\n    flows: [authorization_code]\n  - scope: profile\n    description: Access to basic OpenID profile claims (name, given_name, etc.).\n    flows: [authorization_code]\n  - scope: bank:accounts.basic:read\n    description: CDR — read basic banking account data (masked account numbers, balances).\n    flows: [authorization_code]\n  - scope: bank:accounts.detail:read\n    description: CDR — read detailed banking account data (full account numbers, features).\n    flows: [authorization_code]\n  - scope: bank:transactions:read\n    description: CDR — read banking transaction data.\n    flows: [authorization_code]\n  - scope:\
  \ bank:payees:read\n    description: CDR — read saved payees.\n    flows: [authorization_code]\n  - scope: bank:regular_payments:read\n    description: CDR — read direct debits and scheduled/regular payments.\n    flows: [authorization_code]\n  - scope: common:customer.basic:read\n    description: CDR — read basic customer data (name, occupation / organisation basics).\n    flows: [authorization_code]\n  - scope: common:customer.detail:read\n    description: CDR — read detailed customer data (contact details).\n    flows: [authorization_code]\n  - scope: cdr:registration\n    description: CDR dynamic client registration management.\n    flows: [client_credentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/up-bank/refs/heads/main/scopes/up-bank-scopes.yml
summary_line: 10 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Neobank
- Product Reference Data
token_urls: []
---
