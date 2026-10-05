---
api_specs:
- filename: ottimate-accounts-api-openapi.yml
  format: yaml
  label: Ottimate Accounts API
  slug: ottimate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-accounts-api-openapi.yml
- filename: ottimate-batch-api-openapi.yml
  format: yaml
  label: Ottimate Batch API
  slug: ottimate-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-batch-api-openapi.yml
- filename: ottimate-catalog-api-openapi.yml
  format: yaml
  label: Ottimate Catalog API
  slug: ottimate-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-catalog-api-openapi.yml
- filename: ottimate-dimensions-api-openapi.yml
  format: yaml
  label: Ottimate Dimensions API
  slug: ottimate-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-dimensions-api-openapi.yml
- filename: ottimate-invoices-api-openapi.yml
  format: yaml
  label: Ottimate Invoices API
  slug: ottimate-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-invoices-api-openapi.yml
- filename: ottimate-oauth-api-openapi.yml
  format: yaml
  label: Ottimate OAuth API
  slug: ottimate-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-oauth-api-openapi.yml
- filename: ottimate-receipts-api-openapi.yml
  format: yaml
  label: Ottimate Receipts API
  slug: ottimate-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-receipts-api-openapi.yml
- filename: ottimate-vendors-api-openapi.yml
  format: yaml
  label: Ottimate Vendors API
  slug: ottimate-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-vendors-api-openapi.yml
- filename: ottimate-purchase-orders-api-openapi.yml
  format: yaml
  label: Ottimate Purchase Orders API
  slug: ottimate-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/openapi/ottimate-purchase-orders-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.ottimate.com/auth
flows:
- client_credentials
kind: oauth-scopes
layout: scope
method: searched
name: Plateiq Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ottimate publishes 1 OAuth 2.0 scope via the client_credentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ottimate API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ottimate
provider_slug: ottimate
schemes: []
scope_count: 1
scope_names:
- accounts.can_access_dashboard
scopes:
- description: Grants the OAuth application access to the Ottimate dashboard data surface for the provisioned API User. Currently the only supported OAuth scope.
  flows: []
  scope: accounts.can_access_dashboard
slug: plateiq-scopes
source_filename: plateiq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.ottimate.com/auth.md\ndocs: https://docs.ottimate.com/auth\nprovider: plateiq\napi: Ottimate API\nflow: client_credentials\nnotes: >-\n  The Ottimate OAuth2 client-credentials flow currently supports a single scope.\n  The effective data an integration can reach is further constrained by the\n  API User's account/company/location scoping (see account-structure/scoping).\nscopes:\n- name: accounts.can_access_dashboard\n  description: >-\n    Grants the OAuth application access to the Ottimate dashboard data surface\n    for the provisioned API User. Currently the only supported OAuth scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ottimate/refs/heads/main/scopes/plateiq-scopes.yml
summary_line: 1 scope · client_credentials
tags:
- Company
- Enterprise Saas
- Accounts Payable
- Invoice Automation
- Payments
- Fintech
- Restaurant
- Procurement
- Spend Management
- ERP Integration
token_bound: false
token_urls: []
---
