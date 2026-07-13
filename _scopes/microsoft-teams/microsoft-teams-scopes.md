---
api_specs:
- filename: microsoft-teams-graph-api.yaml
  format: yaml
  label: Microsoft Graph Teams API
  slug: microsoft-graph-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-graph-api.yaml
- filename: microsoft-teams-asyncapi.yaml
  format: yaml
  label: Microsoft Teams Bot Framework API
  slug: microsoft-teams-bot-framework-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/asyncapi/microsoft-teams-asyncapi.yaml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Teams Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Teams publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Teams API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Teams
provider_slug: microsoft-teams
schemes:
- description: OAuth 2.0 authorization using Microsoft Identity Platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-teams-graph-api.yaml
scope_count: 10
scope_names:
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- Channel.Create
- Channel.ReadBasic.All
- ChannelMessage.Read.All
- ChatMessage.Read
- ChatMessage.Send
- OnlineMeetings.ReadWrite.All
- Team.Create
- Team.ReadBasic.All
scopes:
- description: Initiate calls
  flows:
  - authorizationCode
  scope: Calls.Initiate.All
- description: Join group calls
  flows:
  - authorizationCode
  scope: Calls.JoinGroupCall.All
- description: Create channels
  flows:
  - authorizationCode
  scope: Channel.Create
- description: Read channel basic info
  flows:
  - authorizationCode
  scope: Channel.ReadBasic.All
- description: Read channel messages
  flows:
  - authorizationCode
  scope: ChannelMessage.Read.All
- description: Read chat messages
  flows:
  - authorizationCode
  scope: ChatMessage.Read
- description: Send chat messages
  flows:
  - authorizationCode
  scope: ChatMessage.Send
- description: Create and manage online meetings
  flows:
  - authorizationCode
  scope: OnlineMeetings.ReadWrite.All
- description: Create teams
  flows:
  - authorizationCode
  scope: Team.Create
- description: Read teams basic info
  flows:
  - authorizationCode
  scope: Team.ReadBasic.All
slug: microsoft-teams-scopes
source_filename: microsoft-teams-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-teams-graph-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-teams-graph-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization using Microsoft Identity Platform\nscopes:\n- scope: Calls.Initiate.All\n  description: Initiate calls\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: Calls.JoinGroupCall.All\n  description: Join group calls\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: Channel.Create\n  description: Create channels\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: Channel.ReadBasic.All\n  description: Read channel basic info\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: ChannelMessage.Read.All\n  description: Read channel messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: ChatMessage.Read\n  description: Read chat messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: ChatMessage.Send\n  description: Send chat messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: OnlineMeetings.ReadWrite.All\n  description: Create and manage online meetings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: Team.Create\n  description: Create teams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n- scope: Team.ReadBasic.All\n  description: Read teams basic info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-teams-graph-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/scopes/microsoft-teams-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
