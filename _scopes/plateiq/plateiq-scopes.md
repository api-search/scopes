---
api_specs:
- filename: plateiq-openapi.yaml
  format: yaml
  label: Ottimate API
  slug: ottimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-openapi.yaml
authorization_urls: []
description: ''
docs: https://docs.ottimate.com/auth
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Plateiq Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PlateIQ uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PlateIQ
provider_slug: plateiq
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: plateiq-scopes
source_filename: plateiq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.ottimate.com/auth.md\ndocs: https://docs.ottimate.com/auth\nprovider: plateiq\napi: Ottimate API\nflow: client_credentials\nnotes: >-\n  The Ottimate OAuth2 client-credentials flow currently supports a single scope.\n  The effective data an integration can reach is further constrained by the\n  API User's account/company/location scoping (see account-structure/scoping).\nscopes:\n- name: accounts.can_access_dashboard\n  description: >-\n    Grants the OAuth application access to the Ottimate dashboard data surface\n    for the provisioned API User. Currently the only supported OAuth scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/scopes/plateiq-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Enterprise Saas
- Accounts Payable
- Invoice Automation
- Payments
- Fintech
- Restaurants
- Procurement
- Spend Management
- ERP Integration
token_urls: []
---
