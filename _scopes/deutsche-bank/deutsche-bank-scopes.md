---
api_specs:
- filename: deutsche-bank-dbapi-addresses-v2.json
  format: json
  label: Deutsche Bank API Program
  slug: deutsche-bank
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-bank/refs/heads/main/openapi/deutsche-bank-dbapi-addresses-v2.json
- filename: deutsche-bank-merchant-solution-callback-v2.json
  format: json
  label: Deutsche Bank Merchant Solutions
  slug: merchant-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deutsche-bank/refs/heads/main/openapi/deutsche-bank-merchant-solution-callback-v2.json
authorization_urls: []
description: The published Deutsche Bank dbAPI OAuth 2.0 scope reference, harvested verbatim from the scope metadata document the developer portal itself renders on its Available Scopes page. 42 scopes across 8 functional groups. Scopes are requested against the dbAPI OIDC provider (issuer https://simulator-api.db.com/gw/oidc/ in simulation, https://api.db.com in production) using the authorization code, authorization code with PKCE, client credentials or refresh token grant, depending on the API.
docs: https://developer.db.com/apidocumentation/oauthflows/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Deutsche Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Deutsche Bank uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deutsche Bank
provider_slug: deutsche-bank
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: deutsche-bank-scopes
source_filename: deutsche-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Deutsche Bank\nproviderId: deutsche-bank\ngenerated: '2026-09-06'\nmethod: searched\nsource: https://ams-prd.developer.db.com/c2/scopes-metadata.model.json\ndocs: https://developer.db.com/apidocumentation/oauthflows/scopes\nverbatim: scopes/deutsche-bank-scopes-metadata.json\ndescription: >-\n  The published Deutsche Bank dbAPI OAuth 2.0 scope reference, harvested verbatim from the\n  scope metadata document the developer portal itself renders on its Available Scopes page.\n  42 scopes across 8 functional groups. Scopes are requested against the dbAPI OIDC provider\n  (issuer https://simulator-api.db.com/gw/oidc/ in simulation, https://api.db.com in production)\n  using the authorization code, authorization code with PKCE, client credentials or refresh\n  token grant, depending on the API.\ntoken_endpoint: https://simulator-api.db.com/gw/oidc/oauth2/token\nauthorization_endpoint: https://simulator-api.db.com/gw/oidc/oauth2/authorize\n\
  scope_count: 42\nscopes:\n  - name: read_accounts\n    group: banking\n    description: \"Grants read access to all basic cash account data like the current balance and a general account overview for the given customer\"\n  - name: read_accounts_list\n    group: banking\n    description: \"Grants read access to basic cash account data and a general account overview for the given customer\"\n  - name: read_transactions\n    group: banking\n    description: \"Grants read access to transactions for cash accounts (current and deposit) for the given customer. The API provides in default up to 13 months of transaction history\"\n  - name: rent_analysis\n    group: banking\n    description: \"Check rent payments\"\n  - name: income_analysis\n    group: banking\n    description: \"Check income payments\"\n  - name: open_cash_account\n    group: banking\n    description: \"Cash account openings\"\n  - name: open_escrow_account\n    group: banking\n    description: \"Escrow account openings\"\n\
  \  - name: read_credit_cards_list_with_details\n    group: credit_cards\n    description: \"Grants read access to credit card data\"\n  - name: read_credit_card_transactions\n    group: credit_cards\n    description: \"Read your credit card transaction data\"\n  - name: offline_access\n    group: default\n    description: \"Request an OAuth2 Refresh Token\"\n  - name: openid\n    group: default\n    description: \"Request access to OpenId Connect functionality\"\n  - name: investments_report\n    group: investment_portfolio\n    description: \"Generate investments report for the given customer\"\n  - name: read_assets\n    group: investment_portfolio\n    description: \"Grants read access to asset summary of a portfolio group.\"\n  - name: read_performances\n    group: investment_portfolio\n    description: \"Grants read access to performance overview of a portfolio.\"\n  - name: read_security_accounts_list\n    group: investment_portfolio\n    description: \"Grants read access to security\
  \ account data\"\n  - name: read_security_transactions\n    group: investment_portfolio\n    description: \"Grants read access to all security transactions for the given customer\"\n  - name: order_securities\n    group: investment_portfolio\n    description: \"Order securities\"\n  - name: open_esp_securities_account\n    group: investment_portfolio\n    description: \"Open ESP securities accounts\"\n  - name: request_private_loans\n    group: lending\n    description: \"Request private loans\"\n  - name: request_loans\n    group: lending\n    description: \"Request loans\"\n  - name: transaction_notifications\n    group: notification\n    description: \"Enable the transaction subscription feature\"\n  - name: investments_orders_status_notification\n    group: notification\n    description: \"Enable the investments orders subscription feature\"\n  - name: instant_sepa_credit_transfers\n    group: payments\n    description: \"Initiate and check status of instant SEPA credit transfers\"\
  \n  - name: sepa_credit_transfers\n    group: payments\n    description: \"Initiate and check status of SEPA Credit Transfers\"\n  - name: sepa_direct_debit_core\n    group: payments\n    description: \"Initiate and check status of SEPA Direct Debit Core\"\n  - name: bulk_instant_sepa_credit_transfers\n    group: payments\n    description: \"Initiate and check status of bulk SEPA instant credit transfers\"\n  - name: sepa_direct_debit_B2B\n    group: payments\n    description: \"Initiate and check status of SEPA Direct Debit B2B\"\n  - name: bulk_sepa_credit_transfers\n    group: payments\n    description: \"Bulk SEPA Credit Transfers with status check\"\n  - name: read_ownership_information\n    group: reference_data\n    description: \"Information about ultimate beneficiary owners\"\n  - name: read_additional_organization_data\n    group: reference_data\n    description: \"Grants read access to additional organizational information about a partner representing a company. The additional\
  \ data contains legal form, industry, local court, stakeholders and tax identification.\"\n  - name: verify_account_ownership\n    group: reference_data\n    description: \"Performs account verification for the given customer.\"\n  - name: read_partners_legi\n    group: reference_data\n    description: \"Grants read access to legitimation data of the current partner/customer. This data is only available for natural persons. Legitimation data contains information, e.g. about the document type, document number and document issue date for the given customer.\"\n  - name: read_check_information\n    group: reference_data\n    description: \"Know-Your-Customer Information\"\n  - name: read_legal_representatives_data\n    group: reference_data\n    description: \"Information about legal representatives\"\n  - name: read_customer_data\n    group: reference_data\n    description: \"Performs personal data verification for the given customer.\"\n  - name: read_partners\n    group: reference_data\n\
  \    description: \"Grants read access to basic data of the current partner/customer. The basic partner data contains, among other information, the first name, the surname and the birthdate for the given customer. There is some overlap between our /partners endpoint and the /userinfo endpoint provided by OpenID connect.\"\n  - name: read_additional_personal_data\n    group: reference_data\n    description: \"Grants read access to additional data about the partner. The additional data currently contains the tax identifications for the given customer.\"\n  - name: read_addresses\n    group: reference_data\n    description: \"Grants read access to address data for the given customer. Two address types are currently supported: business address and private address.\"\n  - name: age_certificate\n    group: reference_data\n    description: \"Grants a check of a person's age, when compared against a specific minimum age\"\n  - name: reserve_branch_customer_number\n    group: reference_data\n \
  \   description: \"Reserve Branch Customer Number\"\n  - name: read_brand\n    group: reference_data\n    description: \"Grants permission to get data from the /brand endpoint. Only available with client credential grant flow right now.\"\n  - name: create_processing_orders\n    group: uncategorized_scopes\n    description: \"Grants permission to post data with the /processingOrders endpoint. Only available with client credential grant flow right now.\"\ngroups: [{\"id\": \"banking\", \"name\": \"Banking\"}, {\"id\": \"credit_cards\", \"name\": \"Credit Cards\"}, {\"id\": \"default\", \"name\": \"Default\"}, {\"id\": \"investment_portfolio\", \"name\": \"Investment Portfolio\"}, {\"id\": \"lending\", \"name\": \"Lending\"}, {\"id\": \"notification\", \"name\": \"Notification\"}, {\"id\": \"payments\", \"name\": \"Payments\"}, {\"id\": \"reference_data\", \"name\": \"Reference Data\"}, {\"id\": \"uncategorized_scopes\", \"name\": \"Uncategorized Scopes\", \"default\": true}]\nmaintainers:\n\
  \  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-bank/refs/heads/main/scopes/deutsche-bank-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Banking
- Financial
- Wealth Management
- Open Banking
- PSD2
- Payments
- SEPA
- Investments
- Credit Cards
- Merchant Solutions
- Germany
- Financial Services
token_urls: []
---
