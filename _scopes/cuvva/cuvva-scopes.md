---
authorization_urls: []
description: ''
docs: https://github.com/cuvva/docs/blob/master/apis/auth.md
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Cuvva Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cuvva publishes 1 OAuth 2.0 scope via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cuvva API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cuvva
provider_slug: cuvva
schemes:
- flows:
  - flow: authorizationCode
  - flow: refreshToken
  name: OAuth2
  source: https://github.com/cuvva/docs/blob/master/apis/auth.md
scope_count: 1
scope_names:
- self:official_app
scopes:
- description: Audience "self" (the acting user) with the official-app permission — the scope granted to Cuvva's own first-party mobile apps, observed in the authenticate response example.
  flows:
  - authorizationCode
  - refreshToken
  scope: self:official_app
slug: cuvva-scopes
source_filename: cuvva-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/cuvva/docs/blob/master/apis/auth.md\ndocs: https://github.com/cuvva/docs/blob/master/apis/auth.md\nmodel: >-\n  Cuvva's OAuth 2.0 implementation issues scoped access/refresh tokens. Scopes\n  follow an \"<audience>:<permission>\" naming convention. Scopes are optional on\n  refresh/authenticate; when omitted the scopes of the passed-in refresh token are\n  inherited. Only scopes observed verbatim in the public auth docs are recorded\n  here — Cuvva does not publish a complete scope reference.\nschemes:\n  - name: OAuth2\n    source: https://github.com/cuvva/docs/blob/master/apis/auth.md\n    flows:\n      - flow: authorizationCode\n      - flow: refreshToken\nscopes:\n  - scope: \"self:official_app\"\n    description: >-\n      Audience \"self\" (the acting user) with the official-app permission — the\n      scope granted to Cuvva's own first-party mobile apps, observed in the\n      authenticate response\
  \ example.\n    flows: [authorizationCode, refreshToken]\n    sources: [https://github.com/cuvva/docs/blob/master/apis/auth.md]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuvva/refs/heads/main/scopes/cuvva-scopes.yml
summary_line: 1 scope · authorizationCode/refreshToken
tags:
- Company
- Insurance
- Insurtech
- Car Insurance
- Financial Services
- Mobile
- OAuth
- United Kingdom
token_urls: []
---
