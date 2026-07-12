---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap S4Hana Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAP S/4HANA publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP S/4HANA API on a user''s behalf.


  Tokens are issued from https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schemes:
- description: OAuth 2.0 authentication for SAP S/4HANA Cloud
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-s4hana-sales-order-openapi.yml
scope_count: 1
scope_names:
- API_SALES_ORDER_SRV_0001
scopes:
- description: Access to Sales Order API
  flows:
  - clientCredentials
  scope: API_SALES_ORDER_SRV_0001
slug: sap-s4hana-scopes
source_filename: sap-s4hana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-s4hana-sales-order-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/sap-s4hana-sales-order-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication for SAP S/4HANA Cloud\nscopes:\n- scope: API_SALES_ORDER_SRV_0001\n  description: Access to Sales Order API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-s4hana-sales-order-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/scopes/sap-s4hana-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Business Applications
- Cloud
- Enterprise Resource Planning
- ERP
- Finance
- Human Resources
- Inventory
- Logistics
- Manufacturing
- Plant Maintenance
- Procurement
- S/4HANA
- Sales
- SAP
token_urls:
- https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token
---
