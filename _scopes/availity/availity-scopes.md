---
api_specs:
- filename: availity-auth-attachments-api-openapi.yml
  format: yaml
  label: availity Auth Attachments API
  slug: availity-auth-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-auth-attachments-api-openapi.yml
- filename: availity-claim-attachments-api-openapi.yml
  format: yaml
  label: availity Claim Attachments API
  slug: availity-claim-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-attachments-api-openapi.yml
- filename: availity-claim-status-api-openapi.yml
  format: yaml
  label: availity Claim Status API
  slug: availity-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-claim-status-api-openapi.yml
- filename: availity-eligibility-api-openapi.yml
  format: yaml
  label: availity Eligibility API
  slug: availity-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-eligibility-api-openapi.yml
- filename: availity-enhanced-claim-status-api-openapi.yml
  format: yaml
  label: availity Enhanced Claim Status API
  slug: availity-enhanced-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-enhanced-claim-status-api-openapi.yml
- filename: availity-is-auth-required-api-openapi.yml
  format: yaml
  label: availity Is Auth Required API
  slug: availity-is-auth-required-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-is-auth-required-api-openapi.yml
- filename: availity-service-reviews-api-openapi.yml
  format: yaml
  label: availity Service Reviews API
  slug: availity-service-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/openapi/availity-service-reviews-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.availity.com/blog/2025/3/25/availity-api-guide
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Availity Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Availity publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Availity API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Availity
provider_slug: availity
schemes:
- declared_in: all 11 harvested Swagger documents
  flow: application (client credentials)
  name: oauth2
  tokenUrl: https://api.availity.com/v1/token
  type: oauth2
scope_count: 10
scope_names:
- healthcare-hipaa-transactions
- healthcare-hipaa-transactions-standard
- healthcare-hipaa-transactions-demo
- healthcare-hipaa-transactions-highvolume
- healthcare-hipaa-transactions-highvolume-standard
- healthcare-hipaa-transactions-highvolume-unlimited
- rcm-coverages
- rcm-coverages-standard
- aws-availity-payer-list
- aws-availity-payer-list-standard
scopes:
- description: Healthcare HIPAA Transactions — the core product covering Coverages (270/271), Claim Statuses (276/277), Service Reviews (278), Dental Claims, Professional and Institutional claim predeterminations, Configurations, Payer List and Dfs file download.
  flows: []
  scope: healthcare-hipaa-transactions
- description: Standard plan tier — 100,000 calls per day, 100 calls per second, production data.
  flows: []
  scope: healthcare-hipaa-transactions-standard
- description: Demo plan tier — 500 calls per day, 5 calls per second, sandbox environment returning canned PHI-free responses. Auto-approved, no contract required.
  flows: []
  scope: healthcare-hipaa-transactions-demo
- description: Healthcare HIPAA Transactions High Volume — the elevated-throughput variant of the core product.
  flows: []
  scope: healthcare-hipaa-transactions-highvolume
- description: Standard plan tier within the High Volume product.
  flows: []
  scope: healthcare-hipaa-transactions-highvolume-standard
- description: Unlimited plan tier within the High Volume product. No published quota; this tier is not listed on the public catalogue page and is presumably contract-only.
  flows: []
  scope: healthcare-hipaa-transactions-highvolume-unlimited
- description: RCM Coverages — a revenue-cycle-management-specific entitlement over the Coverages (270/271) API. Declared in the Coverages Swagger but not offered as a public catalogue product; visible only inside the machine-readable document.
  flows: []
  scope: rcm-coverages
- description: Standard plan tier within the RCM Coverages product.
  flows: []
  scope: rcm-coverages-standard
- description: AWS Availity Payer List — a separately subscribable product exposing the payer list through an AWS-hosted route at basePath /epdm-payer-list-aws/v1.
  flows: []
  scope: aws-availity-payer-list
- description: Standard plan tier — 1,000,000 calls per day, 100 calls per second.
  flows: []
  scope: aws-availity-payer-list-standard
slug: availity-scopes
source_filename: availity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/_harvested/*-swagger.json (securityDefinitions.oauth2.scopes, first-party documents harvested from developer.availity.com), https://developer.availity.com/blog/2025/3/25/availity-api-guide\ndocs: https://developer.availity.com/blog/2025/3/25/availity-api-guide\nprovider: Availity\nproviderId: availity\nsupersedes: >-\n  The previous derived version of this file (2026-07-11) listed a single scope \"hipaa\" read from\n  hand-authored specs. That was wrong. Availity's real scope vocabulary is the product/plan pair\n  vocabulary below, read from Availity's own published Swagger securityDefinitions.\nsummary: >-\n  Availity's OAuth scopes are not permission verbs. They are PRODUCT and PLAN identifiers: one\n  scope names the API product you subscribed to, and a second, suffixed scope names the plan tier\n  within it. The API Guide instructs callers to send both, space-separated, in the token request:\n  `scope=healthcare-hipaa-transactions\
  \ healthcare-hipaa-transactions-demo`. There is no read/write\n  split and no per-operation scoping — every operation in a product is reachable with the product\n  scope.\nschemes:\n  - name: oauth2\n    type: oauth2\n    flow: application (client credentials)\n    tokenUrl: https://api.availity.com/v1/token\n    declared_in: all 11 harvested Swagger documents\nscope_model:\n  shape: '<product-scope> [<plan-scope>]'\n  request_parameter: scope\n  separator: single space\n  example_request: 'grant_type=client_credentials&client_id=$API_KEY&client_secret=$CLIENT_SECRET&scope=healthcare-hipaa-transactions healthcare-hipaa-transactions-demo'\n  note: >-\n    The token response echoes the granted scope string. Availity warns that the request body\n    parameters are case sensitive.\nscopes:\n  - scope: healthcare-hipaa-transactions\n    kind: product\n    description: >-\n      Healthcare HIPAA Transactions — the core product covering Coverages (270/271), Claim Statuses\n      (276/277), Service\
  \ Reviews (278), Dental Claims, Professional and Institutional claim\n      predeterminations, Configurations, Payer List and Dfs file download.\n    product: healthcare-hipaa-transactions\n    declared_in:\n      - availity-care-cost-estimator-institutional\n      - availity-care-cost-estimator-professional\n      - availity-claim-statuses\n      - availity-configurations\n      - availity-coverages\n      - availity-dental-claims\n      - availity-dfs\n      - availity-patient-cost-estimator-professional\n      - availity-payer-list\n      - availity-service-reviews\n  - scope: healthcare-hipaa-transactions-standard\n    kind: plan\n    description: Standard plan tier — 100,000 calls per day, 100 calls per second, production data.\n    product: healthcare-hipaa-transactions\n  - scope: healthcare-hipaa-transactions-demo\n    kind: plan\n    description: >-\n      Demo plan tier — 500 calls per day, 5 calls per second, sandbox environment returning canned\n      PHI-free responses. Auto-approved,\
  \ no contract required.\n    product: healthcare-hipaa-transactions-demo\n  - scope: healthcare-hipaa-transactions-highvolume\n    kind: product\n    description: Healthcare HIPAA Transactions High Volume — the elevated-throughput variant of the core product.\n    product: healthcare-hipaa-transactions-highvolume\n  - scope: healthcare-hipaa-transactions-highvolume-standard\n    kind: plan\n    description: Standard plan tier within the High Volume product.\n    product: healthcare-hipaa-transactions-highvolume\n  - scope: healthcare-hipaa-transactions-highvolume-unlimited\n    kind: plan\n    description: >-\n      Unlimited plan tier within the High Volume product. No published quota; this tier is not\n      listed on the public catalogue page and is presumably contract-only.\n    product: healthcare-hipaa-transactions-highvolume\n  - scope: rcm-coverages\n    kind: product\n    description: >-\n      RCM Coverages — a revenue-cycle-management-specific entitlement over the Coverages\
  \ (270/271)\n      API. Declared in the Coverages Swagger but not offered as a public catalogue product; visible\n      only inside the machine-readable document.\n    product: rcm-coverages\n    declared_in:\n      - availity-coverages\n  - scope: rcm-coverages-standard\n    kind: plan\n    description: Standard plan tier within the RCM Coverages product.\n    product: rcm-coverages\n  - scope: aws-availity-payer-list\n    kind: product\n    description: >-\n      AWS Availity Payer List — a separately subscribable product exposing the payer list through an\n      AWS-hosted route at basePath /epdm-payer-list-aws/v1.\n    product: aws-availity-payer-list\n    declared_in:\n      - availity-aws-payer-list\n  - scope: aws-availity-payer-list-standard\n    kind: plan\n    description: Standard plan tier — 1,000,000 calls per day, 100 calls per second.\n    product: aws-availity-payer-list\nanomalies:\n  - >-\n    Every harvested document declares its operation-level requirement as\n    `security:\
  \ [{\"oauth2\": [\"hipaa\"]}]` — referencing a scope named \"hipaa\" that is NOT defined in\n    any securityDefinitions.scopes map. The scope vocabulary Availity actually issues at the token\n    endpoint is the product/plan vocabulary above. The \"hipaa\" reference appears to be a stale\n    literal in the gateway's spec-generation template. Recorded because a code generator reading\n    these specs will emit a token request for a scope Availity will not grant.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/scopes/availity-scopes.yml
summary_line: 10 scopes
tags:
- Healthcare
- Clearinghouse
- HIPAA
- X12 EDI
- Eligibility
- Claims
- Prior Authorization
- Revenue Cycle Management
- Payers
- Price Transparency
token_urls: []
---
