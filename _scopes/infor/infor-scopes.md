---
authorization_urls:
- https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2
description: ''
docs: https://docs.infor.com/inforos/2026.x/en-us/useradminlib_cloud/apigatewayag_cloud/vya1611685179822.html
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Infor Scopes
name_suffix: OAuth Scopes
note: Infor does not publish a fixed catalog of OAuth scope strings; ION API Gateway scopes are defined and attached per authorized app or service account by tenant administrators (see "Adding scopes for authorized apps or service accounts", https://docs.infor.com/inforos/2026.x/en-us/useradminlib_cloud/apigatewayag_cloud/vya1611685179822.html).
overview: 'Infor uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://inforos.infor.com/INFOR_DEV/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Infor
provider_slug: infor
schemes:
- description: Infor ION API Client Credentials grant
  flows:
  - flow: clientCredentials
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2ClientCredentials
  source: openapi/infor-ion-api-gateway-openapi.yml
- description: Infor ION API Authorization Code grant
  flows:
  - authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2AuthorizationCode
  source: openapi/infor-ion-api-gateway-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: infor-scopes
source_filename: infor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/infor-ion-api-gateway-openapi.yml\ndocs: https://docs.infor.com/inforos/2026.x/en-us/useradminlib_cloud/apigatewayag_cloud/vya1611685179822.html\nnote: >-\n  Infor does not publish a fixed catalog of OAuth scope strings; ION API Gateway\n  scopes are defined and attached per authorized app or service account by tenant\n  administrators (see \"Adding scopes for authorized apps or service accounts\",\n  https://docs.infor.com/inforos/2026.x/en-us/useradminlib_cloud/apigatewayag_cloud/vya1611685179822.html).\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/infor-ion-api-gateway-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n  description: Infor ION API Client Credentials grant\n- name: OAuth2AuthorizationCode\n  source: openapi/infor-ion-api-gateway-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2\n\
  \    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n  description: Infor ION API Authorization Code grant\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/scopes/infor-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- ERP
- Manufacturing
- Supply Chain
- Cloud
- Integration
token_urls:
- https://inforos.infor.com/INFOR_DEV/as/token.oauth2
---
