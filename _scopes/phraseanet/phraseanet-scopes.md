---
api_specs:
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Records API
  slug: phraseanet-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Databoxes and Collections API
  slug: phraseanet-databoxes-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Metadata API
  slug: phraseanet-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Search API
  slug: phraseanet-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Stories API
  slug: phraseanet-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Baskets API
  slug: phraseanet-baskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Feeds API
  slug: phraseanet-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Account API
  slug: phraseanet-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
authorization_urls:
- https://your-phraseanet-instance/api/oauthv2/authorize
description: ''
docs: https://docs.phraseanet.com/4.1/en/Devel/API/V1/Authentication.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Phraseanet Scopes
name_suffix: OAuth Scopes
note: Phraseanet's OAuth2 does not use or document scopes - access is governed by the authenticated user's rights and collection access within the self-hosted Phraseanet instance, with application registration and user-revocable access instead of scope grants (https://docs.phraseanet.com/4.1/en/Devel/API/V1/Authentication.html).
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
  source: openapi/phraseanet-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: phraseanet-scopes
source_filename: phraseanet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/phraseanet-openapi.yml\ndocs: https://docs.phraseanet.com/4.1/en/Devel/API/V1/Authentication.html\nnote: Phraseanet's OAuth2 does not use or document scopes - access is governed by\n  the authenticated user's rights and collection access within the self-hosted\n  Phraseanet instance, with application registration and user-revocable access\n  instead of scope grants\n  (https://docs.phraseanet.com/4.1/en/Devel/API/V1/Authentication.html).\nschemes:\n- name: oauth2\n  source: openapi/phraseanet-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-phraseanet-instance/api/oauthv2/authorize\n    tokenUrl: https://your-phraseanet-instance/api/oauthv2/token\n  description: OAuth2. Register an application in Phraseanet to obtain a client id and secret.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/scopes/phraseanet-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Digital Asset Management
- DAM
- Media
- Metadata
- Open Source
- Search
token_urls:
- https://your-phraseanet-instance/api/oauthv2/token
---
