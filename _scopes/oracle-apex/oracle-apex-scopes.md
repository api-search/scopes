---
authorization_urls:
- /ords/{schema}/oauth/auth
description: ''
docs: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/25.2/orddg/OAUTH-reference.html
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Oracle Apex Scopes
name_suffix: OAuth Scopes
note: ORDS OAuth publishes no fixed scope catalog; access is granted through developer-defined ORDS privileges and roles per REST-enabled schema (OAUTH.CREATE_CLIENT p_privilege_names, OAUTH.GRANT_CLIENT_ROLE), with JWT scope claims expected to match privilege names (https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/25.2/orddg/OAUTH-reference.html).
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
  source: openapi/ords-rest-api-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: oracle-apex-scopes
source_filename: oracle-apex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ords-rest-api-openapi.json\ndocs: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/25.2/orddg/OAUTH-reference.html\nnote: ORDS OAuth publishes no fixed scope catalog; access is granted through developer-defined\n  ORDS privileges and roles per REST-enabled schema (OAUTH.CREATE_CLIENT p_privilege_names,\n  OAUTH.GRANT_CLIENT_ROLE), with JWT scope claims expected to match privilege names\n  (https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/25.2/orddg/OAUTH-reference.html).\nschemes:\n- name: oauth2\n  source: openapi/ords-rest-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\nscopes: []\n"
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
- Workflow
token_urls:
- /ords/{schema}/oauth/token
---
