---
authorization_urls:
- https://identity.oraclecloud.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Oracle Primavera Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Oracle Primavera publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Oracle Primavera API on a user''s behalf.


  Tokens are issued from https://identity.oraclecloud.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle Primavera
provider_slug: oracle-primavera
schemes:
- description: Oracle Identity Cloud Service OAuth2
  flows:
  - authorizationUrl: https://identity.oraclecloud.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token
  name: oauth2
  source: openapi/oracle-primavera-p6-eppm-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to P6 data
  flows:
  - authorizationCode
  scope: read
- description: Write access to P6 data
  flows:
  - authorizationCode
  scope: write
slug: oracle-primavera-scopes
source_filename: oracle-primavera-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-primavera-p6-eppm-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/oracle-primavera-p6-eppm-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.oraclecloud.com/oauth2/v1/authorize\n    tokenUrl: https://identity.oraclecloud.com/oauth2/v1/token\n  description: Oracle Identity Cloud Service OAuth2\nscopes:\n- scope: read\n  description: Read access to P6 data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oracle-primavera-p6-eppm-openapi.yml\n- scope: write\n  description: Write access to P6 data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/oracle-primavera-p6-eppm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-primavera/refs/heads/main/scopes/oracle-primavera-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Construction
- Engineering
- Project Management
- Scheduling
- Portfolio Management
- Oracle
token_urls:
- https://identity.oraclecloud.com/oauth2/v1/token
---
