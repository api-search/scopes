---
authorization_urls: []
description: ''
docs: https://developer.helpscout.com/mailbox-api/overview/authentication/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Helpscout Scopes
name_suffix: OAuth Scopes
note: Help Scout's Mailbox API OAuth 2.0 (authorization code and client credentials flows) does not define or document any OAuth scopes; access is governed by the authorizing user's Help Scout account permissions (https://developer.helpscout.com/mailbox-api/overview/authentication/).
overview: 'Help Scout uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.helpscout.net/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Help Scout
provider_slug: helpscout
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: helpscout-scopes
source_filename: helpscout-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/helpscout-openapi.yml\ndocs: https://developer.helpscout.com/mailbox-api/overview/authentication/\nnote: Help Scout's Mailbox API OAuth 2.0 (authorization code and client credentials\n  flows) does not define or document any OAuth scopes; access is governed by the\n  authorizing user's Help Scout account permissions (https://developer.helpscout.com/mailbox-api/overview/authentication/).\nschemes:\n- name: oauth2\n  source: openapi/helpscout-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/scopes/helpscout-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Customer Support
- Help Desk
- Email
- Live Chat
- Knowledge Base
- SaaS
token_urls:
- https://api.helpscout.net/v2/oauth2/token
---
