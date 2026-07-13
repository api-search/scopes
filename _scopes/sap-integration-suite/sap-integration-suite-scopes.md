---
api_specs:
- filename: sap-integration-suite-cloud-integration-openapi.yml
  format: yaml
  label: SAP Cloud Integration API
  slug: sap-cloud-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-cloud-integration-openapi.yml
- filename: sap-integration-suite-api-management-openapi.yml
  format: yaml
  label: SAP API Management API
  slug: sap-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-api-management-openapi.yml
authorization_urls: []
description: ''
docs: https://help.sap.com/docs/integration-suite/sap-integration-suite/tasks-and-permissions-556d5575d4b0483e85d4f3251f21d0ec
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Integration Suite Scopes
name_suffix: OAuth Scopes
note: SAP Integration Suite APIs use OAuth 2.0 client credentials with role-based authorization rather than published OAuth scopes; access to each API resource is granted by assigning documented role templates (for example MonitoringDataRead or WorkspacePackagesRead) to the SAP BTP service instance, per https://help.sap.com/docs/integration-suite/sap-integration-suite/tasks-and-permissions-556d5575d4b0483e85d4f3251f21d0ec.
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
  source: openapi/sap-integration-suite-api-management-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-integration-suite-cloud-integration-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-integration-suite-scopes
source_filename: sap-integration-suite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-integration-suite-api-management-openapi.yml, openapi/sap-integration-suite-cloud-integration-openapi.yml\ndocs: https://help.sap.com/docs/integration-suite/sap-integration-suite/tasks-and-permissions-556d5575d4b0483e85d4f3251f21d0ec\nnote: >-\n  SAP Integration Suite APIs use OAuth 2.0 client credentials with role-based\n  authorization rather than published OAuth scopes; access to each API resource\n  is granted by assigning documented role templates (for example\n  MonitoringDataRead or WorkspacePackagesRead) to the SAP BTP service instance,\n  per\n  https://help.sap.com/docs/integration-suite/sap-integration-suite/tasks-and-permissions-556d5575d4b0483e85d4f3251f21d0ec.\nschemes:\n- name: oauth2\n  source: openapi/sap-integration-suite-api-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-integration-suite-cloud-integration-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\nscopes: []\n"
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
token_urls:
- https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
---
