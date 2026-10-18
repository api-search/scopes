---
api_specs:
- filename: sap-successfactors-empemployment-api-openapi.yml
  format: yaml
  label: SAP SuccessFactors EmpEmployment API
  slug: sap-successfactors-empemployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/openapi/sap-successfactors-empemployment-api-openapi.yml
- filename: sap-successfactors-empjob-api-openapi.yml
  format: yaml
  label: SAP SuccessFactors EmpJob API
  slug: sap-successfactors-empjob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/openapi/sap-successfactors-empjob-api-openapi.yml
- filename: sap-successfactors-focompany-api-openapi.yml
  format: yaml
  label: SAP SuccessFactors FOCompany API
  slug: sap-successfactors-focompany-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/openapi/sap-successfactors-focompany-api-openapi.yml
- filename: sap-successfactors-perperson-api-openapi.yml
  format: yaml
  label: SAP SuccessFactors PerPerson API
  slug: sap-successfactors-perperson-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/openapi/sap-successfactors-perperson-api-openapi.yml
- filename: sap-successfactors-upsert-api-openapi.yml
  format: yaml
  label: SAP SuccessFactors Upsert API
  slug: sap-successfactors-upsert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/openapi/sap-successfactors-upsert-api-openapi.yml
- filename: sap-successfactors-user-api-openapi.yml
  format: yaml
  label: SAP SuccessFactors User API
  slug: sap-successfactors-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/openapi/sap-successfactors-user-api-openapi.yml
- filename: sap-successfactors-user-userid-api-openapi.yml
  format: yaml
  label: SAP SuccessFactors User('{userId}') API
  slug: sap-successfactors-user-userid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/openapi/sap-successfactors-user-userid-api-openapi.yml
- filename: sap-successfactors-oauth-api-openapi.yml
  format: yaml
  label: SAP SuccessFactors OAUTH API
  slug: sap-successfactors-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/openapi/sap-successfactors-oauth-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Sap Successfactors Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'SAP SuccessFactors uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.successfactors.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP SuccessFactors
provider_slug: sap-successfactors
schemes:
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-empemployment-api-openapi.yml
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-empjob-api-openapi.yml
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-focompany-api-openapi.yml
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-oauth-api-openapi.yml
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-perperson-api-openapi.yml
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-upsert-api-openapi.yml
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-user-api-openapi.yml
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-user-userid-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-successfactors-scopes
source_filename: sap-successfactors-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/sap-successfactors-empemployment-api-openapi.yml, openapi/sap-successfactors-empjob-api-openapi.yml,\n  openapi/sap-successfactors-focompany-api-openapi.yml, openapi/sap-successfactors-oauth-api-openapi.yml,\n  openapi/sap-successfactors-perperson-api-openapi.yml, openapi/sap-successfactors-upsert-api-openapi.yml,\n  openapi/sap-successfactors-user-api-openapi.yml, openapi/sap-successfactors-user-userid-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/sap-successfactors-empemployment-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n  description: OAuth 2.0 SAML bearer assertion flow.\n- name: oauth2\n  source: openapi/sap-successfactors-empjob-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n  description: OAuth 2.0 SAML bearer assertion flow.\n- name: oauth2\n  source: openapi/sap-successfactors-focompany-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n  description: OAuth 2.0 SAML bearer assertion flow.\n- name: oauth2\n  source: openapi/sap-successfactors-oauth-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n  description: OAuth 2.0 SAML bearer assertion flow.\n- name: oauth2\n  source: openapi/sap-successfactors-perperson-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n  description: OAuth 2.0 SAML bearer assertion flow.\n- name: oauth2\n  source: openapi/sap-successfactors-upsert-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n  description: OAuth 2.0 SAML bearer assertion flow.\n- name: oauth2\n  source: openapi/sap-successfactors-user-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n\
  \  description: OAuth 2.0 SAML bearer assertion flow.\n- name: oauth2\n  source: openapi/sap-successfactors-user-userid-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n  description: OAuth 2.0 SAML bearer assertion flow.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/scopes/sap-successfactors-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- HCM
- Human Resources
- Talent Management
- Payroll
- Enterprise
- SAP
token_bound: false
token_urls:
- https://api.successfactors.com/oauth/token
---
