---
api_specs:
- filename: pg-and-e-authorization-api-openapi.yml
  format: yaml
  label: pg-and-e Authorization API
  slug: pg-and-e-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-authorization-api-openapi.yml
- filename: pg-and-e-subscriptions-api-openapi.yml
  format: yaml
  label: pg-and-e Subscriptions API
  slug: pg-and-e-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-subscriptions-api-openapi.yml
- filename: pg-and-e-usage-api-openapi.yml
  format: yaml
  label: pg-and-e Usage API
  slug: pg-and-e-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/openapi/pg-and-e-usage-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html
flows:
- authorization_code
- client_credentials
- refresh_token
kind: oauth-scopes
layout: scope
method: searched
name: Pg And E Scopes
name_suffix: OAuth Scopes
note: Supersedes the 2026-07-11 derived artifact, which recorded a single scope "usage:read" read out of the in-repo OpenAPI scaffold. PG&E does not use bare string scopes. Share My Data implements the NAESB ESPI authorization profile, in which the granted scope is returned as a single compound FUNCTION-BLOCK STRING. The function-block numbers and their meanings below are transcribed from PG&E's own published "Supported Function Block Scope String Mapping (Click-Thru 2.0)" PDF (HTTP 200, fetched 2026-09-17). An agent must parse the FB= list, not look for OAuth scope names.
overview: 'Pg And E publishes 21 OAuth 2.0 scopes via the authorization_code, client_credentials, and refresh_token flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pg And E API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pg And E
provider_slug: pg-and-e
schemes:
- authorizationUrl: https://api.pge.com/datacustodian/oauth/v2/Authorize
  flows:
  - authorization_code
  - client_credentials
  - refresh_token
  name: oauth2
  testAuthorizationUrl: https://api.pge.com/datacustodian/test/oauth/v2/authorize
  testTokenUrl: https://api.pge.com/datacustodian/test/oauth/v2/token
  tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token
  type: oauth2
scope_count: 21
scope_names:
- FB=1
- FB=3
- FB=4
- FB=5
- FB=8
- FB=10
- FB=13
- FB=14
- FB=15
- FB=16
- FB=18
- FB=19
- FB=31
- FB=32
- FB=35
- FB=37
- FB=38
- FB=39
- FB=40
- FB=46
- FB=47
scopes:
- description: Common services. Always returned; not customer-selectable.
  flows: []
  scope: FB=1
- description: Core services. Always returned; not customer-selectable.
  flows: []
  scope: FB=3
- description: Interval usage data. Granted by the customer selecting Usage Info (electric or gas SAs).
  flows: []
  scope: FB=4
- description: Interval electricity usage. Granted by the customer selecting Usage Info for electric SAs.
  flows: []
  scope: FB=5
- description: Delivered/consumption and received/generation. Always returned.
  flows: []
  scope: FB=8
- description: Gas data. Granted by the customer selecting Usage or Bill Info for gas SAs.
  flows: []
  scope: FB=10
- description: HTTPS support. Always returned.
  flows: []
  scope: FB=13
- description: OAuth 2.0. Always returned.
  flows: []
  scope: FB=14
- description: Billed total usage summary. Granted by Usage or Bill Info.
  flows: []
  scope: FB=15
- description: Usage summary including dollar bill cost. Granted by Bill Info.
  flows: []
  scope: FB=16
- description: Ability to authorize multiple service agreements. Always returned.
  flows: []
  scope: FB=18
- description: IntervalBlocks without full data sets (no UsagePoint/MeterReading). Always returned.
  flows: []
  scope: FB=19
- description: Third-party access to Subscription/Authorization. Always returned.
  flows: []
  scope: FB=31
- description: Third-party access to UsagePoints, MeterReading and collections (excludes ElectricPowerQualitySummary). Always returned.
  flows: []
  scope: FB=32
- description: Supports REST requests for Bulk. Always returned.
  flows: []
  scope: FB=35
- description: published-max / published-min query parameters. Always returned.
  flows: []
  scope: FB=37
- description: Request without prior notification. Always returned.
  flows: []
  scope: FB=38
- description: POST notification that data is ready, followed by a GET from the third party. Always returned. This is the webhook surface.
  flows: []
  scope: FB=39
- description: Authorization performed offline (paper CISR or Ops Portal). Always returned.
  flows: []
  scope: FB=40
- description: Retrieve resources for a RetailCustomer. Granted by Basic and/or Account Info and/or Program Enrollment Info.
  flows: []
  scope: FB=46
- description: Retrieve resources in bulk for a RetailCustomer. Granted by Basic and/or Account Info.
  flows: []
  scope: FB=47
slug: pg-and-e-scopes
source_filename: pg-and-e-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: pg-and-e\nproviderId: pg-and-e\ngenerated: '2026-09-17'\nmethod: searched\nsource: https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/Supported-Function-Block-Scope-String-Mapping-Click-Thru-2.0.pdf\ndocs: https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html\nmodified: '2026-09-17'\nnote: >-\n  Supersedes the 2026-07-11 derived artifact, which recorded a single scope \"usage:read\" read out of\n  the in-repo OpenAPI scaffold. PG&E does not use bare string scopes. Share My Data implements the\n  NAESB ESPI authorization profile, in which the granted scope is returned as a single compound\n  FUNCTION-BLOCK STRING. The function-block numbers and their meanings below are transcribed from\n  PG&E's own published \"Supported Function Block Scope String Mapping (Click-Thru 2.0)\" PDF\n  (HTTP 200, fetched 2026-09-17). An\
  \ agent must parse the FB= list, not look for OAuth scope names.\nschemes:\n  - name: oauth2\n    type: oauth2\n    authorizationUrl: https://api.pge.com/datacustodian/oauth/v2/Authorize\n    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token\n    testAuthorizationUrl: https://api.pge.com/datacustodian/test/oauth/v2/authorize\n    testTokenUrl: https://api.pge.com/datacustodian/test/oauth/v2/token\n    flows:\n      - authorization_code\n      - client_credentials\n      - refresh_token\nscope_format:\n  style: espi-function-block-string\n  example: >-\n    FB=1_3_8_13_14_18_19_31_32_35_37_38_39_40_4_5_10_15_16_46_47;AdditionalScope=Usage_Billing_Basic_Account_ProgramEnrollment;IntervalDuration=900_3600;BlockDuration=Daily;HistoryLength={3P Registered historical length};AccountCollection={count of authorized SAs};BR={ThirdPartyID};dataCustodianId=PGE\n  example_source: >-\n    https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/Supported-Function-Block-Scope-String-Mapping-Click-Thru-2.0.pdf\n\
  \  returned_in:\n    - authorization code response\n    - access token response\n    - GET /GreenButtonConnect/espi/1_1/resource/Authorization\n  parameters:\n    - name: FB\n      description: Underscore-separated list of granted ESPI Green Button function-block numbers.\n    - name: AdditionalScope\n      description: >-\n        Utility-defined authorization selections, e.g.\n        Usage_Billing_Basic_Account_ProgramEnrollment.\n    - name: IntervalDuration\n      description: Granted interval granularity in seconds, e.g. 900_3600 (15-minute and hourly).\n    - name: BlockDuration\n      description: Interval-block grouping, e.g. Daily.\n    - name: HistoryLength\n      description: Historical depth the third party registered for.\n    - name: AccountCollection\n      description: Count of service agreements the customer authorized.\n    - name: BR\n      description: The third-party identifier.\n    - name: dataCustodianId\n      description: Always PGE for this data custodian.\n\
  scope_count: 21\nscopes:\n  - scope: FB=1\n    name: Common\n    description: Common services. Always returned; not customer-selectable.\n    customer_selectable: false\n  - scope: FB=3\n    name: Green Button Connect My Data\n    description: Core services. Always returned; not customer-selectable.\n    customer_selectable: false\n  - scope: FB=4\n    name: Interval Metering\n    description: Interval usage data. Granted by the customer selecting Usage Info (electric or gas SAs).\n    customer_selectable: true\n  - scope: FB=5\n    name: Interval Electricity Metering\n    description: Interval electricity usage. Granted by the customer selecting Usage Info for electric SAs.\n    customer_selectable: true\n  - scope: FB=8\n    name: Forward and Reverse Metering\n    description: Delivered/consumption and received/generation. Always returned.\n    customer_selectable: false\n  - scope: FB=10\n    name: Gas data\n    description: Gas data. Granted by the customer selecting Usage or Bill\
  \ Info for gas SAs.\n    customer_selectable: true\n  - scope: FB=13\n    name: Security and Privacy classes\n    description: HTTPS support. Always returned.\n    customer_selectable: false\n  - scope: FB=14\n    name: Authorization and Authentication (OAuth)\n    description: OAuth 2.0. Always returned.\n    customer_selectable: false\n  - scope: FB=15\n    name: Usage Summary\n    description: Billed total usage summary. Granted by Usage or Bill Info.\n    customer_selectable: true\n  - scope: FB=16\n    name: Usage Summary with Cost\n    description: Usage summary including dollar bill cost. Granted by Bill Info.\n    customer_selectable: true\n  - scope: FB=18\n    name: Multiple UsagePoints\n    description: Ability to authorize multiple service agreements. Always returned.\n    customer_selectable: false\n  - scope: FB=19\n    name: Partial update data\n    description: IntervalBlocks without full data sets (no UsagePoint/MeterReading). Always returned.\n    customer_selectable:\
  \ false\n  - scope: FB=31\n    name: Core REST Services\n    description: Third-party access to Subscription/Authorization. Always returned.\n    customer_selectable: false\n  - scope: FB=32\n    name: Resource Level REST\n    description: >-\n      Third-party access to UsagePoints, MeterReading and collections\n      (excludes ElectricPowerQualitySummary). Always returned.\n    customer_selectable: false\n  - scope: FB=35\n    name: REST for Bulk\n    description: Supports REST requests for Bulk. Always returned.\n    customer_selectable: false\n  - scope: FB=37\n    name: Query Parameters\n    description: published-max / published-min query parameters. Always returned.\n    customer_selectable: false\n  - scope: FB=38\n    name: On Demand Requests\n    description: Request without prior notification. Always returned.\n    customer_selectable: false\n  - scope: FB=39\n    name: Push model\n    description: >-\n      POST notification that data is ready, followed by a GET from the third\
  \ party.\n      Always returned. This is the webhook surface.\n    customer_selectable: false\n  - scope: FB=40\n    name: Offline Authorization to complement OAuth\n    description: Authorization performed offline (paper CISR or Ops Portal). Always returned.\n    customer_selectable: false\n  - scope: FB=46\n    name: Core RetailCustomer\n    description: >-\n      Retrieve resources for a RetailCustomer. Granted by Basic and/or Account Info and/or\n      Program Enrollment Info.\n    customer_selectable: true\n  - scope: FB=47\n    name: REST for RetailCustomer Bulk\n    description: >-\n      Retrieve resources in bulk for a RetailCustomer. Granted by Basic and/or Account Info.\n    customer_selectable: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/scopes/pg-and-e-scopes.yml
summary_line: 21 scopes · authorization_code/client_credentials/refresh_token
tags:
- Energy
- Utilities
- Electricity
- Natural Gas
- California
- United States
- Smart Metering
- Green Button
- ESPI
- Energy Usage Data
- Investor-Owned Utility
- Customer Data Access
token_urls: []
---
