---
api_specs:
- filename: alloy-com-bank-accounts-api-openapi.yml
  format: yaml
  label: Alloy Bank Accounts API
  slug: alloy-com-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-bank-accounts-api-openapi.yml
- filename: alloy-com-batches-api-openapi.yml
  format: yaml
  label: Alloy Batches API
  slug: alloy-com-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-batches-api-openapi.yml
- filename: alloy-com-cases-api-openapi.yml
  format: yaml
  label: Alloy Cases API
  slug: alloy-com-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-cases-api-openapi.yml
- filename: alloy-com-custom-lists-api-openapi.yml
  format: yaml
  label: Alloy Custom Lists API
  slug: alloy-com-custom-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-custom-lists-api-openapi.yml
- filename: alloy-com-documents-api-openapi.yml
  format: yaml
  label: Alloy Documents API
  slug: alloy-com-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-documents-api-openapi.yml
- filename: alloy-com-entities-api-openapi.yml
  format: yaml
  label: Alloy Entities API
  slug: alloy-com-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-entities-api-openapi.yml
- filename: alloy-com-evaluations-api-openapi.yml
  format: yaml
  label: Alloy Evaluations API
  slug: alloy-com-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-evaluations-api-openapi.yml
- filename: alloy-com-events-api-openapi.yml
  format: yaml
  label: Alloy Events API
  slug: alloy-com-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-events-api-openapi.yml
- filename: alloy-com-groups-api-openapi.yml
  format: yaml
  label: Alloy Groups API
  slug: alloy-com-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-groups-api-openapi.yml
- filename: alloy-com-investigations-api-openapi.yml
  format: yaml
  label: Alloy Investigations API
  slug: alloy-com-investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-investigations-api-openapi.yml
- filename: alloy-com-journeys-api-openapi.yml
  format: yaml
  label: Alloy Journeys API
  slug: alloy-com-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-journeys-api-openapi.yml
- filename: alloy-com-lists-api-openapi.yml
  format: yaml
  label: Alloy Lists API
  slug: alloy-com-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-lists-api-openapi.yml
- filename: alloy-com-oauth-api-openapi.yml
  format: yaml
  label: Alloy OAuth API
  slug: alloy-com-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-oauth-api-openapi.yml
- filename: alloy-com-parameters-api-openapi.yml
  format: yaml
  label: Alloy Parameters API
  slug: alloy-com-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-parameters-api-openapi.yml
- filename: alloy-com-portfolio-evaluations-api-openapi.yml
  format: yaml
  label: Alloy Portfolio Evaluations API
  slug: alloy-com-portfolio-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-portfolio-evaluations-api-openapi.yml
- filename: alloy-com-published-attributes-api-openapi.yml
  format: yaml
  label: Alloy Published Attributes API
  slug: alloy-com-published-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-published-attributes-api-openapi.yml
- filename: alloy-com-reviews-api-openapi.yml
  format: yaml
  label: Alloy Reviews API
  slug: alloy-com-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-reviews-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.alloy.com/public/docs/authentication-guide
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Alloy Com Scopes
name_suffix: OAuth Scopes
note: Alloy's API uses OAuth 2.0 client_credentials (API token/secret exchanged for a one-hour bearer token) or Basic HTTP auth, and does not use or document OAuth scopes (https://developer.alloy.com/public/docs/authentication-guide).
overview: 'Alloy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/bearer.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alloy
provider_slug: alloy-com
schemes:
- description: OAuth2 using a workflow token and secret to generate a bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/bearer
  name: oauth2
  source: openapi/alloy-identity-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: alloy-com-scopes
source_filename: alloy-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alloy-identity-api-openapi.yml\ndocs: https://developer.alloy.com/public/docs/authentication-guide\nnote: Alloy's API uses OAuth 2.0 client_credentials (API token/secret exchanged for a\n  one-hour bearer token) or Basic HTTP auth, and does not use or document OAuth scopes\n  (https://developer.alloy.com/public/docs/authentication-guide).\nschemes:\n- name: oauth2\n  source: openapi/alloy-identity-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/bearer\n  description: OAuth2 using a workflow token and secret to generate a bearer token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/scopes/alloy-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Identity Decisioning
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Credit Underwriting
- Ongoing Monitoring
- Case Management
- Fintech
- Banking
token_urls:
- /oauth/bearer
---
