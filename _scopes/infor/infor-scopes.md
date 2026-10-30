---
api_specs:
- filename: infor-contents-api-openapi.yml
  format: yaml
  label: Infor Contents API
  slug: infor-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-contents-api-openapi.yml
- filename: infor-icua-api-openapi.yml
  format: yaml
  label: Infor ICUA API
  slug: infor-icua-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-icua-api-openapi.yml
- filename: infor-languages-api-openapi.yml
  format: yaml
  label: Infor Languages API
  slug: infor-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-languages-api-openapi.yml
- filename: infor-products-api-openapi.yml
  format: yaml
  label: Infor Products API
  slug: infor-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-products-api-openapi.yml
- filename: infor-recenttopics-api-openapi.yml
  format: yaml
  label: Infor Recent Topics API
  slug: infor-recenttopics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-recenttopics-api-openapi.yml
- filename: infor-s3-docs-api-openapi.yml
  format: yaml
  label: Infor S3 Docs API
  slug: infor-s3-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-s3-docs-api-openapi.yml
- filename: infor-search-api-openapi.yml
  format: yaml
  label: Infor Search API
  slug: infor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-search-api-openapi.yml
- filename: infor-security-api-openapi.yml
  format: yaml
  label: Infor Security API
  slug: infor-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-security-api-openapi.yml
- filename: infor-solutions-api-openapi.yml
  format: yaml
  label: Infor Solutions API
  slug: infor-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-solutions-api-openapi.yml
- filename: infor-userfavorites-api-openapi.yml
  format: yaml
  label: Infor User Favorites API
  slug: infor-userfavorites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-userfavorites-api-openapi.yml
- filename: infor-web-api-openapi.yml
  format: yaml
  label: Infor Web API
  slug: infor-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-web-api-openapi.yml
authorization_urls:
- https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Infor Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
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
  source: openapi/infor-ion-documents-api-openapi.yml
- description: Infor ION API Authorization Code grant
  flows:
  - authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2AuthorizationCode
  source: openapi/infor-ion-documents-api-openapi.yml
- description: Infor ION API Client Credentials grant
  flows:
  - flow: clientCredentials
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2ClientCredentials
  source: openapi/infor-m3-api-api-openapi.yml
- description: Infor ION API Authorization Code grant
  flows:
  - authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2AuthorizationCode
  source: openapi/infor-m3-api-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: infor-scopes
source_filename: infor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/infor-ion-documents-api-openapi.yml, openapi/infor-m3-api-api-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/infor-ion-documents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n  description: Infor ION API Client Credentials grant\n- name: OAuth2AuthorizationCode\n  source: openapi/infor-ion-documents-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n  description: Infor ION API Authorization Code grant\n- name: OAuth2ClientCredentials\n  source: openapi/infor-m3-api-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n  description: Infor ION API Client Credentials grant\n- name: OAuth2AuthorizationCode\n\
  \  source: openapi/infor-m3-api-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n  description: Infor ION API Authorization Code grant\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/scopes/infor-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- ERP
- Manufacturing
- Supply Chain
- Cloud
- Integration
token_bound: false
token_urls:
- https://inforos.infor.com/INFOR_DEV/as/token.oauth2
---
