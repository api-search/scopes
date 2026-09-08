---
api_specs:
- filename: citizens-financial-group-accounts-openapi.yml
  format: yaml
  label: Citizens Accounts API
  slug: citizens-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-accounts-openapi.yml
- filename: citizens-financial-group-statements-openapi.yml
  format: yaml
  label: Citizens Statements API
  slug: citizens-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-statements-openapi.yml
- filename: citizens-financial-group-payments-openapi.yml
  format: yaml
  label: Citizens Payments API
  slug: citizens-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-payments-openapi.yml
- filename: citizens-financial-group-account-validation-openapi.yml
  format: yaml
  label: Citizens Account Validation API
  slug: citizens-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-account-validation-openapi.yml
- filename: citizens-financial-group-account-transfer-openapi.yml
  format: yaml
  label: Citizens Account Transfer API
  slug: citizens-account-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-account-transfer-openapi.yml
- filename: citizens-financial-group-information-reporting-openapi.yml
  format: yaml
  label: Citizens Information Reporting API
  slug: citizens-information-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-information-reporting-openapi.yml
- filename: citizens-financial-group-authorize-openapi.yml
  format: yaml
  label: Citizens Authorize API
  slug: citizens-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-authorize-openapi.yml
- filename: citizens-financial-group-atm-locator-openapi.yml
  format: yaml
  label: Citizens ATM Locator API
  slug: citizens-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-atm-locator-openapi.yml
- filename: citizens-financial-group-branch-locator-openapi.yml
  format: yaml
  label: Citizens Branch Locator API
  slug: citizens-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-branch-locator-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.citizensbank.com/content/qut/CitizensPaymentAPIUserGuide.pdf
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Citizens Financial Group Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Citizens Financial Group publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Citizens Financial Group API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Citizens Financial Group
provider_slug: citizens-financial-group
schemes: []
scope_count: 5
scope_names:
- ir:read
- av:read
- transfer:initiate
- Payment:Initiate
- Payment:Query
scopes:
- description: Access to read Information Reporting data (account list, balances, transactions).
  flows:
  - clientCredentials
  scope: ir:read
- description: Access to read Account Validation data.
  flows:
  - clientCredentials
  scope: av:read
- description: Access to initiate an internal account transfer.
  flows:
  - clientCredentials
  scope: transfer:initiate
- description: Submit an RTP or ACH payment instruction.
  flows:
  - clientCredentials
  scope: Payment:Initiate
- description: Retrieve participant status and payment status.
  flows:
  - clientCredentials
  scope: Payment:Query
slug: citizens-financial-group-scopes
source_filename: citizens-financial-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  Scope strings read from the harvested OpenAPI securitySchemes in openapi/ and from the sample token\n  requests published in the Citizens API user guides (Payments v1.3, Account Transfer v1.0, Account\n  Validation v1.6, Information Reporting v1.6).\ndocs: https://developer.citizensbank.com/content/qut/CitizensPaymentAPIUserGuide.pdf\nprovider: Citizens Financial Group\nproviderId: citizens-financial-group\n\nauthorization:\n  flow: clientCredentials\n  grant_type: client_credentials\n  client_authentication: private_key_jwt over mTLS\n  token_endpoint_production: https://apis.citizensbank.com/as/token.oauth2\n  token_endpoint_sandbox: https://sandboxapis.citizensbank.com/as/token.oauth2\n  note: >-\n    Scopes are requested as a space-delimited `scope` form parameter on the token request. Citizens\n    does not publish a consolidated scope reference page; the list below is the union of every scope\n    string that appears\
  \ in a published contract or a published sample request.\n\nscopes:\n  - scope: ir:read\n    description: Access to read Information Reporting data (account list, balances, transactions).\n    flows: [clientCredentials]\n    evidence:\n      - openapi/citizens-financial-group-information-reporting-openapi.yml\n      - openapi/citizens-financial-group-payments-openapi.yml\n      - https://developer.citizensbank.com/content/qut/CitizensInformationReportingAPIUserGuide.pdf\n  - scope: av:read\n    description: Access to read Account Validation data.\n    flows: [clientCredentials]\n    evidence:\n      - openapi/citizens-financial-group-account-validation-openapi.yml\n      - https://developer.citizensbank.com/content/qut/CitizensAccountValidationAPIUserGuide.pdf\n  - scope: 'transfer:initiate'\n    description: Access to initiate an internal account transfer.\n    flows: [clientCredentials]\n    evidence:\n      - openapi/citizens-financial-group-account-transfer-openapi.yml\n  - scope:\
  \ 'Payment:Initiate'\n    description: Submit an RTP or ACH payment instruction.\n    flows: [clientCredentials]\n    evidence:\n      - https://developer.citizensbank.com/content/qut/CitizensPaymentAPIUserGuide.pdf\n    note: >-\n      Published only in the user guide's sample token request\n      (--data 'scope=Payment:Initiate Payment:Query'); the Payments OpenAPI declares ir:read instead,\n      which looks like a copy-paste carry-over from Information Reporting.\n  - scope: 'Payment:Query'\n    description: Retrieve participant status and payment status.\n    flows: [clientCredentials]\n    evidence:\n      - https://developer.citizensbank.com/content/qut/CitizensPaymentAPIUserGuide.pdf\n\ngaps:\n  - >-\n    The Payments OpenAPI's oauth2 scope map disagrees with the Payments user guide sample request\n    (ir:read vs Payment:Initiate / Payment:Query). Recorded as published; not reconciled.\n  - >-\n    No scope reference page exists on developer.citizensbank.com. Scopes for the FDX\
  \ Accounts /\n    Statements surface and for Authorize are not published - those contracts declare header key\n    schemes only.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/scopes/citizens-financial-group-scopes.yml
summary_line: 5 scopes
tags:
- Banking
- Buy Now Pay Later
- Financial-Services
- FDX
- Locator
- Open Banking
- Payments
token_urls: []
---
