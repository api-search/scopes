---
authorization_urls: []
description: ''
docs: https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Wordline Scopes
name_suffix: OAuth Scopes
note: Documented scopes below apply to the Worldline Acquiring API (OAuth 2.0 client credentials); the Financial Services portal APIs also use client credentials but publish no scopes (https://financial-services.developer.worldline.com/acquiring/documentation/authentication).
overview: 'Worldline publishes 7 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Worldline API on a user''s behalf.


  Tokens are issued from https://sbx-wlip.api1-eu2.psapigateway.preprod.giservices.io/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Worldline
provider_slug: wordline
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://sbx-wlip.api1-eu2.psapigateway.preprod.giservices.io/token
  name: basic
  source: openapi/worldline-card-issuing-api-2.41.1.json
scope_count: 7
scope_names:
- processing_payment
- processing_refund
- processing_credittransfer
- processing_accountverification
- processing_operation_reverse
- processing_dcc_rate
- services_ping
scopes:
- description: Allows to create, get and make actions on payments.
  flows: []
  scope: processing_payment
- description: Allows to create, get and make actions on standalone refunds.
  flows: []
  scope: processing_refund
- description: Allows to create and get a credit transfer.
  flows: []
  scope: processing_credittransfer
- description: Allows to perform an account verification.
  flows: []
  scope: processing_accountverification
- description: Allows to reverse an operation.
  flows: []
  scope: processing_operation_reverse
- description: Allows to request a dynamic currency conversion (DCC) rate.
  flows: []
  scope: processing_dcc_rate
- description: Allows to test the connection to the API.
  flows: []
  scope: services_ping
slug: wordline-scopes
source_filename: wordline-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/worldline-card-issuing-api-2.41.1.json\ndocs: https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication\nnote: Documented scopes below apply to the Worldline Acquiring API (OAuth 2.0 client\n  credentials); the Financial Services portal APIs also use client credentials but\n  publish no scopes (https://financial-services.developer.worldline.com/acquiring/documentation/authentication).\nschemes:\n- name: basic\n  source: openapi/worldline-card-issuing-api-2.41.1.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sbx-wlip.api1-eu2.psapigateway.preprod.giservices.io/token\nscopes:\n- scope: processing_payment\n  description: Allows to create, get and make actions on payments.\n  sources:\n  - https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication\n- scope: processing_refund\n  description: Allows to create, get and make actions on standalone refunds.\n\
  \  sources:\n  - https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication\n- scope: processing_credittransfer\n  description: Allows to create and get a credit transfer.\n  sources:\n  - https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication\n- scope: processing_accountverification\n  description: Allows to perform an account verification.\n  sources:\n  - https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication\n- scope: processing_operation_reverse\n  description: Allows to reverse an operation.\n  sources:\n  - https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication\n- scope: processing_dcc_rate\n  description: Allows to request a dynamic currency conversion (DCC) rate.\n  sources:\n  - https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication\n- scope: services_ping\n  description: Allows to test the connection to the API.\n  sources:\n\
  \  - https://docs.acquiring.worldline-solutions.com/Developer-Tools/API/api-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordline/refs/heads/main/scopes/wordline-scopes.yml
summary_line: 7 scopes · clientCredentials
tags:
- Payments
- Payment Processing
- Acquiring
- Issuing
- Open Banking
- Digital Banking
- FinTech
- Europe
token_urls:
- https://sbx-wlip.api1-eu2.psapigateway.preprod.giservices.io/token
---
