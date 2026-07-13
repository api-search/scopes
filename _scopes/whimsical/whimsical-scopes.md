---
api_specs:
- filename: whimsical-openapi.yml
  format: yaml
  label: Whimsical API (Beta)
  slug: whimsical-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/openapi/whimsical-openapi.yml
authorization_urls:
- https://whimsical.com/oauth/authorize
description: ''
docs: https://whimsical.com/learn/integrations/api
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Whimsical Scopes
name_suffix: OAuth Scopes
note: Whimsical's limited-beta API uses OAuth 2.1 but publishes no scopes; credentials are issued privately by Whimsical support and no scopes/permissions reference exists (https://whimsical.com/learn/integrations/api).
overview: 'Whimsical uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://whimsical.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Whimsical
provider_slug: whimsical
schemes:
- description: OAuth 2.1 authorization (contact Whimsical support for client credentials)
  flows:
  - authorizationUrl: https://whimsical.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://whimsical.com/oauth/token
  name: OAuth2
  source: openapi/whimsical-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: whimsical-scopes
source_filename: whimsical-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whimsical-openapi.yml\ndocs: https://whimsical.com/learn/integrations/api\nnote: Whimsical's limited-beta API uses OAuth 2.1 but publishes no scopes; credentials\n  are issued privately by Whimsical support and no scopes/permissions reference exists\n  (https://whimsical.com/learn/integrations/api).\nschemes:\n- name: OAuth2\n  source: openapi/whimsical-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://whimsical.com/oauth/authorize\n    tokenUrl: https://whimsical.com/oauth/token\n  description: OAuth 2.1 authorization (contact Whimsical support for client credentials)\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whimsical/refs/heads/main/scopes/whimsical-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Collaboration
- Diagramming
- Flowcharts
- Wireframes
- Mind Maps
token_urls:
- https://whimsical.com/oauth/token
---
