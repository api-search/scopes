---
api_specs:
- filename: sap-ariba-invoices-api-openapi.yml
  format: yaml
  label: SAP Ariba Invoices API
  slug: sap-ariba-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-invoices-api-openapi.yml
- filename: sap-ariba-purchase-order-line-items-api-openapi.yml
  format: yaml
  label: SAP Ariba Purchase Order Line Items API
  slug: sap-ariba-purchase-order-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-purchase-order-line-items-api-openapi.yml
- filename: sap-ariba-purchase-orders-api-openapi.yml
  format: yaml
  label: SAP Ariba Purchase Orders API
  slug: sap-ariba-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-purchase-orders-api-openapi.yml
- filename: sap-ariba-receipts-api-openapi.yml
  format: yaml
  label: SAP Ariba Receipts API
  slug: sap-ariba-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-receipts-api-openapi.yml
- filename: sap-ariba-requisitions-api-openapi.yml
  format: yaml
  label: SAP Ariba Requisitions API
  slug: sap-ariba-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-requisitions-api-openapi.yml
- filename: sap-ariba-suppliers-api-openapi.yml
  format: yaml
  label: SAP Ariba Suppliers API
  slug: sap-ariba-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/openapi/sap-ariba-suppliers-api-openapi.yml
authorization_urls: []
description: ''
docs: https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/sap-ariba-developer-portal-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Ariba Scopes
name_suffix: OAuth Scopes
note: SAP Ariba's OAuth token requests (grant_type client_credentials or openapi_2lo against https://api.ariba.com/v2/oauth/token) do not use or document OAuth scopes; API access is governed by per-application approval and the required apiKey parameter (https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/sap-ariba-developer-portal-authentication).
overview: 'SAP Ariba uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.ariba.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Ariba
provider_slug: sap-ariba
schemes:
- description: OAuth 2.0 Client Credentials flow for SAP Ariba API authentication. Obtain client credentials from the SAP Ariba Developer Portal.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: oauth2
  source: openapi/sap-ariba-procurement-api.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-ariba-scopes
source_filename: sap-ariba-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-ariba-procurement-api.yml\ndocs: https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/sap-ariba-developer-portal-authentication\nnote: SAP Ariba's OAuth token requests (grant_type client_credentials or openapi_2lo\n  against https://api.ariba.com/v2/oauth/token) do not use or document OAuth scopes;\n  API access is governed by per-application approval and the required apiKey parameter\n  (https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/sap-ariba-developer-portal-authentication).\nschemes:\n- name: oauth2\n  source: openapi/sap-ariba-procurement-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n  description: OAuth 2.0 Client Credentials flow for SAP Ariba API authentication. Obtain client\n    credentials from the SAP Ariba Developer Portal.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/scopes/sap-ariba-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
token_urls:
- https://api.ariba.com/v2/oauth/token
---
