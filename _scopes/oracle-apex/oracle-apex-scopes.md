---
api_specs:
- filename: oracle-apex-autorest-api-openapi.yml
  format: yaml
  label: Oracle APEX AutoREST API
  slug: oracle-apex-autorest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-autorest-api-openapi.yml
- filename: oracle-apex-handlers-api-openapi.yml
  format: yaml
  label: Oracle APEX Handlers API
  slug: oracle-apex-handlers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-handlers-api-openapi.yml
- filename: oracle-apex-modules-api-openapi.yml
  format: yaml
  label: Oracle APEX Modules API
  slug: oracle-apex-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-modules-api-openapi.yml
- filename: oracle-apex-oauth-clients-api-openapi.yml
  format: yaml
  label: Oracle APEX OAuth Clients API
  slug: oracle-apex-oauth-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-oauth-clients-api-openapi.yml
- filename: oracle-apex-overview-api-openapi.yml
  format: yaml
  label: Oracle APEX Overview API
  slug: oracle-apex-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-overview-api-openapi.yml
- filename: oracle-apex-parameters-api-openapi.yml
  format: yaml
  label: Oracle APEX Parameters API
  slug: oracle-apex-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-parameters-api-openapi.yml
- filename: oracle-apex-privileges-api-openapi.yml
  format: yaml
  label: Oracle APEX Privileges API
  slug: oracle-apex-privileges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-privileges-api-openapi.yml
- filename: oracle-apex-properties-api-openapi.yml
  format: yaml
  label: Oracle APEX Properties API
  slug: oracle-apex-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-properties-api-openapi.yml
- filename: oracle-apex-roles-api-openapi.yml
  format: yaml
  label: Oracle APEX Roles API
  slug: oracle-apex-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-roles-api-openapi.yml
- filename: oracle-apex-templates-api-openapi.yml
  format: yaml
  label: Oracle APEX Templates API
  slug: oracle-apex-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-templates-api-openapi.yml
authorization_urls:
- /ords/{schema}/oauth/auth
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Oracle Apex Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Oracle APEX uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /ords/{schema}/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle APEX
provider_slug: oracle-apex
schemes:
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-autorest-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-handlers-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-modules-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-oauth-clients-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-overview-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-parameters-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-privileges-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-properties-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-roles-api-openapi.yml
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-apex-templates-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: oracle-apex-scopes
source_filename: oracle-apex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/oracle-apex-autorest-api-openapi.yml, openapi/oracle-apex-handlers-api-openapi.yml,\n  openapi/oracle-apex-modules-api-openapi.yml, openapi/oracle-apex-oauth-clients-api-openapi.yml,\n  openapi/oracle-apex-overview-api-openapi.yml, openapi/oracle-apex-parameters-api-openapi.yml,\n  openapi/oracle-apex-privileges-api-openapi.yml, openapi/oracle-apex-properties-api-openapi.yml,\n  openapi/oracle-apex-roles-api-openapi.yml, openapi/oracle-apex-templates-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/oracle-apex-autorest-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source: openapi/oracle-apex-handlers-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source: openapi/oracle-apex-modules-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source: openapi/oracle-apex-oauth-clients-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization\
  \ using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source: openapi/oracle-apex-overview-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source: openapi/oracle-apex-parameters-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source: openapi/oracle-apex-privileges-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow:\
  \ authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source: openapi/oracle-apex-properties-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source: openapi/oracle-apex-roles-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n- name: oauth2\n  source:\
  \ openapi/oracle-apex-templates-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/scopes/oracle-apex-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- APEX
- Cloud
- Database
- Development Platform
- Enterprise
- Generative AI
- Low-Code
- Oracle
- ORDS
- PL/SQL
- REST API
- Web Applications
- Workflows
token_bound: false
token_urls:
- /ords/{schema}/oauth/token
---
