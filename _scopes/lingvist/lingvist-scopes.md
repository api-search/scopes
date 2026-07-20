---
authorization_urls:
- https://learn.lingvist.com/#sso
description: ''
docs: https://github.com/lingvist/nodebb-plugin-sso-lingvist
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lingvist Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lingvist publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lingvist API on a user''s behalf.


  Tokens are issued from https://api.lingvist.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lingvist
provider_slug: lingvist
schemes:
- flows:
  - authorizationUrl: https://learn.lingvist.com/#sso
    flow: authorizationCode
    tokenUrl: https://api.lingvist.com/oauth2/token
  name: LingvistOAuth2
  source: https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/library.js
scope_count: 1
scope_names:
- auth
scopes:
- description: Authenticate the Lingvist user and read their profile from https://api.lingvist.com/1.0/user/profile (used for single sign-on).
  flows:
  - authorizationCode
  scope: auth
slug: lingvist-scopes
source_filename: lingvist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/library.js\ndocs: https://github.com/lingvist/nodebb-plugin-sso-lingvist\nnotes: >-\n  Lingvist publishes no scopes/permissions reference page. The single scope below\n  is the one Lingvist's own SSO plugin requests (`constants.scope = 'auth'`).\n  There is no OIDC discovery document and no OpenAPI to derive further scopes\n  from, so this list is what is verifiably published — not necessarily the full\n  scope surface of the internal API.\nschemes:\n- name: LingvistOAuth2\n  source: https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/library.js\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://learn.lingvist.com/#sso\n    tokenUrl: https://api.lingvist.com/oauth2/token\nscopes:\n- scope: auth\n  description: >-\n    Authenticate the Lingvist user and read their profile from\n    https://api.lingvist.com/1.0/user/profile (used\
  \ for single sign-on).\n  flows:\n  - authorizationCode\n  sources:\n  - https://github.com/lingvist/nodebb-plugin-sso-lingvist/blob/master/library.js\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingvist/refs/heads/main/scopes/lingvist-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Education
- Language Learning
- EdTech
- Artificial Intelligence
- Machine Learning
- Spaced Repetition
- Mobile
- Estonia
- Consumer
token_urls:
- https://api.lingvist.com/oauth2/token
---
