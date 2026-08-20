---
api_specs:
- filename: autofi-api-openapi.yml
  format: yaml
  label: AutoFi API
  slug: autofi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-api-openapi.yml
authorization_urls: []
description: ''
docs: https://api.autofi.com/api.html
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Autofi Scopes
name_suffix: OAuth Scopes
note: AutoFi does not declare an `oauth2` securityScheme. It declares a single `http` `bearer` scheme (`bearerAuth`) and attaches scope strings to the per-operation security requirement, so the scope vocabulary below is read from the `security[].bearerAuth[]` arrays in the OpenAPI rather than from an oauth2 `flows.scopes` map. The reference does not publish a standalone scope / permission page, and no authorization-server metadata document is served, so these seven scopes are the complete published vocabulary as of this pass.
overview: 'AutoFi publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the AutoFi API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AutoFi
provider_slug: autofi
schemes:
- bearerFormat: Bearer {token}
  grant: client credentials (clientId + clientSecret exchanged for a JWT)
  name: bearerAuth
  scheme: bearer
  source: openapi/autofi-api-openapi.yml
  token_endpoint: https://api.autofi.com/auth/token
  type: http
scope_count: 7
scope_names:
- create:loanapplications
- read:loanapplications
- lookup:dealers
- create:dealmaker
- create:dealmakercredit
- create:estimate
- create:prequalification
scopes:
- description: Create a new loan application.
  flows: []
  scope: create:loanapplications
- description: Read loan application details and external resources.
  flows: []
  scope: read:loanapplications
- description: Look up AutoFi dealers.
  flows: []
  scope: lookup:dealers
- description: Create a Dealmaker loan application (experimental).
  flows: []
  scope: create:dealmaker
- description: Create a Dealmaker credit application (experimental).
  flows: []
  scope: create:dealmakercredit
- description: Calculate cash, finance and lease payment estimates.
  flows: []
  scope: create:estimate
- description: Submit a prequalification request.
  flows: []
  scope: create:prequalification
slug: autofi-scopes
source_filename: autofi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/autofi-api-openapi.yml\ndocs: https://api.autofi.com/api.html\nnote: >-\n  AutoFi does not declare an `oauth2` securityScheme. It declares a single `http`\n  `bearer` scheme (`bearerAuth`) and attaches scope strings to the per-operation\n  security requirement, so the scope vocabulary below is read from the\n  `security[].bearerAuth[]` arrays in the OpenAPI rather than from an oauth2\n  `flows.scopes` map. The reference does not publish a standalone scope /\n  permission page, and no authorization-server metadata document is served, so\n  these seven scopes are the complete published vocabulary as of this pass.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer {token}\n  token_endpoint: https://api.autofi.com/auth/token\n  grant: client credentials (clientId + clientSecret exchanged for a JWT)\n  source: openapi/autofi-api-openapi.yml\nscopes:\n- scope: create:loanapplications\n  description:\
  \ Create a new loan application.\n  operations:\n  - POST /v1/loan-application\n  sources: [openapi/autofi-api-openapi.yml]\n- scope: read:loanapplications\n  description: Read loan application details and external resources.\n  operations:\n  - GET /v1/loan-application/{loanApplicationId}\n  - GET /v1/loan-application/{loanApplicationId}/externalResources\n  sources: [openapi/autofi-api-openapi.yml]\n- scope: lookup:dealers\n  description: Look up AutoFi dealers.\n  operations:\n  - POST /v1/dealer/lookup\n  sources: [openapi/autofi-api-openapi.yml]\n- scope: create:dealmaker\n  description: Create a Dealmaker loan application (experimental).\n  operations:\n  - POST /v1/dealmaker\n  sources: [openapi/autofi-api-openapi.yml]\n- scope: create:dealmakercredit\n  description: Create a Dealmaker credit application (experimental).\n  operations:\n  - POST /v1/dealmaker/credit-application\n  sources: [openapi/autofi-api-openapi.yml]\n- scope: create:estimate\n  description: Calculate cash,\
  \ finance and lease payment estimates.\n  operations:\n  - POST /v1/estimate/cash\n  - POST /v1/estimate/finance\n  - POST /v1/estimate/lease\n  sources: [openapi/autofi-api-openapi.yml]\n- scope: create:prequalification\n  description: Submit a prequalification request.\n  operations:\n  - POST /v1/prequalification\n  sources: [openapi/autofi-api-openapi.yml]\nunscoped_operations:\n- POST /auth/token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/scopes/autofi-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Automotive
- Fintech
- Digital Retail
- Auto Finance
- Dealerships
- Sales Enablement
- Software-as-a-Service
- Lending
- Loan Origination
- Credit Decisioning
- Payment Calculation
- Prequalification
token_urls: []
---
