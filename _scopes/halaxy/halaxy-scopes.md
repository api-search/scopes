---
api_specs:
- filename: halaxy-appointment-api-openapi.yml
  format: yaml
  label: Halaxy Appointment API
  slug: halaxy-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-appointment-api-openapi.yml
- filename: halaxy-chargeitemdefinition-api-openapi.yml
  format: yaml
  label: Halaxy Charge Item Definition API
  slug: halaxy-chargeitemdefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-chargeitemdefinition-api-openapi.yml
- filename: halaxy-coverage-api-openapi.yml
  format: yaml
  label: Halaxy Coverage API
  slug: halaxy-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-coverage-api-openapi.yml
- filename: halaxy-invoice-api-openapi.yml
  format: yaml
  label: Halaxy Invoice API
  slug: halaxy-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-invoice-api-openapi.yml
- filename: halaxy-invoiceline-api-openapi.yml
  format: yaml
  label: Halaxy Invoice Line API
  slug: halaxy-invoiceline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-invoiceline-api-openapi.yml
- filename: halaxy-organization-api-openapi.yml
  format: yaml
  label: Halaxy Organization API
  slug: halaxy-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-organization-api-openapi.yml
- filename: halaxy-patient-api-openapi.yml
  format: yaml
  label: Halaxy Patient API
  slug: halaxy-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-patient-api-openapi.yml
- filename: halaxy-paymenttransaction-api-openapi.yml
  format: yaml
  label: Halaxy Payment Transaction API
  slug: halaxy-paymenttransaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-paymenttransaction-api-openapi.yml
- filename: halaxy-practitioner-api-openapi.yml
  format: yaml
  label: Halaxy Practitioner API
  slug: halaxy-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-practitioner-api-openapi.yml
- filename: halaxy-referral-api-openapi.yml
  format: yaml
  label: Halaxy Referral API
  slug: halaxy-referral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-referral-api-openapi.yml
- filename: halaxy-referraldefinition-api-openapi.yml
  format: yaml
  label: Halaxy Referral Definition API
  slug: halaxy-referraldefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-referraldefinition-api-openapi.yml
- filename: halaxy-schedule-api-openapi.yml
  format: yaml
  label: Halaxy Schedule API
  slug: halaxy-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-schedule-api-openapi.yml
- filename: halaxy-slot-api-openapi.yml
  format: yaml
  label: Halaxy Slot API
  slug: halaxy-slot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-slot-api-openapi.yml
- filename: halaxy-capability-statement-api-openapi.yml
  format: yaml
  label: Halaxy Capability Statement API
  slug: halaxy-capability-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-capability-statement-api-openapi.yml
- filename: halaxy-document-reference-api-openapi.yml
  format: yaml
  label: Halaxy Document Reference API
  slug: halaxy-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-document-reference-api-openapi.yml
- filename: halaxy-healthcare-service-api-openapi.yml
  format: yaml
  label: Halaxy Healthcare Service API
  slug: halaxy-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-healthcare-service-api-openapi.yml
- filename: halaxy-practitioner-role-api-openapi.yml
  format: yaml
  label: Halaxy Practitioner Role API
  slug: halaxy-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-practitioner-role-api-openapi.yml
- filename: halaxy-search-parameter-api-openapi.yml
  format: yaml
  label: Halaxy Search Parameter API
  slug: halaxy-search-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-search-parameter-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.halaxy.com/docs/troubleshooting-guide.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Halaxy Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one. The docs publish no OAuth scope reference either; access is set per API key in the Halaxy API Key Manager ("Check the API Key Manager in Halaxy - does your API key have appropriate access for the request objective? (You can check this in Settings > Integrations > External)").
overview: 'Halaxy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /main/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Halaxy
provider_slug: halaxy
schemes:
- description: OAuth 2.0 client credentials Grant
  flows:
  - flow: clientCredentials
    tokenUrl: /main/oauth/token
  name: oauth
  source: openapi/halaxy-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: halaxy-scopes
source_filename: halaxy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: none\nsource: openapi/halaxy-api-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/halaxy-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /main/oauth/token\n  description: OAuth 2.0 client credentials Grant\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security\n  requirement references one. The docs publish no OAuth scope reference either; access\n  is set per API key in the Halaxy API Key Manager (\"Check the API Key Manager in\n  Halaxy - does your API key have appropriate access for the request objective? (You\n  can check this in Settings > Integrations > External)\").\ndocs: https://developers.halaxy.com/docs/troubleshooting-guide.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/scopes/halaxy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Practice Management
- FHIR
- Telehealth
- Appointments
- Billing
- Patients
token_bound: false
token_urls:
- /main/oauth/token
---
