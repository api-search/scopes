---
api_specs:
- filename: solera-dashboard-assignment-openapi.json
  format: json
  label: Solera Dashboard Assignment API
  slug: solera-dashboard-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-dashboard-assignment-openapi.json
- filename: solera-claim-images-openapi.json
  format: json
  label: Solera ClaimImages API
  slug: solera-claim-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-claim-images-openapi.json
- filename: solera-gic-integration-openapi.json
  format: json
  label: Solera EAPI GIC Integration API
  slug: solera-gic-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-gic-integration-openapi.json
- filename: solera-getdocuments-v1-openapi.json
  format: json
  label: Audatex GetDocuments API
  slug: solera-getdocuments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getdocuments-v1-openapi.json
- filename: solera-getimage-v1-openapi.json
  format: json
  label: Audatex Assignment Get Document API (GetImage)
  slug: solera-getimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getimage-v1-openapi.json
- filename: solera-eapi-getdocument-openapi.json
  format: json
  label: Solera EAPI Get Document API
  slug: solera-eapi-getdocument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-eapi-getdocument-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Solera Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Solera publishes 4 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Solera API on a user''s behalf.


  Tokens are issued from https://dispatch-login-demo.audatex.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Solera
provider_slug: solera
schemes:
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  source: openapi/solera-claim-images-openapi.json
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    tokenUrl: https://dispatch-login.audatex.com/connect/token
  name: oauth2
  source: openapi/solera-claim-images-prod-swagger.json
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  source: openapi/solera-dashboard-assignment-openapi.json
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  source: openapi/solera-eapi-getdocument-openapi.json
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    tokenUrl: https://dispatch-login.audatex.com/connect/token
  name: oauth2
  source: openapi/solera-enterprise-assignment-prod-swagger.json
- flows:
  - flow: password
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  source: openapi/solera-getdocuments-v1-openapi.json
- flows:
  - flow: password
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  source: openapi/solera-getdocuments-v2-openapi.json
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  source: openapi/solera-gic-integration-openapi.json
scope_count: 4
scope_names:
- b2b.fnol.api
- b2b.fnol.documents
- readAccess
- writeAccess
scopes:
- description: Audatex Assignment API Access
  flows:
  - password
  scope: b2b.fnol.api
- description: Audatex Assignment API Access
  flows:
  - password
  scope: b2b.fnol.documents
- description: ''
  flows: []
  scope: readAccess
- description: ''
  flows: []
  scope: writeAccess
slug: solera-scopes
source_filename: solera-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: openapi/solera-claim-images-openapi.json, openapi/solera-claim-images-prod-swagger.json,\n  openapi/solera-dashboard-assignment-openapi.json, openapi/solera-eapi-getdocument-openapi.json,\n  openapi/solera-enterprise-assignment-prod-swagger.json, openapi/solera-getdocuments-v1-openapi.json,\n  openapi/solera-getdocuments-v2-openapi.json, openapi/solera-gic-integration-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/solera-claim-images-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n  description: Authorization using the JWT Bearer scheme\n- name: oauth2\n  source: openapi/solera-claim-images-prod-swagger.json\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login.audatex.com/connect/token\n  description: Authorization using the JWT Bearer scheme\n- name: oauth2\n  source: openapi/solera-dashboard-assignment-openapi.json\n  flows:\n  - flow:\
  \ password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n  description: Authorization using the JWT Bearer scheme\n- name: oauth2\n  source: openapi/solera-eapi-getdocument-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n  description: Authorization using the JWT Bearer scheme\n- name: oauth2\n  source: openapi/solera-enterprise-assignment-prod-swagger.json\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login.audatex.com/connect/token\n  description: Authorization using the JWT Bearer scheme\n- name: oauth2\n  source: openapi/solera-getdocuments-v1-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n- name: oauth2\n  source: openapi/solera-getdocuments-v2-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n- name: oauth2\n  source: openapi/solera-gic-integration-openapi.json\n\
  \  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n  description: Authorization using the JWT Bearer scheme\nscopes:\n- scope: b2b.fnol.api\n  description: Audatex Assignment API Access\n  flows:\n  - password\n  sources:\n  - openapi/solera-claim-images-openapi.json\n  - openapi/solera-claim-images-prod-swagger.json\n  - openapi/solera-dashboard-assignment-openapi.json\n  - openapi/solera-eapi-getdocument-openapi.json\n  - openapi/solera-enterprise-assignment-prod-swagger.json\n  - openapi/solera-gic-integration-openapi.json\n- scope: b2b.fnol.documents\n  description: Audatex Assignment API Access\n  flows:\n  - password\n  sources:\n  - openapi/solera-getdocuments-v1-openapi.json\n  - openapi/solera-getdocuments-v2-openapi.json\n- scope: readAccess\n  sources:\n  - openapi/solera-dashboard-assignment-openapi.json\n  - openapi/solera-eapi-getdocument-openapi.json\n  - openapi/solera-getdocuments-v1-openapi.json\n  - openapi/solera-getdocuments-v2-openapi.json\n\
  \  - openapi/solera-gic-integration-openapi.json\n- scope: writeAccess\n  sources:\n  - openapi/solera-dashboard-assignment-openapi.json\n  - openapi/solera-eapi-getdocument-openapi.json\n  - openapi/solera-getdocuments-v1-openapi.json\n  - openapi/solera-getdocuments-v2-openapi.json\n  - openapi/solera-gic-integration-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/scopes/solera-scopes.yml
summary_line: 4 scopes · password
tags:
- Insurance
- United States
- Property and Casualty
- Claims
- Claims Technology
- Automotive Claims
- FNOL
- Vehicle Damage Assessment
- Risk Data
- CIECA
- Insurtech
token_urls:
- https://dispatch-login-demo.audatex.com/connect/token
- https://dispatch-login.audatex.com/connect/token
---
