---
api_specs:
- filename: phraseanet-account-api-openapi.yml
  format: yaml
  label: Phraseanet Account API
  slug: phraseanet-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-account-api-openapi.yml
- filename: phraseanet-baskets-api-openapi.yml
  format: yaml
  label: Phraseanet Baskets API
  slug: phraseanet-baskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-baskets-api-openapi.yml
- filename: phraseanet-databoxes-api-openapi.yml
  format: yaml
  label: Phraseanet Databoxes API
  slug: phraseanet-databoxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-databoxes-api-openapi.yml
- filename: phraseanet-feeds-api-openapi.yml
  format: yaml
  label: Phraseanet Feeds API
  slug: phraseanet-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-feeds-api-openapi.yml
- filename: phraseanet-metadata-api-openapi.yml
  format: yaml
  label: Phraseanet Metadata API
  slug: phraseanet-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-metadata-api-openapi.yml
- filename: phraseanet-quarantine-api-openapi.yml
  format: yaml
  label: Phraseanet Quarantine API
  slug: phraseanet-quarantine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-quarantine-api-openapi.yml
- filename: phraseanet-records-api-openapi.yml
  format: yaml
  label: Phraseanet Records API
  slug: phraseanet-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-records-api-openapi.yml
- filename: phraseanet-search-api-openapi.yml
  format: yaml
  label: Phraseanet Search API
  slug: phraseanet-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-search-api-openapi.yml
- filename: phraseanet-stories-api-openapi.yml
  format: yaml
  label: Phraseanet Stories API
  slug: phraseanet-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-stories-api-openapi.yml
authorization_urls:
- https://your-phraseanet-instance/api/oauthv2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Phraseanet Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Phraseanet uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://your-phraseanet-instance/api/oauthv2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Phraseanet
provider_slug: phraseanet
schemes:
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-account-api-openapi.yml
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-baskets-api-openapi.yml
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-databoxes-api-openapi.yml
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-feeds-api-openapi.yml
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-metadata-api-openapi.yml
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-quarantine-api-openapi.yml
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-records-api-openapi.yml
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-search-api-openapi.yml
- description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.
  flows:
  - authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize
    flow: authorizationCode
    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token
  name: oauth2
  source: openapi/phraseanet-stories-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: phraseanet-scopes
source_filename: phraseanet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/phraseanet-account-api-openapi.yml, openapi/phraseanet-baskets-api-openapi.yml,\n  openapi/phraseanet-databoxes-api-openapi.yml, openapi/phraseanet-feeds-api-openapi.yml, openapi/phraseanet-metadata-api-openapi.yml,\n  openapi/phraseanet-quarantine-api-openapi.yml, openapi/phraseanet-records-api-openapi.yml,\n  openapi/phraseanet-search-api-openapi.yml, openapi/phraseanet-stories-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/phraseanet-account-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n- name: oauth2\n  source: openapi/phraseanet-baskets-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n\
  \    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n- name: oauth2\n  source: openapi/phraseanet-databoxes-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n- name: oauth2\n  source: openapi/phraseanet-feeds-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n- name: oauth2\n  source: openapi/phraseanet-metadata-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n\
  \    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n- name: oauth2\n  source: openapi/phraseanet-quarantine-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n- name: oauth2\n  source: openapi/phraseanet-records-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n- name: oauth2\n  source: openapi/phraseanet-search-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n\
  \    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\n- name: oauth2\n  source: openapi/phraseanet-stories-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/scopes/phraseanet-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Digital Asset Management
- Media
- Metadata
- Open Source
- Search
token_bound: false
token_urls:
- https://your-phraseanet-instance/api/oauthv2/token
---
