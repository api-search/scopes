---
api_specs:
- filename: formassembly-aggregates-api-openapi.yml
  format: yaml
  label: FormAssembly Aggregates API
  slug: formassembly-aggregates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-aggregates-api-openapi.yml
- filename: formassembly-connectors-api-openapi.yml
  format: yaml
  label: FormAssembly Connectors API
  slug: formassembly-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-connectors-api-openapi.yml
- filename: formassembly-form-elements-api-openapi.yml
  format: yaml
  label: FormAssembly Form Elements API
  slug: formassembly-form-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-form-elements-api-openapi.yml
- filename: formassembly-forms-api-openapi.yml
  format: yaml
  label: FormAssembly Forms API
  slug: formassembly-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-forms-api-openapi.yml
- filename: formassembly-responses-api-openapi.yml
  format: yaml
  label: FormAssembly Responses API
  slug: formassembly-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-responses-api-openapi.yml
- filename: formassembly-themes-api-openapi.yml
  format: yaml
  label: FormAssembly Themes API
  slug: formassembly-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-themes-api-openapi.yml
- filename: formassembly-oauth2-api-openapi.yml
  format: yaml
  label: FormAssembly O Auth2 API
  slug: formassembly-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-oauth2-api-openapi.yml
authorization_urls:
- https://app.formassembly.com/oauth/login
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Formassembly Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'FormAssembly uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://app.formassembly.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FormAssembly
provider_slug: formassembly
schemes:
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  source: openapi/formassembly-aggregates-api-openapi.yml
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  source: openapi/formassembly-connectors-api-openapi.yml
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  source: openapi/formassembly-form-elements-api-openapi.yml
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  source: openapi/formassembly-forms-api-openapi.yml
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  source: openapi/formassembly-oauth2-api-openapi.yml
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  source: openapi/formassembly-responses-api-openapi.yml
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  source: openapi/formassembly-themes-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: formassembly-scopes
source_filename: formassembly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/formassembly-aggregates-api-openapi.yml, openapi/formassembly-connectors-api-openapi.yml,\n  openapi/formassembly-form-elements-api-openapi.yml, openapi/formassembly-forms-api-openapi.yml,\n  openapi/formassembly-oauth2-api-openapi.yml, openapi/formassembly-responses-api-openapi.yml,\n  openapi/formassembly-themes-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/formassembly-aggregates-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formassembly.com/oauth/login\n    tokenUrl: https://app.formassembly.com/oauth/access_token\n- name: oauth2\n  source: openapi/formassembly-connectors-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formassembly.com/oauth/login\n    tokenUrl: https://app.formassembly.com/oauth/access_token\n- name: oauth2\n  source: openapi/formassembly-form-elements-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://app.formassembly.com/oauth/login\n    tokenUrl: https://app.formassembly.com/oauth/access_token\n- name: oauth2\n  source: openapi/formassembly-forms-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formassembly.com/oauth/login\n    tokenUrl: https://app.formassembly.com/oauth/access_token\n- name: oauth2\n  source: openapi/formassembly-oauth2-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formassembly.com/oauth/login\n    tokenUrl: https://app.formassembly.com/oauth/access_token\n- name: oauth2\n  source: openapi/formassembly-responses-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formassembly.com/oauth/login\n    tokenUrl: https://app.formassembly.com/oauth/access_token\n- name: oauth2\n  source: openapi/formassembly-themes-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formassembly.com/oauth/login\n\
  \    tokenUrl: https://app.formassembly.com/oauth/access_token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/scopes/formassembly-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Forms
- Data Collection
- Salesforce
- Enterprise
- HIPAA
- Compliance
- Government
- FedRAMP
- Workflows
- E-Signature
token_bound: false
token_urls:
- https://app.formassembly.com/oauth/access_token
---
