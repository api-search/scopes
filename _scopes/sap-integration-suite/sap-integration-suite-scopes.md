---
api_specs:
- filename: sap-integration-suite-api-products-api-openapi.yml
  format: yaml
  label: SAP Integration Suite API Products API
  slug: sap-integration-suite-api-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-api-products-api-openapi.yml
- filename: sap-integration-suite-api-proxies-api-openapi.yml
  format: yaml
  label: SAP Integration Suite API Proxies API
  slug: sap-integration-suite-api-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-api-proxies-api-openapi.yml
- filename: sap-integration-suite-applications-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Applications API
  slug: sap-integration-suite-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-applications-api-openapi.yml
- filename: sap-integration-suite-developers-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Developers API
  slug: sap-integration-suite-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-developers-api-openapi.yml
- filename: sap-integration-suite-integration-flows-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Integration Flows API
  slug: sap-integration-suite-integration-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-integration-flows-api-openapi.yml
- filename: sap-integration-suite-integration-packages-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Integration Packages API
  slug: sap-integration-suite-integration-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-integration-packages-api-openapi.yml
- filename: sap-integration-suite-key-value-maps-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Key Value Maps API
  slug: sap-integration-suite-key-value-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-key-value-maps-api-openapi.yml
- filename: sap-integration-suite-message-processing-logs-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Message Processing Logs API
  slug: sap-integration-suite-message-processing-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-message-processing-logs-api-openapi.yml
- filename: sap-integration-suite-runtime-artifacts-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Runtime Artifacts API
  slug: sap-integration-suite-runtime-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-runtime-artifacts-api-openapi.yml
- filename: sap-integration-suite-service-endpoints-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Service Endpoints API
  slug: sap-integration-suite-service-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-service-endpoints-api-openapi.yml
- filename: sap-integration-suite-variables-api-openapi.yml
  format: yaml
  label: SAP Integration Suite Variables API
  slug: sap-integration-suite-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-variables-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Sap Integration Suite Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'SAP Integration Suite uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Integration Suite
provider_slug: sap-integration-suite
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-api-products-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-api-proxies-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-applications-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-developers-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-integration-flows-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-integration-packages-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-key-value-maps-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-message-processing-logs-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-runtime-artifacts-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-service-endpoints-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-variables-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-integration-suite-scopes
source_filename: sap-integration-suite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/sap-integration-suite-api-products-api-openapi.yml, openapi/sap-integration-suite-api-proxies-api-openapi.yml,\n  openapi/sap-integration-suite-applications-api-openapi.yml, openapi/sap-integration-suite-developers-api-openapi.yml,\n  openapi/sap-integration-suite-integration-flows-api-openapi.yml, openapi/sap-integration-suite-integration-packages-api-openapi.yml,\n  openapi/sap-integration-suite-key-value-maps-api-openapi.yml, openapi/sap-integration-suite-message-processing-logs-api-openapi.yml,\n  openapi/sap-integration-suite-runtime-artifacts-api-openapi.yml, openapi/sap-integration-suite-service-endpoints-api-openapi.yml,\n  openapi/sap-integration-suite-variables-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/sap-integration-suite-api-products-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source:\
  \ openapi/sap-integration-suite-api-proxies-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-applications-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-developers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-integration-flows-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-integration-packages-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n\
  - name: oauth2\n  source: openapi/sap-integration-suite-key-value-maps-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-message-processing-logs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-runtime-artifacts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-service-endpoints-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-variables-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n\
  scopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/scopes/sap-integration-suite-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Management
- Cloud Integration
- Enterprise Integration
- Event Mesh
- iPaaS
- SAP
- SAP BTP
token_bound: false
token_urls:
- https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
---
