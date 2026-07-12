---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Microcks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microcks publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microcks API on a user''s behalf.


  Tokens are issued from https://keycloak.example.com/realms/microcks/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microcks
provider_slug: microcks
schemes:
- description: JWT Bearer acquired using OAuth 2 Authentication flow or Direct Access Grant
  flows:
  - flow: clientCredentials
    tokenUrl: https://keycloak.example.com/realms/microcks/protocol/openid-connect/token
  name: jwt-bearer
  source: openapi/microcks-openapi.yml
scope_count: 3
scope_names:
- admin
- manager
- user
scopes:
- description: Administrator of the Microcks instance
  flows:
  - clientCredentials
  scope: admin
- description: Services & APIs content manager
  flows:
  - clientCredentials
  scope: manager
- description: Simple authenticated user
  flows:
  - clientCredentials
  scope: user
slug: microcks-scopes
source_filename: microcks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microcks-openapi.yml\nschemes:\n- name: jwt-bearer\n  source: openapi/microcks-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://keycloak.example.com/realms/microcks/protocol/openid-connect/token\n  description: JWT Bearer acquired using OAuth 2 Authentication flow or Direct Access Grant\nscopes:\n- scope: admin\n  description: Administrator of the Microcks instance\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microcks-openapi.yml\n- scope: manager\n  description: Services & APIs content manager\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microcks-openapi.yml\n- scope: user\n  description: Simple authenticated user\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microcks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microcks/refs/heads/main/scopes/microcks-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- API Testing
- Cloud Native
- DevOps
- Mocking
- Open Source
token_urls:
- https://keycloak.example.com/realms/microcks/protocol/openid-connect/token
---
