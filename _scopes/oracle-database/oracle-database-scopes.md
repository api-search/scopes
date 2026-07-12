---
authorization_urls:
- /ords/{schema}/oauth/auth
description: ''
docs: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/25.2/orddg/developing-REST-applications.html
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Oracle Database Scopes
name_suffix: OAuth Scopes
note: ORDS publishes no fixed OAuth scope catalog — scopes are the user-defined ORDS privilege names protecting each REST module (JWT scope claims must match the privilege name), per https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/25.2/orddg/developing-REST-applications.html.
overview: 'Oracle Database uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /ords/{schema}/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle Database
provider_slug: oracle-database
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-database-ords-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-database-soda-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: oracle-database-scopes
source_filename: oracle-database-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-database-ords-openapi.yml, openapi/oracle-database-soda-openapi.yml\ndocs: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/25.2/orddg/developing-REST-applications.html\nnote: ORDS publishes no fixed OAuth scope catalog — scopes are the user-defined ORDS\n  privilege names protecting each REST module (JWT scope claims must match the privilege\n  name), per https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/25.2/orddg/developing-REST-applications.html.\nschemes:\n- name: oauth2\n  source: openapi/oracle-database-ords-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n- name: oauth2\n  source: openapi/oracle-database-soda-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n\
  scopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/scopes/oracle-database-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Cloud
- Database
- Enterprise
- Oracle
- REST API
- SQL
token_urls:
- /ords/{schema}/oauth/token
---
