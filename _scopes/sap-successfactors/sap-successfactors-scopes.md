---
authorization_urls: []
description: ''
docs: https://help.sap.com/docs/successfactors-platform/sap-successfactors-api-reference-guide-odata-v2/authentication-using-oauth-2-0
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Successfactors Scopes
name_suffix: OAuth Scopes
note: SAP SuccessFactors OAuth 2.0 (SAML bearer assertion flow) does not use published OAuth scopes; access tokens carry an empty scope and API authorization is governed by the role-based permissions (RBP) of the user identified in the SAML assertion (https://help.sap.com/docs/successfactors-platform/sap-successfactors-api-reference-guide-odata-v2/authentication-using-oauth-2-0).
overview: 'SAP SuccessFactors uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.successfactors.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP SuccessFactors
provider_slug: sap-successfactors
schemes:
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  source: openapi/sap-successfactors-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-successfactors-scopes
source_filename: sap-successfactors-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-successfactors-openapi.yml\ndocs: https://help.sap.com/docs/successfactors-platform/sap-successfactors-api-reference-guide-odata-v2/authentication-using-oauth-2-0\nnote: >-\n  SAP SuccessFactors OAuth 2.0 (SAML bearer assertion flow) does not use\n  published OAuth scopes; access tokens carry an empty scope and API\n  authorization is governed by the role-based permissions (RBP) of the user\n  identified in the SAML assertion\n  (https://help.sap.com/docs/successfactors-platform/sap-successfactors-api-reference-guide-odata-v2/authentication-using-oauth-2-0).\nschemes:\n- name: oauth2\n  source: openapi/sap-successfactors-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n  description: OAuth 2.0 SAML bearer assertion flow.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/scopes/sap-successfactors-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- HCM
- HR
- Human Resources
- Talent Management
- Payroll
- Enterprise
- SAP
token_urls:
- https://api.successfactors.com/oauth/token
---
