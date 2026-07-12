---
authorization_urls: []
description: ''
docs: https://www.learnworlds.dev/docs/api/b6b6c2d4906e9-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Learnworlds Scopes
name_suffix: OAuth Scopes
note: LearnWorlds API uses the OAuth2 client credentials grant (plus an Lw-Client header) and does not publish or use OAuth scopes; access is governed by school plan and API credentials (see https://www.learnworlds.dev/docs/api/b6b6c2d4906e9-authentication).
overview: 'LearnWorlds uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://yourschool.learnworlds.com/admin/api/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LearnWorlds
provider_slug: learnworlds
schemes:
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  source: openapi/learnworlds-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: learnworlds-scopes
source_filename: learnworlds-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/learnworlds-openapi.yml\ndocs: https://www.learnworlds.dev/docs/api/b6b6c2d4906e9-authentication\nnote: LearnWorlds API uses the OAuth2 client credentials grant (plus an Lw-Client\n  header) and does not publish or use OAuth scopes; access is governed by school\n  plan and API credentials (see https://www.learnworlds.dev/docs/api/b6b6c2d4906e9-authentication).\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/learnworlds-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it as Authorization: Bearer\n    ACCESS_TOKEN.'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/scopes/learnworlds-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Online Courses
- LMS
- eLearning
- Education
- Course Platform
- Creator Economy
token_urls:
- https://yourschool.learnworlds.com/admin/api/oauth2/access_token
---
