---
authorization_urls: []
description: ''
docs: https://www.mongodb.com/docs/atlas/api/api-authentication/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Mongodb Scopes
name_suffix: OAuth Scopes
note: MongoDB Atlas Service Accounts use the OAuth 2.0 client_credentials flow without scopes; permissions are governed by Atlas roles assigned to the service account (https://www.mongodb.com/docs/atlas/api/api-authentication/).
overview: 'MongoDB uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://cloud.mongodb.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MongoDB
provider_slug: mongodb
schemes:
- description: Learn more about [Service Accounts](https://www.mongodb.com/docs/atlas/api/service-accounts-overview).
  flows:
  - flow: clientCredentials
    tokenUrl: https://cloud.mongodb.com/api/oauth/token
  name: ServiceAccounts
  source: openapi/mongodb-atlas-openapi.yaml
scope_count: 0
scope_names: []
scopes: []
slug: mongodb-scopes
source_filename: mongodb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mongodb-atlas-openapi.yaml\ndocs: https://www.mongodb.com/docs/atlas/api/api-authentication/\nnote: MongoDB Atlas Service Accounts use the OAuth 2.0 client_credentials flow without\n  scopes; permissions are governed by Atlas roles assigned to the service account\n  (https://www.mongodb.com/docs/atlas/api/api-authentication/).\nschemes:\n- name: ServiceAccounts\n  source: openapi/mongodb-atlas-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cloud.mongodb.com/api/oauth/token\n  description: Learn more about [Service Accounts](https://www.mongodb.com/docs/atlas/api/service-accounts-overview).\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mongodb/refs/heads/main/scopes/mongodb-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Cloud Database
- Database
- Document Database
- NoSQL
token_urls:
- https://cloud.mongodb.com/api/oauth/token
---
