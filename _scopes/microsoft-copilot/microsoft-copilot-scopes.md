---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Copilot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Copilot publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Copilot API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schemes:
- description: OAuth 2.0 authorization using Microsoft identity platform (Azure AD). Requires a Microsoft 365 Copilot license for each user accessing Copilot API functionality.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-copilot-openapi.yml
scope_count: 5
scope_names:
- AIInteraction.Read.All
- Chat.Read
- ExternalItem.Read.All
- Files.Read.All
- Sites.Read.All
scopes:
- description: Read all AI interactions for compliance
  flows:
  - authorizationCode
  scope: AIInteraction.Read.All
- description: Read user chat messages
  flows:
  - authorizationCode
  scope: Chat.Read
- description: Read external items from Copilot connectors
  flows:
  - authorizationCode
  scope: ExternalItem.Read.All
- description: Read all files the user can access
  flows:
  - authorizationCode
  scope: Files.Read.All
- description: Read items in all site collections
  flows:
  - authorizationCode
  scope: Sites.Read.All
slug: microsoft-copilot-scopes
source_filename: microsoft-copilot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-copilot-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-copilot-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: OAuth 2.0 authorization using Microsoft identity platform (Azure AD). Requires\n    a Microsoft 365 Copilot license for each user accessing Copilot API functionality.\nscopes:\n- scope: AIInteraction.Read.All\n  description: Read all AI interactions for compliance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-copilot-openapi.yml\n- scope: Chat.Read\n  description: Read user chat messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-copilot-openapi.yml\n- scope: ExternalItem.Read.All\n  description: Read external items from Copilot connectors\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/microsoft-copilot-openapi.yml\n- scope: Files.Read.All\n  description: Read all files the user can access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-copilot-openapi.yml\n- scope: Sites.Read.All\n  description: Read items in all site collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-copilot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/scopes/microsoft-copilot-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft 365
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
