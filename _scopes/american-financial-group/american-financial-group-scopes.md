---
api_specs:
- filename: american-financial-group-shop-openapi.yml
  format: yaml
  label: Great American Carrier Services Shop API
  slug: great-american-carrier-services-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-shop-openapi.yml
- filename: american-financial-group-submission-openapi.yml
  format: yaml
  label: Great American Carrier Services Submission API
  slug: great-american-carrier-services-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-submission-openapi.yml
- filename: american-financial-group-product-openapi.yml
  format: yaml
  label: Great American Carrier Services Product API
  slug: great-american-carrier-services-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-product-openapi.yml
- filename: american-financial-group-risk-selection-openapi.yml
  format: yaml
  label: Great American Carrier Services Risk Selection API
  slug: great-american-carrier-services-risk-selection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-risk-selection-openapi.yml
- filename: american-financial-group-rating-openapi.yml
  format: yaml
  label: Great American Carrier Services Rating API
  slug: great-american-carrier-services-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-rating-openapi.yml
- filename: american-financial-group-forms-openapi.yml
  format: yaml
  label: Great American Carrier Services Forms API
  slug: great-american-carrier-services-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-forms-openapi.yml
- filename: american-financial-group-issuance-openapi.yml
  format: yaml
  label: Great American Carrier Services Issuance API
  slug: great-american-carrier-services-issuance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-issuance-openapi.yml
- filename: american-financial-group-policy-openapi.yml
  format: yaml
  label: Great American Carrier Services Policy API
  slug: great-american-carrier-services-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-policy-openapi.yml
- filename: american-financial-group-document-openapi.yml
  format: yaml
  label: Great American Carrier Services Document API
  slug: great-american-carrier-services-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-document-openapi.yml
- filename: american-financial-group-billing-openapi.yml
  format: yaml
  label: Great American Carrier Services Billing API
  slug: great-american-carrier-services-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-billing-openapi.yml
- filename: american-financial-group-ingestion-openapi.yml
  format: yaml
  label: Great American Carrier Services Ingestion API
  slug: great-american-carrier-services-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-ingestion-openapi.yml
- filename: american-financial-group-risk-assessment-openapi.yml
  format: yaml
  label: Great American Carrier Services Risk Assessment API
  slug: great-american-carrier-services-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-risk-assessment-openapi.yml
- filename: american-financial-group-letters-openapi.yml
  format: yaml
  label: Great American Carrier Services Letters API
  slug: great-american-carrier-services-letters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-letters-openapi.yml
- filename: american-financial-group-producer-openapi.yml
  format: yaml
  label: Great American Carrier Services Producer API
  slug: great-american-carrier-services-producer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-producer-openapi.yml
- filename: american-financial-group-contract-openapi.yml
  format: yaml
  label: Great American Carrier Services Contract API
  slug: great-american-carrier-services-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-contract-openapi.yml
- filename: american-financial-group-opportunity-openapi.yml
  format: yaml
  label: Great American Carrier Services Opportunity API
  slug: great-american-carrier-services-opportunity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-opportunity-openapi.yml
- filename: american-financial-group-notification-openapi.yml
  format: yaml
  label: Great American Carrier Services Notification API
  slug: great-american-carrier-services-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-notification-openapi.yml
- filename: american-financial-group-claims-openapi.yml
  format: yaml
  label: Great American Carrier Services Claims API
  slug: great-american-carrier-services-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/openapi/american-financial-group-claims-openapi.yml
authorization_urls: []
description: ''
docs: https://api-documentation.gaig.com/policy/index.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: American Financial Group Scopes
name_suffix: OAuth Scopes
note: 'Great American secures every Carrier Services API with OAuth 2.0 client_credentials but publishes no named scope vocabulary. Authorization is carried instead by `api_product_list_json` on the token response — an array of granted API product identifiers (documented example: ["issuance-dev","rating-dev"]) — and is further narrowed per consumer at runtime: GET /api/endpoints returns only the endpoints that client is entitled to call, and a call to an unentitled endpoint returns 501 Not Implemented. The published scope list is therefore genuinely empty, not merely unfound; the entitlement surface is per-client and must be read from the live /api/endpoints response.'
overview: 'American Financial Group uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: American Financial Group
provider_slug: american-financial-group
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: american-financial-group-scopes
source_filename: american-financial-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://api-documentation.gaig.com/policy/index.html\ndocs: https://api-documentation.gaig.com/policy/index.html\noauth:\n  flow: clientCredentials\n  token_endpoint_prod: https://prod01.api.gaig.com/oauth/token\nscope_count: 0\nscopes: []\nauthorization_model: api-products\nnote: >-\n  Great American secures every Carrier Services API with OAuth 2.0 client_credentials but publishes no\n  named scope vocabulary. Authorization is carried instead by `api_product_list_json` on the token\n  response — an array of granted API product identifiers (documented example: [\"issuance-dev\",\"rating-dev\"]) —\n  and is further narrowed per consumer at runtime: GET /api/endpoints returns only the endpoints that\n  client is entitled to call, and a call to an unentitled endpoint returns 501 Not Implemented. The\n  published scope list is therefore genuinely empty, not merely unfound; the entitlement surface is\n  per-client and must be read\
  \ from the live /api/endpoints response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/scopes/american-financial-group-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Property Casualty
- Specialty Insurance
- Annuities
- Financial-Services
- Commercial Insurance
- Fortune 500
token_urls: []
---
