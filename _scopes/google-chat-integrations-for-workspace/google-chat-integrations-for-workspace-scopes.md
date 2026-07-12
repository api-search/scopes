---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Chat Integrations For Workspace Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Chat Integrations for Workspace publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Chat Integrations for Workspace API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Chat Integrations for Workspace
provider_slug: google-chat-integrations-for-workspace
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-chat-integrations-for-workspace-openapi.yml
scope_count: 3
scope_names:
- chat.memberships
- chat.messages
- chat.spaces
scopes:
- description: Manage Chat memberships
  flows:
  - authorizationCode
  scope: chat.memberships
- description: Manage Chat messages
  flows:
  - authorizationCode
  scope: chat.messages
- description: Manage Chat spaces
  flows:
  - authorizationCode
  scope: chat.spaces
slug: google-chat-integrations-for-workspace-scopes
source_filename: google-chat-integrations-for-workspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-chat-integrations-for-workspace-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-chat-integrations-for-workspace-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: chat.memberships\n  description: Manage Chat memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-openapi.yml\n- scope: chat.messages\n  description: Manage Chat messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-openapi.yml\n- scope: chat.spaces\n  description: Manage Chat spaces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chat-integrations-for-workspace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/scopes/google-chat-integrations-for-workspace-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Google Workspace
- Team Chat
- Messaging
- Collaboration
- Chat Apps
- Spaces
- Slash Commands
- Bots
token_urls:
- https://oauth2.googleapis.com/token
---
