---
authorization_urls: []
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Hubject Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Hubject uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hubject
provider_slug: hubject
schemes:
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: MO
  source: openapi/hubject-opcp-ccp-openapi.json
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: OEM
  source: openapi/hubject-opcp-ccp-openapi.json
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: CPO
  source: openapi/hubject-opcp-ccp-openapi.json
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: CPS
  source: openapi/hubject-opcp-ccp-openapi.json
- description: OAuth2 is used to grant access to the endpoint. In the case of "MO without PKI" role, the MO is using Hubject V2G PKI to sign certificates.
  flows:
  - flow: authorizationCode
  name: MO_without_PKI
  source: openapi/hubject-opcp-cps-openapi.json
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: MO_with_own_PKI
  source: openapi/hubject-opcp-cps-openapi.json
- description: OAuth2 is used to grant access to the CPO related endpoint.
  flows:
  - flow: authorizationCode
  name: CPO
  source: openapi/hubject-opcp-est-openapi.json
- description: OAuth2 is used to grant access to the MO related endpoint.
  flows:
  - flow: authorizationCode
  name: MO_with_V2G_PKI
  source: openapi/hubject-opcp-est-openapi.json
- description: OAuth2 is used to grant access to the OEM related endpoint.
  flows:
  - flow: authorizationCode
  name: OEM_with_V2G_PKI
  source: openapi/hubject-opcp-est-openapi.json
- description: OAuth2 is used to grant access to the CPS Operator related endpoint.
  flows:
  - flow: authorizationCode
  name: CPS
  source: openapi/hubject-opcp-est-openapi.json
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: MO
  source: openapi/hubject-opcp-pcp-openapi.json
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: OEM
  source: openapi/hubject-opcp-pcp-openapi.json
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: All_roles
  source: openapi/hubject-opcp-rcp-openapi.json
- description: OAuth2 is used to grant access to the endpoint.
  flows:
  - flow: authorizationCode
  name: Admin
  source: openapi/hubject-opcp-rcp-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: hubject-scopes
source_filename: hubject-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/hubject-opcp-ccp-openapi.json, openapi/hubject-opcp-cps-openapi.json, openapi/hubject-opcp-est-openapi.json,\n  openapi/hubject-opcp-pcp-openapi.json, openapi/hubject-opcp-rcp-openapi.json\nschemes:\n- name: MO\n  source: openapi/hubject-opcp-ccp-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\n- name: OEM\n  source: openapi/hubject-opcp-ccp-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\n- name: CPO\n  source: openapi/hubject-opcp-ccp-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\n- name: CPS\n  source: openapi/hubject-opcp-ccp-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\n- name: MO_without_PKI\n  source: openapi/hubject-opcp-cps-openapi.json\n\
  \  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint. In the case of \"MO without PKI\"\n    role, the MO is using Hubject V2G PKI to sign certificates.\n- name: MO_with_own_PKI\n  source: openapi/hubject-opcp-cps-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\n- name: CPO\n  source: openapi/hubject-opcp-est-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the CPO related endpoint.\n- name: MO_with_V2G_PKI\n  source: openapi/hubject-opcp-est-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the MO related endpoint.\n- name: OEM_with_V2G_PKI\n  source: openapi/hubject-opcp-est-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the OEM related endpoint.\n- name: CPS\n  source: openapi/hubject-opcp-est-openapi.json\n  flows:\n\
  \  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the CPS Operator related endpoint.\n- name: MO\n  source: openapi/hubject-opcp-pcp-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\n- name: OEM\n  source: openapi/hubject-opcp-pcp-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\n- name: All_roles\n  source: openapi/hubject-opcp-rcp-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\n- name: Admin\n  source: openapi/hubject-opcp-rcp-openapi.json\n  flows:\n  - flow: authorizationCode\n  description: OAuth2 is used to grant access to the endpoint.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/hubject/scopes/hubject-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- E-Mobility
- EV Charging
- Interoperability
token_bound: false
token_urls: []
---
