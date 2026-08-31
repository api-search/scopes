---
api_specs:
- filename: con-edison-applicationinformation-api-openapi.yml
  format: yaml
  label: Con Edison Application Information API
  slug: con-edison-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-applicationinformation-api-openapi.yml
- filename: con-edison-authorization-api-openapi.yml
  format: yaml
  label: Con Edison Authorization API
  slug: con-edison-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-authorization-api-openapi.yml
- filename: con-edison-batch-api-openapi.yml
  format: yaml
  label: Con Edison Batch API
  slug: con-edison-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-batch-api-openapi.yml
- filename: con-edison-electricpowerusagesummary-api-openapi.yml
  format: yaml
  label: Con Edison Electric Power Usage Summary API
  slug: con-edison-electricpowerusagesummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-electricpowerusagesummary-api-openapi.yml
- filename: con-edison-intervalblock-api-openapi.yml
  format: yaml
  label: Con Edison Interval Block API
  slug: con-edison-intervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-intervalblock-api-openapi.yml
- filename: con-edison-localtimeparameters-api-openapi.yml
  format: yaml
  label: Con Edison Local Time Parameters API
  slug: con-edison-localtimeparameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-localtimeparameters-api-openapi.yml
- filename: con-edison-meterreading-api-openapi.yml
  format: yaml
  label: Con Edison Meter Reading API
  slug: con-edison-meterreading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-meterreading-api-openapi.yml
- filename: con-edison-readingtype-api-openapi.yml
  format: yaml
  label: Con Edison Reading Type API
  slug: con-edison-readingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-readingtype-api-openapi.yml
- filename: con-edison-realtimebatch-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Batch API
  slug: con-edison-realtimebatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimebatch-api-openapi.yml
- filename: con-edison-realtimeintervalblock-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Interval Block API
  slug: con-edison-realtimeintervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimeintervalblock-api-openapi.yml
- filename: con-edison-realtimereadingtype-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Reading Type API
  slug: con-edison-realtimereadingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimereadingtype-api-openapi.yml
- filename: con-edison-retailcustomer-api-openapi.yml
  format: yaml
  label: Con Edison Retail Customer API
  slug: con-edison-retailcustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-retailcustomer-api-openapi.yml
- filename: con-edison-servicestatus-api-openapi.yml
  format: yaml
  label: Con Edison Service Status API
  slug: con-edison-servicestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-servicestatus-api-openapi.yml
- filename: con-edison-usagepoint-api-openapi.yml
  format: yaml
  label: Con Edison Usage Point API
  slug: con-edison-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-usagepoint-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.coned.com/en/accounts-billing/share-energy-usage-data/become-a-third-party
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Con Edison Scopes
name_suffix: OAuth Scopes
note: 'Con Edison''s Swagger 2.0 definition declares no securityDefinitions, so derive-oauth-scopes.py produced nothing. The scope model below is transcribed from section 3.2.3 "Functional Blocks and its description" of the Third-Party Technical Onboarding Document v4.4 (last updated 2026-05-07). Scopes are NAESB REQ.21 ESPI functional blocks (FB), not free-form strings: a single scope value is a semicolon-delimited string carrying the FB list plus interval/history qualifiers.'
overview: 'Con Edison publishes 17 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Con Edison API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Con Edison
provider_slug: con-edison
schemes: []
scope_count: 17
scope_names:
- FB=1
- FB=3
- FB=4
- FB=5
- FB=7
- FB=8
- FB=10
- FB=15
- FB=16
- FB=35
- FB=51
- FB=53
- FB=56
- FB=57
- FB=58
- FB=60
- FB=67
scopes:
- description: ''
  flows: []
  scope: FB=1
- description: ''
  flows: []
  scope: FB=3
- description: ''
  flows: []
  scope: FB=4
- description: ''
  flows: []
  scope: FB=5
- description: ''
  flows: []
  scope: FB=7
- description: ''
  flows: []
  scope: FB=8
- description: ''
  flows: []
  scope: FB=10
- description: ''
  flows: []
  scope: FB=15
- description: ''
  flows: []
  scope: FB=16
- description: ''
  flows: []
  scope: FB=35
- description: ''
  flows: []
  scope: FB=51
- description: ''
  flows: []
  scope: FB=53
- description: ''
  flows: []
  scope: FB=56
- description: ''
  flows: []
  scope: FB=57
- description: ''
  flows: []
  scope: FB=58
- description: ''
  flows: []
  scope: FB=60
- description: ''
  flows: []
  scope: FB=67
slug: con-edison-scopes
source_filename: con-edison-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://www.coned.com/-/media/files/coned/documents/accountandbilling/share-my-data/onboarding-doc.pdf\ndocs: https://www.coned.com/en/accounts-billing/share-energy-usage-data/become-a-third-party\nnote: >-\n  Con Edison's Swagger 2.0 definition declares no securityDefinitions, so derive-oauth-scopes.py\n  produced nothing. The scope model below is transcribed from section 3.2.3 \"Functional Blocks and its\n  description\" of the Third-Party Technical Onboarding Document v4.4 (last updated 2026-05-07).\n  Scopes are NAESB REQ.21 ESPI functional blocks (FB), not free-form strings: a single scope value is\n  a semicolon-delimited string carrying the FB list plus interval/history qualifiers.\nmodel:\n  style: espi-functional-blocks\n  format: FB=<block>_<block>...;IntervalDuration=<...>;BlockDuration=<...>;HistoryLength=<seconds>;BR=<ApplicationInformationId>\n  qualifiers:\n  - name: IntervalDuration\n    example: Monthly_3600_900_300\n\
  \    description: Interval lengths in seconds the third party may request (3600 hourly, 900 fifteen-minute, 300 five-minute) plus Monthly\n  - name: BlockDuration\n    example: Monthly_Daily\n    description: Aggregation block sizes returned\n  - name: HistoryLength\n    example: '63072000'\n    description: Maximum history in seconds — 63,072,000 seconds is the documented two-year cap\n  - name: BR\n    example: '000092'\n    description: Bulk Resource id — same value as the ApplicationInformation ID, obtained from the Get All Third-Party Applications endpoint\n  customer_control: >-\n    The customer sees the requested scopes on the Con Edison / Orange & Rockland authorization screen\n    and may remove scopes (removal only, no addition) before accepting.\nscopes:\n- scope: FB=1\n  name: Usage Data common\n  block: 1\n  mandatory_for: [consumption, billing]\n- scope: FB=3\n  name: Usage Data Connect My Data\n  block: 3\n  mandatory_for: [consumption, billing]\n- scope: FB=4\n  name:\
  \ Interval Reading\n  block: 4\n  mandatory_for: [consumption]\n- scope: FB=5\n  name: Electricity Interval Metering\n  block: 5\n- scope: FB=7\n  name: Net Electricity Metering\n  block: 7\n- scope: FB=8\n  name: Forward and Reverse Electricity Metering\n  block: 8\n- scope: FB=10\n  name: Natural Gas Interval Metering\n  block: 10\n- scope: FB=15\n  name: Usage Summary\n  block: 15\n- scope: FB=16\n  name: Usage Summary with cost\n  block: 16\n- scope: FB=35\n  name: Usage Data Bulk\n  block: 35\n- scope: FB=51\n  name: Retail Customer Common\n  block: 51\n  mandatory_for: [retail-customer]\n- scope: FB=53\n  name: Retail Customer Connect My Data\n  block: 53\n  mandatory_for: [retail-customer]\n- scope: FB=56\n  name: Retail Customer Billing Information\n  block: 56\n- scope: FB=57\n  name: Retail Customer Account-Agreement Information\n  block: 57\n- scope: FB=58\n  name: Retail Customer Service-location Information\n  block: 58\n- scope: FB=60\n  name: Retail Customer Meter Information\n\
  \  block: 60\n- scope: FB=67\n  name: Retail Customer Bulk\n  block: 67\nmandatory_minimums:\n- use_case: Consumption\n  blocks: [1, 3, 4]\n- use_case: Billing\n  blocks: [1, 3]\n- use_case: Retail Customer\n  blocks: [51, 53]\npublished_scope_examples:\n- name: Consumption Electricity Scope\n  value: FB=1_3_4_5;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n- name: Consumption Electricity Net Scope\n  value: FB=1_3_4_7;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n- name: Consumption Gas Scope\n  value: FB=1_3_4_10;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n- name: Consumption Forward Reverse Scope\n  value: FB=1_3_4_8;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n- name: Billing Information Without Cost Scope\n  value: FB=1_3_15;IntervalDuration=Monthly;BlockDuration=Monthly;HistoryLength=63072000;BR=000092\n\
  - name: Billing Information With Cost Scope\n  value: FB=1_3_15_16;IntervalDuration=Monthly;BlockDuration=Monthly;HistoryLength=63072000;BR=000092\n- name: RetailCustomer Billing Account Scope\n  value: FB=51_53_56;BR=000092\n- name: RetailCustomer Meter Scope\n  value: FB=51_53_56_57_58_60;BR=000092\n- name: Multiple Scopes combined\n  value: FB=1_3_4_5_7_8_10_15_16_51_53_56_57_58_60;IntervalDuration=Monthly_3600_900_300;BlockDuration=Monthly_Daily;HistoryLength=63072000;BR=000092\n- name: Third-Party Client Access Token (client_credentials)\n  value: FB=34_35\n  note: The bulk/client-credentials scope published in section 3.3.2; FB_34 is not described in the document's functional-block table.\n- name: Refresh-token example\n  value: FB=1_3_4_5_7_10_15_16_51_53_56_57_58_60\nflows: [authorizationCode, refreshToken, clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/scopes/con-edison-scopes.yml
summary_line: 17 scopes
tags:
- Energy
- United States
- New York
- Utilities
- Electricity
- Gas
- Steam
- Smart Metering
- Green Button
- Energy Data
- Grid
- Distribution
- Hosting Capacity
- Distributed Energy Resources
- Solar
- EV Charging
- Demand Response
token_urls: []
---
