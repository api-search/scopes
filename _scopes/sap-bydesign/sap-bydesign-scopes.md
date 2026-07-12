---
authorization_urls: []
description: ''
docs: https://github.com/SAP-samples/partner-reference-application/blob/main/Tutorials/35b-Multi-Tenancy-Provisioning-Connect-ByD.md
flows:
- clientCredentials
- saml2Bearer
kind: oauth-scopes
layout: scope
method: searched
name: Sap Bydesign Scopes
name_suffix: OAuth Scopes
note: SAP Business ByDesign does not publish a full OAuth scopes catalog; scopes are tenant-specific work center IDs granted to an OAuth 2.0 client registration in the "Application and User Management - OAuth 2.0 Client Registration" work center view, and UIWC:CC_HOME is the only scope ID documented publicly by SAP (see docs URL).
overview: 'SAP Business ByDesign publishes 1 OAuth 2.0 scope via the clientCredentials and saml2Bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP Business ByDesign API on a user''s behalf.


  Tokens are issued from https://{tenant}.bydesign.cloud.sap/sap/bc/sec/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Business ByDesign
provider_slug: sap-bydesign
schemes:
- description: OAuth 2.0 authentication for SAP Business ByDesign.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.bydesign.cloud.sap/sap/bc/sec/oauth2/token
  - description: OAuth 2.0 SAML Bearer assertion flow used for principal propagation from SAP BTP and side-by-side extensions into SAP Business ByDesign.
    flow: saml2Bearer
    tokenUrl: https://{tenant}.bydesign.cloud.sap/sap/bc/sec/oauth2/token
  name: oAuth2
  source: openapi/sap-bydesign-odata-api.json
scope_count: 1
scope_names:
- UIWC:CC_HOME
scopes:
- description: Home work center scope. SAP's official guidance states selecting scope ID UIWC:CC_HOME "is sufficient for most use cases"; effective access to OData services is determined by the work centers assigned to the OAuth client and the propagated business user's authorizations.
  flows: []
  scope: UIWC:CC_HOME
slug: sap-bydesign-scopes
source_filename: sap-bydesign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/sap-bydesign-odata-api.json\ndocs: https://github.com/SAP-samples/partner-reference-application/blob/main/Tutorials/35b-Multi-Tenancy-Provisioning-Connect-ByD.md\nschemes:\n- name: oAuth2\n  source: openapi/sap-bydesign-odata-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.bydesign.cloud.sap/sap/bc/sec/oauth2/token\n  - flow: saml2Bearer\n    tokenUrl: https://{tenant}.bydesign.cloud.sap/sap/bc/sec/oauth2/token\n    description: OAuth 2.0 SAML Bearer assertion flow used for principal propagation\n      from SAP BTP and side-by-side extensions into SAP Business ByDesign.\n  description: OAuth 2.0 authentication for SAP Business ByDesign.\nnote: SAP Business ByDesign does not publish a full OAuth scopes catalog; scopes\n  are tenant-specific work center IDs granted to an OAuth 2.0 client registration\n  in the \"Application and User Management - OAuth 2.0 Client Registration\" work center\n\
  \  view, and UIWC:CC_HOME is the only scope ID documented publicly by SAP (see docs\n  URL).\nscopes:\n- scope: UIWC:CC_HOME\n  description: Home work center scope. SAP's official guidance states selecting scope\n    ID UIWC:CC_HOME \"is sufficient for most use cases\"; effective access to OData\n    services is determined by the work centers assigned to the OAuth client and the\n    propagated business user's authorizations.\n  sources:\n  - https://github.com/SAP-samples/partner-reference-application/blob/main/Tutorials/35b-Multi-Tenancy-Provisioning-Connect-ByD.md\n  - https://github.com/SAP-samples/sme-partner-reference-application/blob/main/Tutorials/04-ByD-Integration.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/scopes/sap-bydesign-scopes.yml
summary_line: 1 scope · clientCredentials/saml2Bearer
tags:
- ERP
- Cloud
- Midmarket
- Financials
- CRM
- Procurement
- Supply Chain
- Project Management
- OData
- SOAP
- SAP
token_urls:
- https://{tenant}.bydesign.cloud.sap/sap/bc/sec/oauth2/token
---
