---
authorization_urls: []
description: ''
docs: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/19.4/aelig/OAUTH-reference.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Oracle Database 19C Scopes
name_suffix: OAuth Scopes
note: ORDS OAuth 2.0 does not use named scopes; access for OAuth clients is controlled through ORDS privileges (p_privilege_names) and roles granted to the client, per the OAUTH PL/SQL Package Reference (https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/19.4/aelig/OAUTH-reference.html).
overview: 'Oracle Database 19c uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{host}:{port}/ords/{schema}/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle Database 19c
provider_slug: oracle-database-19c
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{host}:{port}/ords/{schema}/oauth/token
  name: oauth2
  source: openapi/oracle-database-19c-ords-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: oracle-database-19c-scopes
source_filename: oracle-database-19c-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-database-19c-ords-openapi.yml\ndocs: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/19.4/aelig/OAUTH-reference.html\nnote: >-\n  ORDS OAuth 2.0 does not use named scopes; access for OAuth clients is\n  controlled through ORDS privileges (p_privilege_names) and roles granted to\n  the client, per the OAUTH PL/SQL Package Reference\n  (https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/19.4/aelig/OAUTH-reference.html).\nschemes:\n- name: oauth2\n  source: openapi/oracle-database-19c-ords-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{host}:{port}/ords/{schema}/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-database-19c/refs/heads/main/scopes/oracle-database-19c-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Database
- Enterprise
- Json
- Machine-Learning
- Nosql
- Oracle
- Rest
- Sql
token_urls:
- https://{host}:{port}/ords/{schema}/oauth/token
---
