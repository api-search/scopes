---
api_specs:
- filename: green-button-alliance-espi-openapi.json
  format: json
  label: PG&E Share My Data (Green Button Connect My Data) ESPI API
  slug: pge-share-my-data-espi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/green-button-alliance-espi-openapi.json
authorization_urls:
- https://sharemydata.pge.com/myAuthorization
- https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
description: PG&E Share My Data does not use named OAuth scope strings. Authorized scope is expressed as an ESPI (NAESB REQ.21) function-block scope string returned on the authorization-code response, the access-token response and the Authorization API, combining a numeric FB= list with a utility-defined AdditionalScope list and authorization parameters. Reproduced here from PG&E's published mapping.
docs: https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/Supported-Function-Block-Scope-String-Mapping-Click-Thru-2.0.pdf
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Pge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pacific Gas and Electric publishes 21 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pacific Gas and Electric API on a user''s behalf.


  Tokens are issued from https://api.pge.com/datacustodian/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pacific Gas and Electric
provider_slug: pge
schemes:
- flows:
  - authorizationUrl: https://sharemydata.pge.com/myAuthorization
    flow: authorizationCode
    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token
  - flow: clientCredentials
    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token
  name: OAuth2AuthorizationCode
  source: docs
- first_party: false
  flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  note: Green Button Alliance sandbox scheme, not a PG&E endpoint.
  source: openapi/green-button-alliance-espi-openapi.json
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
- description: Common services.
  flows: []
  scope: FB=1
- description: Core services.
  flows: []
  scope: FB=3
- description: Interval usage data.
  flows: []
  scope: FB=4
- description: Interval usage data for electric service agreements.
  flows: []
  scope: FB=5
- description: Delivered/Consumption and Received/Generation.
  flows: []
  scope: FB=8
- description: Gas data.
  flows: []
  scope: FB=10
- description: HTTPS support.
  flows: []
  scope: FB=13
- description: OAuth 2.0.
  flows: []
  scope: FB=14
- description: Usage summary information (billed total usage).
  flows: []
  scope: FB=15
- description: Usage summary with dollar bill cost.
  flows: []
  scope: FB=16
- description: Ability to authorize multiple service agreements.
  flows: []
  scope: FB=18
- description: IntervalBlocks without full data sets (without UsagePoints, MeterReading).
  flows: []
  scope: FB=19
- description: Third-party access to Subscription/Authorization.
  flows: []
  scope: FB=31
- description: Third-party access to UsagePoints, MeterReading and collections (excludes ElectricPowerQualitySummary).
  flows: []
  scope: FB=32
- description: Support REST request for Bulk.
  flows: []
  scope: FB=35
- description: published-max, published-min.
  flows: []
  scope: FB=37
- description: Request without prior notification.
  flows: []
  scope: FB=38
- description: Post Notification (of data being ready) followed by GET.
  flows: []
  scope: FB=39
- description: Authorization performed offline (manual paper CISR or Ops Portal).
  flows: []
  scope: FB=40
- description: Retrieve resources for a RetailCustomer.
  flows: []
  scope: FB=46
- description: Retrieve resources in Bulk for RetailCustomers via REST.
  flows: []
  scope: FB=47
slug: pge-scopes
source_filename: pge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/Supported-Function-Block-Scope-String-Mapping-Click-Thru-2.0.pdf\n  (HTTP 200, fetched and text-extracted 2026-07-27), corroborated against the\n  authorization examples printed on\n  https://www.pge.com/en/save-energy-and-money/energy-saving-programs/smartmeter/third-party-companies.html\n  (HTTP 200). Supersedes the derived pass over\n  openapi/green-button-alliance-espi-openapi.json, which declares zero scopes.\ndocs: https://www.pge.com/assets/pge/docs/save-energy-and-money/energy-savings-programs/Supported-Function-Block-Scope-String-Mapping-Click-Thru-2.0.pdf\ndescription: >-\n  PG&E Share My Data does not use named OAuth scope strings. Authorized scope is\n  expressed as an ESPI (NAESB REQ.21) function-block scope string returned on\n  the authorization-code response, the access-token response and the\n  Authorization API, combining\
  \ a numeric FB= list with a utility-defined\n  AdditionalScope list and authorization parameters. Reproduced here from PG&E's\n  published mapping.\nscope_string:\n  parameter: scope\n  format: >-\n    FB=<underscore-delimited function block numbers>;AdditionalScope=<underscore-delimited\n    selections>;IntervalDuration=<seconds>;BlockDuration=<period>;HistoryLength=<months>;AccountCollection=<count>;BR=<ThirdPartyID>;dataCustodianId=PGE\n  published_example: >-\n    scope=FB=1_3_8_13_14_18_19_31_32_35_37_38_39_40_4_5_10_15_16_46_47;AdditionalScope=Usage_Billing_Basic_Account_ProgramEnrollment;IntervalDuration=900_3600;BlockDuration=Daily;HistoryLength={3P\n    Registered historical length};AccountCollection={count of\n    authorizedSAs};BR={ThirdPartyID};dataCustodianId=PGE\n  returned_on:\n    - Authorization Code Request response (redirect to redirect_uri)\n    - Access Token Request response\n    - Authorization API resource\n  always_returned_function_blocks: [1, 3, 8, 13, 14, 18,\
  \ 19, 31, 32, 35, 37, 38, 39]\nschemes:\n  - name: OAuth2AuthorizationCode\n    source: docs\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sharemydata.pge.com/myAuthorization\n        tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token\n      - flow: clientCredentials\n        tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token\n  - name: oauth2\n    source: openapi/green-button-alliance-espi-openapi.json\n    first_party: false\n    note: Green Button Alliance sandbox scheme, not a PG&E endpoint.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n        tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n      - flow: clientCredentials\n        tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\nscopes:\n  - scope: FB=1\n    name: Common\n    description: Common services.\n    customer_selectable: false\n    always_returned:\
  \ true\n  - scope: FB=3\n    name: Green Button Connect My Data\n    description: Core services.\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=4\n    name: Interval Metering\n    description: Interval usage data.\n    customer_selectable: true\n    granted_when: Usage Info authorized for an electric or gas service agreement.\n  - scope: FB=5\n    name: Interval Electricity Metering\n    description: Interval usage data for electric service agreements.\n    customer_selectable: true\n    granted_when: Usage authorized for an electric service agreement.\n  - scope: FB=8\n    name: Forward and Reverse Metering\n    description: Delivered/Consumption and Received/Generation.\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=10\n    name: Gas data\n    description: Gas data.\n    customer_selectable: true\n    granted_when: Usage or Billing Info authorized for a gas service agreement.\n  - scope: FB=13\n    name: Security and Privacy classes\n\
  \    description: HTTPS support.\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=14\n    name: Authorization and Authentication (OAuth)\n    description: OAuth 2.0.\n    customer_selectable: true\n    always_returned: true\n  - scope: FB=15\n    name: Usage Summary\n    description: Usage summary information (billed total usage).\n    customer_selectable: true\n    granted_when: Usage or Billing Info authorized.\n  - scope: FB=16\n    name: Usage Summary with Cost\n    description: Usage summary with dollar bill cost.\n    customer_selectable: true\n    granted_when: Billing Info authorized.\n  - scope: FB=18\n    name: Multiple UsagePoints\n    description: Ability to authorize multiple service agreements.\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=19\n    name: Partial update data\n    description: IntervalBlocks without full data sets (without UsagePoints, MeterReading).\n    customer_selectable: false\n    always_returned: true\n\
  \  - scope: FB=31\n    name: Core REST Services\n    description: Third-party access to Subscription/Authorization.\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=32\n    name: Resource Level REST\n    description: >-\n      Third-party access to UsagePoints, MeterReading and collections (excludes\n      ElectricPowerQualitySummary).\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=35\n    name: REST for Bulk\n    description: Support REST request for Bulk.\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=37\n    name: Query Parameters\n    description: published-max, published-min.\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=38\n    name: On Demand Requests\n    description: Request without prior notification.\n    customer_selectable: false\n    always_returned: true\n  - scope: FB=39\n    name: Push model\n    description: Post Notification (of data being ready) followed by GET.\n\
  \    customer_selectable: false\n    always_returned: true\n  - scope: FB=40\n    name: Offline Authorization to complement OAuth\n    description: Authorization performed offline (manual paper CISR or Ops Portal).\n    customer_selectable: false\n    granted_when: Offline authorization created via the paper CISR form.\n  - scope: FB=46\n    name: Core RetailCustomer\n    description: Retrieve resources for a RetailCustomer.\n    customer_selectable: true\n    granted_when: Basic and/or Account Info and/or ProgramEnrollment Info authorized.\n  - scope: FB=47\n    name: REST for RetailCustomer Bulk\n    description: Retrieve resources in Bulk for RetailCustomers via REST.\n    customer_selectable: true\n    granted_when: Basic and/or Account Info and/or ProgramEnrollment Info authorized.\nadditional_scope:\n  parameter: AdditionalScope\n  format: Underscore-delimited list of customer-authorized selections.\n  values:\n    - value: Usage\n      description: Interval usage data for authorized\
  \ service agreements.\n    - value: Billing\n      description: Billing information including billed usage and cost.\n    - value: Basic\n      description: Basic customer information.\n    - value: Account\n      description: Account information.\n    - value: ProgramEnrollment\n      description: Demand response and other program enrollment information.\nauthorization_parameters:\n  - parameter: IntervalDuration\n    description: Authorized interval durations in seconds (published example 900_3600).\n  - parameter: BlockDuration\n    description: Block duration of returned data (published example Daily).\n  - parameter: HistoryLength\n    description: Third-party registered historical length.\n  - parameter: AccountCollection\n    description: Count of authorized service agreements.\n  - parameter: BR\n    description: Third-party identifier.\n  - parameter: dataCustodianId\n    description: Always PGE for Share My Data.\nnotes: >-\n  The mapping document also publishes worked example\
  \ scope strings per service\n  agreement type (Electric, Gas, Electric + Gas) for each combination of\n  authorized data groups; those rules are captured above under granted_when\n  rather than duplicated. FB numbers are ESPI-standard function blocks, so this\n  scope model is portable across Green Button Connect My Data data custodians.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/scopes/pge-scopes.yml
summary_line: 21 scopes · authorizationCode/clientCredentials
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- California
- Smart Metering
- Green Button
- ESPI
- Energy Data
- Grid
- Demand Response
- Investor-Owned Utility
token_urls:
- https://api.pge.com/datacustodian/oauth/v2/token
- https://sandbox.greenbuttonalliance.org:8443/oauth/token
---
