---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Oracle Transportation Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Oracle Transportation Management publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Oracle Transportation Management API on a user''s behalf.


  Tokens are issued from https://login.oracle.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle Transportation Management
provider_slug: oracle-transportation-management
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.oracle.com/oauth2/v1/token
  name: oauth2
  source: openapi/oracle-otm-business-objects-openapi.yml
scope_count: 2
scope_names:
- otm.read
- otm.write
scopes:
- description: Read OTM data
  flows:
  - clientCredentials
  scope: otm.read
- description: Write OTM data
  flows:
  - clientCredentials
  scope: otm.write
slug: oracle-transportation-management-scopes
source_filename: oracle-transportation-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-otm-business-objects-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/oracle-otm-business-objects-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.oracle.com/oauth2/v1/token\nscopes:\n- scope: otm.read\n  description: Read OTM data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oracle-otm-business-objects-openapi.yml\n- scope: otm.write\n  description: Write OTM data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/oracle-otm-business-objects-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-transportation-management/refs/heads/main/scopes/oracle-transportation-management-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Logistics
- Transportation
- Freight
- Supply Chain
- Shipping
- Global Trade
- Oracle
token_urls:
- https://login.oracle.com/oauth2/v1/token
---
