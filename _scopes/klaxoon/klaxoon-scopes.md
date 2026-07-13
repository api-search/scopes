---
api_specs:
- filename: klaxoon-openapi.yml
  format: yaml
  label: Klaxoon API
  slug: klaxoon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaxoon/refs/heads/main/openapi/klaxoon-openapi.yml
authorization_urls:
- https://access.klaxoon.com/auth
description: ''
docs: https://developers.klaxoon.com/klaxoon/docs/scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Klaxoon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Klaxoon publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Klaxoon API on a user''s behalf.


  Tokens are issued from https://access.klaxoon.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Klaxoon
provider_slug: klaxoon
schemes:
- description: OAuth 2.0 authorization-code flow against Klaxoon. Scopes are issued per integration via the Klaxoon developer portal.
  flows:
  - authorizationUrl: https://access.klaxoon.com/auth
    flow: authorizationCode
    tokenUrl: https://access.klaxoon.com/token
  name: OAuth2
  source: openapi/klaxoon-openapi.yml
scope_count: 10
scope_names:
- identity:read
- auditlog:read
- board:read
- board:write
- quiz:read
- survey:read
- memo:read
- adventure:read
- mission:read
- session:read
scopes:
- description: View profile informations of the authenticated user (email, first name, last name).
  flows: []
  scope: identity:read
- description: 'Read Audit Logs for an organization. Note: the authenticated user authorizing your application must have a Company Admin role within the organization for full access to the Company Audit Logs.'
  flows: []
  scope: auditlog:read
- description: Read Boards and Board content of a Klaxoon user.
  flows: []
  scope: board:read
- description: Create and modify Boards and Board content of a Klaxoon user.
  flows: []
  scope: board:write
- description: Get the list of Quizzes of a Klaxoon user and informations on Quiz participants and results.
  flows: []
  scope: quiz:read
- description: Get the list of Surveys of a Klaxoon user and informations on Survey participants and results.
  flows: []
  scope: survey:read
- description: Get the list of Memos of a Klaxoon user and informations on Memo participants and results.
  flows: []
  scope: memo:read
- description: Get the list of Adventures of a Klaxoon user and informations on Adventure participants and results.
  flows: []
  scope: adventure:read
- description: Get the list of Missions of a Klaxoon user and informations on Mission participants and results.
  flows: []
  scope: mission:read
- description: Get the list of Sessions of a Klaxoon user and informations on Session participants and results.
  flows: []
  scope: session:read
slug: klaxoon-scopes
source_filename: klaxoon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/klaxoon-openapi.yml\ndocs: https://developers.klaxoon.com/klaxoon/docs/scopes\nschemes:\n- name: OAuth2\n  source: openapi/klaxoon-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://access.klaxoon.com/auth\n    tokenUrl: https://access.klaxoon.com/token\n  description: OAuth 2.0 authorization-code flow against Klaxoon. Scopes are issued per integration\n    via the Klaxoon developer portal.\nscopes:\n- scope: identity:read\n  description: View profile informations of the authenticated user (email, first\n    name, last name).\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n- scope: auditlog:read\n  description: 'Read Audit Logs for an organization. Note: the authenticated user\n    authorizing your application must have a Company Admin role within the organization\n    for full access to the Company Audit Logs.'\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n\
  - scope: board:read\n  description: Read Boards and Board content of a Klaxoon user.\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n- scope: board:write\n  description: Create and modify Boards and Board content of a Klaxoon user.\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n- scope: quiz:read\n  description: Get the list of Quizzes of a Klaxoon user and informations on Quiz\n    participants and results.\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n- scope: survey:read\n  description: Get the list of Surveys of a Klaxoon user and informations on Survey\n    participants and results.\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n- scope: memo:read\n  description: Get the list of Memos of a Klaxoon user and informations on Memo participants\n    and results.\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n- scope: adventure:read\n  description: Get the list of Adventures of\
  \ a Klaxoon user and informations on Adventure\n    participants and results.\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n- scope: mission:read\n  description: Get the list of Missions of a Klaxoon user and informations on Mission\n    participants and results.\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n- scope: session:read\n  description: Get the list of Sessions of a Klaxoon user and informations on Session\n    participants and results.\n  sources:\n  - https://developers.klaxoon.com/klaxoon/docs/scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaxoon/refs/heads/main/scopes/klaxoon-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Collaboration
- Meetings
- Productivity
- Team Collaboration
- Workshops
- Brainstorming
- Whiteboard
token_urls:
- https://access.klaxoon.com/token
---
