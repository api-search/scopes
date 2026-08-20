---
api_specs:
- filename: university-of-wisconsin-madison-person-api-openapi.yml
  format: yaml
  label: Person API
  slug: person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-person-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-person-api-openapi.yml
  format: yaml
  label: Mock Person API
  slug: mock-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-person-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-person-api-certificates-openapi.yml
  format: yaml
  label: Mock Person API (Certificates)
  slug: mock-person-api-certificates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-person-api-certificates-openapi.yml
- filename: university-of-wisconsin-madison-hr-api-openapi.yml
  format: yaml
  label: HR API
  slug: hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-hr-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-hr-api-openapi.yml
  format: yaml
  label: Mock HR API
  slug: mock-hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-hr-api-openapi.yml
- filename: university-of-wisconsin-madison-manifest-api-openapi.yml
  format: yaml
  label: Manifest API
  slug: manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-manifest-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-manifest-api-openapi.yml
  format: yaml
  label: Mock Manifest API
  slug: mock-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-manifest-api-openapi.yml
- filename: university-of-wisconsin-madison-finance-api-openapi.yml
  format: yaml
  label: Finance API
  slug: finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-finance-api-openapi.yml
- filename: university-of-wisconsin-madison-locations-api-openapi.yml
  format: yaml
  label: Locations API
  slug: locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-locations-api-openapi.yml
- filename: university-of-wisconsin-madison-enterprise-billing-api-openapi.yml
  format: yaml
  label: Enterprise Billing API
  slug: enterprise-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-enterprise-billing-api-openapi.yml
- filename: university-of-wisconsin-madison-oauth-api-openapi.yml
  format: yaml
  label: OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-oauth-api-openapi.yml
- filename: university-of-wisconsin-madison-course-search-api-openapi.yml
  format: yaml
  label: Public Course Search API
  slug: course-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-course-search-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: University Of Wisconsin Madison Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Wisconsin-Madison uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Wisconsin-Madison
provider_slug: university-of-wisconsin-madison
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-wisconsin-madison-scopes
source_filename: university-of-wisconsin-madison-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: openapi/ (12 contracts)\nx-operator: institution\nsummary:\n  scopes_declared: 0\n  detail: >-\n    UW-Madison declares ZERO OAuth scopes. Every one of the 10 contracts carrying\n    OAuth2ClientCredentials declares `scopes: {}` — an empty scope object — and no operation\n    attaches a scope requirement. This is a real, measurable gap, not missing data on our side:\n    authorization is decided outside the contract, by which Apigee API products a client\n    application has been manually approved for. The contracts therefore cannot tell a consumer\n    or an agent what a token will actually permit.\n  consequence: >-\n    Least-privilege is not expressible. A token is scoped by product grant, and the product\n    grant is not machine-readable from anything UW-Madison publishes.\nscopes: []\nauthorization_model:\n  mechanism: apigee-api-product\n  products_observed:\n  - name: api-team-manifest-api\n    display: Manifest API\n\
  \    approval: manual\n  - name: eces-api-enterprise-billing\n    display: Enterprise Billing API\n    approval: manual\n  detail: >-\n    Read from the developer portal's own catalog endpoint\n    (/portals/api/sites/{siteId}/liveportal/apis). Every listed API product uses\n    approvalType \"manual\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/scopes/university-of-wisconsin-madison-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Wisconsin
- Big Ten
- Association of American Universities
- Identity
- Identity Federation
- Course Catalog
- Research Repository
- Student Information System
- Human Resources
- Finance
- Curriculum
token_urls: []
---
