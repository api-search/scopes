---
api_specs:
- filename: zenzap-agentic-api-openapi.yml
  format: yaml
  label: ZenZap Agentic API
  slug: zenzap-agentic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-agentic-api-openapi.yml
- filename: zenzap-long-polling-api-openapi.yml
  format: yaml
  label: ZenZap Long Polling API
  slug: zenzap-long-polling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-long-polling-api-openapi.yml
- filename: zenzap-members-api-openapi.yml
  format: yaml
  label: ZenZap Members API
  slug: zenzap-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-members-api-openapi.yml
- filename: zenzap-messages-api-openapi.yml
  format: yaml
  label: ZenZap Messages API
  slug: zenzap-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-messages-api-openapi.yml
- filename: zenzap-oauth-api-openapi.yml
  format: yaml
  label: ZenZap OAuth API
  slug: zenzap-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-oauth-api-openapi.yml
- filename: zenzap-polls-api-openapi.yml
  format: yaml
  label: ZenZap Polls API
  slug: zenzap-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-polls-api-openapi.yml
- filename: zenzap-tasks-api-openapi.yml
  format: yaml
  label: ZenZap Tasks API
  slug: zenzap-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-tasks-api-openapi.yml
- filename: zenzap-topics-group-chats-channels-conversations-api-openapi.yml
  format: yaml
  label: ZenZap Topics (group chats/channels/conversations) API
  slug: zenzap-topics-group-chats-channels-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-topics-group-chats-channels-conversations-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.zenzap.co/api-reference/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Zenzap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ZenZap publishes 12 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ZenZap API on a user''s behalf.


  Tokens are issued from https://api.zenzap.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ZenZap
provider_slug: zenzap
schemes:
- description: 'OAuth 2.0 `client_credentials` grant for API-key bots. Use the `clientId` and `clientSecret` returned when the bot was created (or rotated) to mint short-lived access tokens. See [Authentication](/api-reference/authentication) for details.


    Access tokens are bearer JWTs and expire after 1 hour. There is no refresh token — re-mint with the client credentials when the token expires.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.zenzap.co/oauth/token
  name: oauth2ClientCredentials
  source: openapi/zenzap-openapi-original.yml
scope_count: 12
scope_names:
- channel:list
- channel:read
- channel:write
- member:read
- message:read
- message:send
- message:write
- poll:write
- reaction:write
- task:read
- task:write
- updates:read
scopes:
- description: List topics the bot belongs to
  flows:
  - clientCredentials
  scope: channel:list
- description: Read topic metadata
  flows:
  - clientCredentials
  scope: channel:read
- description: Create/update topics and manage members
  flows:
  - clientCredentials
  scope: channel:write
- description: List organization members
  flows:
  - clientCredentials
  scope: member:read
- description: Read messages
  flows:
  - clientCredentials
  scope: message:read
- description: Send messages
  flows:
  - clientCredentials
  scope: message:send
- description: Edit / delete / mark-delivered / mark-read messages
  flows:
  - clientCredentials
  scope: message:write
- description: Create polls and cast / retract votes
  flows:
  - clientCredentials
  scope: poll:write
- description: Add and remove reactions on messages
  flows:
  - clientCredentials
  scope: reaction:write
- description: Read tasks
  flows:
  - clientCredentials
  scope: task:read
- description: Create / update / delete tasks
  flows:
  - clientCredentials
  scope: task:write
- description: Long-poll for outbound events
  flows:
  - clientCredentials
  scope: updates:read
slug: zenzap-scopes
source_filename: zenzap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/zenzap-openapi-original.yml\ndocs: https://docs.zenzap.co/api-reference/authentication\nnotes: >-\n  Scopes are documented on the Authentication page and passed as a\n  space-separated subset to POST /oauth/token. Each endpoint requires a\n  specific scope.\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/zenzap-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.zenzap.co/oauth/token\n  description: |-\n    OAuth 2.0 `client_credentials` grant for API-key bots. Use the `clientId` and `clientSecret` returned when the bot was created (or rotated) to mint short-lived access tokens. See [Authentication](/api-reference/authentication) for details.\n\n    Access tokens are bearer JWTs and expire after 1 hour. There is no refresh token — re-mint with the client credentials when the token expires.\nscopes:\n- scope: channel:list\n  description: List topics the bot belongs to\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: channel:read\n  description: Read topic metadata\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: channel:write\n  description: Create/update topics and manage members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: member:read\n  description: List organization members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: message:read\n  description: Read messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: message:send\n  description: Send messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: message:write\n  description: Edit / delete / mark-delivered / mark-read messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n\
  - scope: poll:write\n  description: Create polls and cast / retract votes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: reaction:write\n  description: Add and remove reactions on messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: task:read\n  description: Read tasks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: task:write\n  description: Create / update / delete tasks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n- scope: updates:read\n  description: Long-poll for outbound events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zenzap-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/scopes/zenzap-scopes.yml
summary_line: 12 scopes · clientCredentials
tags:
- Company
- Ai Ml
- Messaging
- Team Communication
- Collaboration
- Chat
- Bots
- Webhooks
- Productivity
- Tasks
token_urls:
- https://api.zenzap.co/oauth/token
---
