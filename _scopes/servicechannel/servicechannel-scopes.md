---
api_specs:
- filename: servicechannel-service-automation-openapi-original.json
  format: json
  label: ServiceChannel Service Automation API
  slug: servicechannel-service-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/openapi/servicechannel-service-automation-openapi-original.json
- filename: servicechannel-fixxbook-openapi-original.json
  format: json
  label: ServiceChannel Fixxbook API
  slug: servicechannel-fixxbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/openapi/servicechannel-fixxbook-openapi-original.json
authorization_urls:
- https://sb2login.servicechannel.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Servicechannel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ServiceChannel uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sb2login.servicechannel.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ServiceChannel
provider_slug: servicechannel
schemes:
- description: OAuth2 Authorization
  flows:
  - authorizationUrl: https://sb2login.servicechannel.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sb2login.servicechannel.com/oauth/token
  name: oauth2
  source: openapi/servicechannel-fixxbook-openapi-original.json
- description: OAuth2 Authorization
  flows:
  - authorizationUrl: https://sb2login.servicechannel.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sb2login.servicechannel.com/oauth/token
  name: oauth2
  source: openapi/servicechannel-service-automation-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: servicechannel-scopes
source_filename: servicechannel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/servicechannel-fixxbook-openapi-original.json, openapi/servicechannel-service-automation-openapi-original.json\nschemes:\n- name: oauth2\n  source: openapi/servicechannel-fixxbook-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sb2login.servicechannel.com/oauth/authorize\n    tokenUrl: https://sb2login.servicechannel.com/oauth/token\n  description: OAuth2 Authorization\n- name: oauth2\n  source: openapi/servicechannel-service-automation-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sb2login.servicechannel.com/oauth/authorize\n    tokenUrl: https://sb2login.servicechannel.com/oauth/token\n  description: OAuth2 Authorization\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/scopes/servicechannel-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Services
- Facilities Management
- Work Orders
- Field Service
- Maintenance
- Asset Management
- Service Providers
- Invoicing
token_urls:
- https://sb2login.servicechannel.com/oauth/token
---
