---
api_specs:
- filename: servicefusion-calendar-tasks-api-openapi.yml
  format: yaml
  label: Service Fusion Calendar Tasks API
  slug: servicefusion-calendar-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-calendar-tasks-api-openapi.yml
- filename: servicefusion-contacts-api-openapi.yml
  format: yaml
  label: Service Fusion Contacts API
  slug: servicefusion-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-contacts-api-openapi.yml
- filename: servicefusion-customers-api-openapi.yml
  format: yaml
  label: Service Fusion Customers API
  slug: servicefusion-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-customers-api-openapi.yml
- filename: servicefusion-estimates-api-openapi.yml
  format: yaml
  label: Service Fusion Estimates API
  slug: servicefusion-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-estimates-api-openapi.yml
- filename: servicefusion-invoices-api-openapi.yml
  format: yaml
  label: Service Fusion Invoices API
  slug: servicefusion-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-invoices-api-openapi.yml
- filename: servicefusion-jobs-api-openapi.yml
  format: yaml
  label: Service Fusion Jobs API
  slug: servicefusion-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-jobs-api-openapi.yml
- filename: servicefusion-payments-api-openapi.yml
  format: yaml
  label: Service Fusion Payments API
  slug: servicefusion-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-payments-api-openapi.yml
- filename: servicefusion-products-and-services-api-openapi.yml
  format: yaml
  label: Service Fusion Products and Services API
  slug: servicefusion-products-and-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-products-and-services-api-openapi.yml
- filename: servicefusion-techs-and-users-api-openapi.yml
  format: yaml
  label: Service Fusion Techs and Users API
  slug: servicefusion-techs-and-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-techs-and-users-api-openapi.yml
authorization_urls:
- https://api.servicefusion.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Servicefusion Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Service Fusion uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.servicefusion.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Service Fusion
provider_slug: servicefusion
schemes:
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-calendar-tasks-api-openapi.yml
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-contacts-api-openapi.yml
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-customers-api-openapi.yml
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-estimates-api-openapi.yml
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-invoices-api-openapi.yml
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-jobs-api-openapi.yml
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-payments-api-openapi.yml
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-products-and-services-api-openapi.yml
- description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.
  flows:
  - authorizationUrl: https://api.servicefusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  - flow: clientCredentials
    tokenUrl: https://api.servicefusion.com/oauth/access_token
  name: oauth2
  source: openapi/servicefusion-techs-and-users-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: servicefusion-scopes
source_filename: servicefusion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/servicefusion-calendar-tasks-api-openapi.yml, openapi/servicefusion-contacts-api-openapi.yml,\n  openapi/servicefusion-customers-api-openapi.yml, openapi/servicefusion-estimates-api-openapi.yml,\n  openapi/servicefusion-invoices-api-openapi.yml, openapi/servicefusion-jobs-api-openapi.yml,\n  openapi/servicefusion-payments-api-openapi.yml, openapi/servicefusion-products-and-services-api-openapi.yml,\n  openapi/servicefusion-techs-and-users-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/servicefusion-calendar-tasks-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n- name: oauth2\n\
  \  source: openapi/servicefusion-contacts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n- name: oauth2\n  source: openapi/servicefusion-customers-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n- name: oauth2\n  source: openapi/servicefusion-estimates-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n- name: oauth2\n  source: openapi/servicefusion-invoices-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n- name: oauth2\n  source: openapi/servicefusion-jobs-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  -\
  \ flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n- name: oauth2\n  source: openapi/servicefusion-payments-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n- name: oauth2\n  source: openapi/servicefusion-products-and-services-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description:\
  \ OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\n- name: oauth2\n  source: openapi/servicefusion-techs-and-users-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/scopes/servicefusion-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Field Service Management
- Home Services
- Contractors
- Scheduling
- Dispatch
- Invoicing
token_bound: false
token_urls:
- https://api.servicefusion.com/oauth/access_token
---
