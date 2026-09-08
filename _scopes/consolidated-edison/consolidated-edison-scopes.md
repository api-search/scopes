---
api_specs:
- filename: consolidated-edison-green-button-connect-openapi.yml
  format: yaml
  label: Green Button Connect My Data
  slug: green-button-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-green-button-connect-openapi.yml
authorization_urls:
- https://www.coned.com/en/oauth/authorize
description: ''
docs: https://www.coned.com/en/accounts-billing/share-energy-usage-data/become-a-third-party
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Consolidated Edison Scopes
name_suffix: OAuth Scopes
note: Green Button Connect does not use free-text OAuth scope strings. Per NAESB ESPI, the scope parameter is a structured expression built from ESPI Functional Blocks (FB), interval/block durations, history length and a Business Resource (BR) id. The functional blocks below are the ones Con Edison publishes as available in its Third-Party Technical Onboarding Document v4.4; the scope_examples are Con Edison's own published values, copied verbatim.
overview: 'Consolidated Edison publishes 17 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Consolidated Edison API on a user''s behalf.


  Tokens are issued from https://api.coned.com/gbc/espi/1_1/oauth/Token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Consolidated Edison
provider_slug: consolidated-edison
schemes:
- flows:
  - authorizationUrl: https://www.coned.com/en/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token
  - flow: clientCredentials
    tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token
  name: GreenButtonOAuth2
  source: authentication/consolidated-edison-authentication.yml
scope_count: 17
scope_names:
- FB_01
- FB_03
- FB_04
- FB_05
- FB_07
- FB_08
- FB_10
- FB_15
- FB_16
- FB_35
- FB_51
- FB_53
- FB_56
- FB_57
- FB_58
- FB_60
- FB_67
scopes:
- description: Usage Data common
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_01
- description: Usage Data Connect My Data
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_03
- description: Interval Reading
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_04
- description: Electricity Interval Metering
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_05
- description: Net Electricity Metering
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_07
- description: Forward and Reverse Electricity Metering
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_08
- description: Natural Gas Interval Metering
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_10
- description: Usage Summary
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_15
- description: Usage Summary with cost
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_16
- description: Usage Data Bulk
  flows:
  - clientCredentials
  scope: FB_35
- description: Retail Customer Common
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_51
- description: Retail Customer Connect My Data
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_53
- description: Retail Customer Billing Information
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_56
- description: Retail Customer Account-Agreement Information
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_57
- description: Retail Customer Service-location Information
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_58
- description: Retail Customer Meter Information
  flows:
  - authorizationCode
  - clientCredentials
  scope: FB_60
- description: Retail Customer Bulk
  flows:
  - clientCredentials
  scope: FB_67
slug: consolidated-edison-scopes
source_filename: consolidated-edison-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://edge-e-dcxprod-web-bechbkdqagefb9ge.a03.azurefd.net/-/media/files/coned/documents/accountandbilling/share-my-data/onboarding-doc.pdf\ndocs: >-\n  https://www.coned.com/en/accounts-billing/share-energy-usage-data/become-a-third-party\nnote: >-\n  Green Button Connect does not use free-text OAuth scope strings. Per NAESB\n  ESPI, the scope parameter is a structured expression built from ESPI\n  Functional Blocks (FB), interval/block durations, history length and a\n  Business Resource (BR) id. The functional blocks below are the ones Con\n  Edison publishes as available in its Third-Party Technical Onboarding\n  Document v4.4; the scope_examples are Con Edison's own published values,\n  copied verbatim.\nscope_model:\n  parameter: scope\n  syntax: >-\n    FB=<functional block ids joined by _>;IntervalDuration=<...>;BlockDuration=<...>;HistoryLength=<seconds>;BR=<business resource id>\n  business_resource: '000092'\n\
  \  history_length_seconds: 63072000\n  history_length_note: Two years of history is the published maximum.\n  selection: >-\n    A third party may present the scope picker to the customer, or send a\n    predefined scope. The customer may remove (but not add) preselected scopes\n    on Con Edison's authorization page.\nschemes:\n  - name: GreenButtonOAuth2\n    source: authentication/consolidated-edison-authentication.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.coned.com/en/oauth/authorize\n        tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token\n      - flow: clientCredentials\n        tokenUrl: https://api.coned.com/gbc/espi/1_1/oauth/Token\nscopes:\n  - scope: FB_01\n    description: Usage Data common\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_03\n    description: Usage Data Connect My Data\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_04\n    description: Interval Reading\n    flows: [authorizationCode,\
  \ clientCredentials]\n  - scope: FB_05\n    description: Electricity Interval Metering\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_07\n    description: Net Electricity Metering\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_08\n    description: Forward and Reverse Electricity Metering\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_10\n    description: Natural Gas Interval Metering\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_15\n    description: Usage Summary\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_16\n    description: Usage Summary with cost\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_35\n    description: Usage Data Bulk\n    flows: [clientCredentials]\n  - scope: FB_51\n    description: Retail Customer Common\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_53\n    description: Retail Customer Connect My Data\n    flows: [authorizationCode,\
  \ clientCredentials]\n  - scope: FB_56\n    description: Retail Customer Billing Information\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_57\n    description: Retail Customer Account-Agreement Information\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_58\n    description: Retail Customer Service-location Information\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_60\n    description: Retail Customer Meter Information\n    flows: [authorizationCode, clientCredentials]\n  - scope: FB_67\n    description: Retail Customer Bulk\n    flows: [clientCredentials]\nmandatory_blocks:\n  - use_case: Consumption\n    required: [1, 3, 4]\n  - use_case: Billing\n    required: [1, 3]\n  - use_case: Retail Customer\n    required: [51, 53]\nscope_examples:\n  - name: Consumption Electricity Scope\n    value: FB=1_3_4_5;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n  - name: Consumption Electricity\
  \ Net Scope\n    value: FB=1_3_4_7;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n  - name: Consumption Gas Scope\n    value: FB=1_3_4_10;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n  - name: Consumption Forward Reverse Scope\n    value: FB=1_3_4_8;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n  - name: Billing Information Without Cost Scope\n    value: FB=1_3_15;IntervalDuration=Monthly;BlockDuration=Monthly;HistoryLength=63072000;BR=000092\n  - name: Billing Information With Cost Scope\n    value: FB=1_3_15_16;IntervalDuration=Monthly;BlockDuration=Monthly;HistoryLength=63072000;BR=000092\n  - name: Retail Customer Billing Account Scope\n    value: FB=51_53_56;BR=000092\n  - name: Retail Customer Meter Scope\n    value: FB=51_53_56_57_58_60;BR=000092\n  - name: Multiple Scopes combined\n    value: FB=1_3_4_5_7_8_10_15_16_51_53_56_57_58_60;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n\
  \  - name: Client Access Token bulk scope\n    value: FB=34_35\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/scopes/consolidated-edison-scopes.yml
summary_line: 17 scopes · authorizationCode/clientCredentials
tags:
- AMI
- Demand Response
- ESPI
- Energy
- Fortune 500
- Green Button
- Interval Data
- NAESB
- Natural Gas
- New York
- OAuth2
- Steam
- Utility
token_urls:
- https://api.coned.com/gbc/espi/1_1/oauth/Token
---
