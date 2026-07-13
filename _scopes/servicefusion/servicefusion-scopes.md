---
api_specs:
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Customers API
  slug: servicefusion-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Contacts API
  slug: servicefusion-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Jobs API
  slug: servicefusion-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Estimates API
  slug: servicefusion-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Invoices API
  slug: servicefusion-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Products and Services API
  slug: servicefusion-products-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Payments API
  slug: servicefusion-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Techs and Users API
  slug: servicefusion-techs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
- filename: servicefusion-openapi.yml
  format: yaml
  label: Service Fusion Calendar Tasks API
  slug: servicefusion-calendar-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/openapi/servicefusion-openapi.yml
authorization_urls:
- https://api.servicefusion.com/oauth/authorize
description: ''
docs: https://docs.servicefusion.com/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Servicefusion Scopes
name_suffix: OAuth Scopes
note: Service Fusion's OAuth 2.0 implementation (authorization_code and client_credentials grants per the official RAML definition at https://docs.servicefusion.com/, and the Connected Apps guide at https://servicefusion.zendesk.com/hc/en-us/articles/360039138891) does not define or document any scopes; access is controlled per connected app via its client credentials, not via granular OAuth scopes.
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
  source: openapi/servicefusion-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: servicefusion-scopes
source_filename: servicefusion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/servicefusion-openapi.yml\ndocs: https://docs.servicefusion.com/\nnote: Service Fusion's OAuth 2.0 implementation (authorization_code and client_credentials\n  grants per the official RAML definition at https://docs.servicefusion.com/, and the\n  Connected Apps guide at https://servicefusion.zendesk.com/hc/en-us/articles/360039138891)\n  does not define or document any scopes; access is controlled per connected app via\n  its client credentials, not via granular OAuth scopes.\nschemes:\n- name: oauth2\n  source: openapi/servicefusion-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.servicefusion.com/oauth/authorize\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  - flow: clientCredentials\n    tokenUrl: https://api.servicefusion.com/oauth/access_token\n  description: OAuth 2.0. Access tokens are issued at https://api.servicefusion.com/oauth/access_token.\nscopes:\
  \ []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicefusion/refs/heads/main/scopes/servicefusion-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Field Service Management
- FSM
- Home Services
- Contractors
- Scheduling
- Dispatch
- Invoicing
token_urls:
- https://api.servicefusion.com/oauth/access_token
---
