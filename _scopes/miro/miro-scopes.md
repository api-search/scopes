---
authorization_urls:
- https://miro.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Miro Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Miro publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Miro API on a user''s behalf.


  Tokens are issued from https://api.miro.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Miro
provider_slug: miro
schemes:
- description: For more information, see https://developers.miro.com/reference/authorization-flow-for-expiring-tokens
  flows:
  - authorizationUrl: https://miro.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.miro.com/v1/oauth/token
  name: oAuth2AuthCode
  source: openapi/miro-openapi.json
scope_count: 8
scope_names:
- boards:read
- boards:write
- microphone:listen
- organizations:read
- organizations:teams:read
- organizations:teams:write
- screen:record
- webcam:record
scopes:
- description: Retrieve information about boards, board members, or items
  flows:
  - authorizationCode
  scope: boards:read
- description: Create, update, or delete boards, board members, or items
  flows:
  - authorizationCode
  scope: boards:write
- description: Access a user's microphone to record audio in an iFrame
  flows:
  - authorizationCode
  scope: microphone:listen
- description: Read information about the organization, such as name, plan, number of licenses, organization settings, or organization members.
  flows:
  - authorizationCode
  scope: organizations:read
- description: Read team information, such as the list of teams, team settings, team members, for an organization.
  flows:
  - authorizationCode
  scope: organizations:teams:read
- description: Create or delete teams, update team information, team settings, team members, for an organization.
  flows:
  - authorizationCode
  scope: organizations:teams:write
- description: Access a user's screen to record it in an iFrame
  flows:
  - authorizationCode
  scope: screen:record
- description: Allows an iFrame to access a user's camera to record video
  flows:
  - authorizationCode
  scope: webcam:record
slug: miro-scopes
source_filename: miro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/miro-openapi.json\nschemes:\n- name: oAuth2AuthCode\n  source: openapi/miro-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://miro.com/oauth/authorize\n    tokenUrl: https://api.miro.com/v1/oauth/token\n  description: For more information, see https://developers.miro.com/reference/authorization-flow-for-expiring-tokens\nscopes:\n- scope: boards:read\n  description: Retrieve information about boards, board members, or items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/miro-openapi.json\n- scope: boards:write\n  description: Create, update, or delete boards, board members, or items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/miro-openapi.json\n- scope: microphone:listen\n  description: Access a user's microphone to record audio in an iFrame\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/miro-openapi.json\n- scope: organizations:read\n  description:\
  \ Read information about the organization, such as name, plan, number of licenses,\n    organization settings, or organization members.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/miro-openapi.json\n- scope: organizations:teams:read\n  description: Read team information, such as the list of teams, team settings, team members,\n    for an organization.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/miro-openapi.json\n- scope: organizations:teams:write\n  description: Create or delete teams, update team information, team settings, team members,\n    for an organization.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/miro-openapi.json\n- scope: screen:record\n  description: Access a user's screen to record it in an iFrame\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/miro-openapi.json\n- scope: webcam:record\n  description: Allows an iFrame to access a user's camera to record video\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/miro-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/scopes/miro-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Productivity
- Whiteboard
- Visual Collaboration
- Diagramming
- SaaS
token_urls:
- https://api.miro.com/v1/oauth/token
---
