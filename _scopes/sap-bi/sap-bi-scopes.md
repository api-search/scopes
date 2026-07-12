---
authorization_urls: []
description: ''
docs: https://help.sap.com/docs/SAP_ANALYTICS_CLOUD/00f68c2e08b941f081002fd3691d86a7/4f43b54398fc4acaa5efa32badfe3df6.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Bi Scopes
name_suffix: OAuth Scopes
note: SAP does not publish named OAuth scope strings for these APIs; SAP Analytics Cloud OAuth clients are authorized via client Purpose/Access selections (Interactive Usage, or API Access with Story Listing / User Provisioning privileges) and SAP Datasphere OAuth clients via global and scoped roles/privileges (https://help.sap.com/docs/SAP_DATASPHERE/9f804b8efa8043539289f42f372c4862/3f92b46fe0314e8ba60720e409c219fc.html).
overview: 'SAP Business Intelligence uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{tenant}.sapanalytics.cloud/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Business Intelligence
provider_slug: sap-bi
schemes:
- description: OAuth 2.0 authentication for SAP Analytics Cloud
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.sapanalytics.cloud/oauth/token
  name: oauth2
  source: openapi/sap-bi-analytics-cloud-openapi.yml
- description: OAuth 2.0 authentication for SAP Datasphere
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.datasphere.cloud.sap/oauth/token
  name: oauth2
  source: openapi/sap-bi-datasphere-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-bi-scopes
source_filename: sap-bi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-bi-analytics-cloud-openapi.yml, openapi/sap-bi-datasphere-openapi.yml\ndocs: https://help.sap.com/docs/SAP_ANALYTICS_CLOUD/00f68c2e08b941f081002fd3691d86a7/4f43b54398fc4acaa5efa32badfe3df6.html\nnote: >-\n  SAP does not publish named OAuth scope strings for these APIs; SAP Analytics Cloud\n  OAuth clients are authorized via client Purpose/Access selections (Interactive Usage,\n  or API Access with Story Listing / User Provisioning privileges) and SAP Datasphere\n  OAuth clients via global and scoped roles/privileges\n  (https://help.sap.com/docs/SAP_DATASPHERE/9f804b8efa8043539289f42f372c4862/3f92b46fe0314e8ba60720e409c219fc.html).\nschemes:\n- name: oauth2\n  source: openapi/sap-bi-analytics-cloud-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.sapanalytics.cloud/oauth/token\n  description: OAuth 2.0 authentication for SAP Analytics Cloud\n- name: oauth2\n  source: openapi/sap-bi-datasphere-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.datasphere.cloud.sap/oauth/token\n  description: OAuth 2.0 authentication for SAP Datasphere\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bi/refs/heads/main/scopes/sap-bi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
token_urls:
- https://{tenant}.sapanalytics.cloud/oauth/token
- https://{tenant}.datasphere.cloud.sap/oauth/token
---
