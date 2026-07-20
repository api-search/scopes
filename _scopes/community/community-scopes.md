---
api_specs:
- filename: community-async-openapi-original.yml
  format: yaml
  label: Community Async REST API
  slug: community-async-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-async-openapi-original.yml
authorization_urls:
- https://oauth-login.community.com/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Community Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Community uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Community
provider_slug: community
schemes:
- flows:
  - authorizationUrl: https://oauth-login.community.com/
    flow: authorizationCode
    tokenUrl: /oauth/v1/token
  name: oAuth
  source: openapi/community-async-openapi-original.yml
scope_count: 0
scope_names: []
scopes: []
slug: community-scopes
source_filename: community-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/community-async-openapi-original.yml\nschemes:\n- name: oAuth\n  source: openapi/community-async-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-login.community.com/\n    tokenUrl: /oauth/v1/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/scopes/community-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Messaging
- SMS
- Communications
- Conversational
- Marketing
- Creators
- Webhooks
- Company
token_urls:
- /oauth/v1/token
---
