---
api_specs:
- filename: helpscout-conversations-api-openapi.yml
  format: yaml
  label: Help Scout Conversations API
  slug: helpscout-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-conversations-api-openapi.yml
- filename: helpscout-customers-api-openapi.yml
  format: yaml
  label: Help Scout Customers API
  slug: helpscout-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-customers-api-openapi.yml
- filename: helpscout-mailboxes-api-openapi.yml
  format: yaml
  label: Help Scout Mailboxes API
  slug: helpscout-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-mailboxes-api-openapi.yml
- filename: helpscout-tags-api-openapi.yml
  format: yaml
  label: Help Scout Tags API
  slug: helpscout-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-tags-api-openapi.yml
- filename: helpscout-teams-api-openapi.yml
  format: yaml
  label: Help Scout Teams API
  slug: helpscout-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-teams-api-openapi.yml
- filename: helpscout-threads-api-openapi.yml
  format: yaml
  label: Help Scout Threads API
  slug: helpscout-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-threads-api-openapi.yml
- filename: helpscout-users-api-openapi.yml
  format: yaml
  label: Help Scout Users API
  slug: helpscout-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-users-api-openapi.yml
- filename: helpscout-webhooks-api-openapi.yml
  format: yaml
  label: Help Scout Webhooks API
  slug: helpscout-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-webhooks-api-openapi.yml
- filename: helpscout-workflows-api-openapi.yml
  format: yaml
  label: Help Scout Workflows API
  slug: helpscout-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/openapi/helpscout-workflows-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Helpscout Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
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
  source: openapi/helpscout-conversations-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-customers-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-mailboxes-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-tags-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-teams-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-threads-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-users-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-webhooks-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.helpscout.net/v2/oauth2/token
  name: oauth2
  source: openapi/helpscout-workflows-api-openapi.yml
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
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/helpscout-conversations-api-openapi.yml, openapi/helpscout-customers-api-openapi.yml,\n  openapi/helpscout-mailboxes-api-openapi.yml, openapi/helpscout-openapi.yml, openapi/helpscout-tags-api-openapi.yml,\n  openapi/helpscout-teams-api-openapi.yml, openapi/helpscout-threads-api-openapi.yml, openapi/helpscout-users-api-openapi.yml,\n  openapi/helpscout-webhooks-api-openapi.yml, openapi/helpscout-workflows-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/helpscout-conversations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n- name: oauth2\n  source: openapi/helpscout-customers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n- name: oauth2\n  source: openapi/helpscout-mailboxes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n\
  - name: oauth2\n  source: openapi/helpscout-tags-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n- name: oauth2\n  source: openapi/helpscout-teams-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n- name: oauth2\n  source: openapi/helpscout-threads-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n- name: oauth2\n  source: openapi/helpscout-users-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n- name: oauth2\n  source: openapi/helpscout-webhooks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n- name: oauth2\n  source: openapi/helpscout-workflows-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\n- name: oauth2\n\
  \  source: openapi/helpscout-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.helpscout.net/v2/oauth2/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helpscout/refs/heads/main/scopes/helpscout-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Customer Service
- Help Desk
- Email
- Live Chat
- Knowledge Base
- Software-as-a-Service
token_bound: false
token_urls:
- https://api.helpscout.net/v2/oauth2/token
---
