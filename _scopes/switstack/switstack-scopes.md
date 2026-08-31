---
api_specs:
- filename: switstack-auth-api-openapi.yml
  format: yaml
  label: Switstack Auth API
  slug: switstack-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-auth-api-openapi.yml
- filename: switstack-bom-api-openapi.yml
  format: yaml
  label: Switstack BOM API
  slug: switstack-bom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-bom-api-openapi.yml
- filename: switstack-config-api-openapi.yml
  format: yaml
  label: Switstack Config API
  slug: switstack-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-config-api-openapi.yml
- filename: switstack-parser-api-openapi.yml
  format: yaml
  label: Switstack Parser API
  slug: switstack-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-parser-api-openapi.yml
- filename: switstack-payment-api-openapi.yml
  format: yaml
  label: Switstack Payment API
  slug: switstack-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-payment-api-openapi.yml
- filename: switstack-suite-api-openapi.yml
  format: yaml
  label: Switstack Suite API
  slug: switstack-suite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-suite-api-openapi.yml
- filename: switstack-test-api-openapi.yml
  format: yaml
  label: Switstack Test API
  slug: switstack-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-test-api-openapi.yml
- filename: switstack-validation-api-openapi.yml
  format: yaml
  label: Switstack Validation API
  slug: switstack-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-validation-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.switstack.io/switcloud/security_authentication/
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Switstack Scopes
name_suffix: OAuth Scopes
note: Switstack publishes OAuth 2.0 but no scope vocabulary. Both OpenAPI documents declare the password flow with an empty `scopes` map, and the Switcloud security & authentication page describes authorization as three named roles (Super Admin, Organization Admin, Simple User) rather than delegatable scopes; Swittest documents two (Data, Full). There is no published scopes/permissions reference page. The roles are recorded in authentication/switstack-authentication.yml under authorization_model — an honest zero here, not an omission.
overview: 'Switstack uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Switstack
provider_slug: switstack
schemes:
- flows:
  - flow: password
    tokenUrl: auth/token
  - flow: clientCredentials
    source: https://docs.switstack.io/switcloud/security_authentication/
    tokenUrl: auth/token
  name: OAuth2PasswordBearer
  source: openapi/switstack-switcloud-openapi.yml
- flows:
  - flow: password
    tokenUrl: auth/token
  name: OAuth2PasswordBearer
  source: openapi/switstack-swittest-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: switstack-scopes
source_filename: switstack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/switstack-switcloud-openapi.yml, openapi/switstack-swittest-openapi.yml\ndocs: https://docs.switstack.io/switcloud/security_authentication/\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/switstack-switcloud-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: auth/token\n  - flow: clientCredentials\n    tokenUrl: auth/token\n    source: https://docs.switstack.io/switcloud/security_authentication/\n- name: OAuth2PasswordBearer\n  source: openapi/switstack-swittest-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: auth/token\nscopes: []\nscope_count: 0\nnote: >-\n  Switstack publishes OAuth 2.0 but no scope vocabulary. Both OpenAPI documents declare the password flow with an\n  empty `scopes` map, and the Switcloud security & authentication page describes authorization as three named roles\n  (Super Admin, Organization Admin, Simple User) rather than delegatable scopes; Swittest documents two (Data,\n\
  \  Full). There is no published scopes/permissions reference page. The roles are recorded in\n  authentication/switstack-authentication.yml under authorization_model — an honest zero here, not an omission.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/scopes/switstack-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Fintech Insurtech
- Payments
- EMV
- emv-level-2
- card-present
- point-of-sale
- softpos
- tap-to-pay
- payment-terminals
- in-store-payments
- pci-mpoc
- certification-testing
- retail-payments
- estate-management
token_urls:
- auth/token
---
