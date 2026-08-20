---
api_specs:
- filename: flowdock-streaming-api-asyncapi.yml
  format: yaml
  label: Flowdock Streaming API
  slug: streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/asyncapi/flowdock-streaming-api-asyncapi.yml
- filename: flowdock-scim-api-openapi.yml
  format: yaml
  label: Flowdock SCIM Provisioning API
  slug: scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-scim-api-openapi.yml
- filename: flowdock-authentication-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Authentication API
  slug: flowdock-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-authentication-api-openapi.yml
- filename: flowdock-chat-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Chat API
  slug: flowdock-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-chat-api-openapi.yml
- filename: flowdock-files-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Files API
  slug: flowdock-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-files-api-openapi.yml
- filename: flowdock-flows-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Flows API
  slug: flowdock-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-flows-api-openapi.yml
- filename: flowdock-invitations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Invitations API
  slug: flowdock-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-invitations-api-openapi.yml
- filename: flowdock-messages-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Messages API
  slug: flowdock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-messages-api-openapi.yml
- filename: flowdock-organizations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Organizations API
  slug: flowdock-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-organizations-api-openapi.yml
- filename: flowdock-private-conversations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Private Conversations API
  slug: flowdock-private-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-private-conversations-api-openapi.yml
- filename: flowdock-private-messages-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Private Messages API
  slug: flowdock-private-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-private-messages-api-openapi.yml
- filename: flowdock-sources-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Sources API
  slug: flowdock-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-sources-api-openapi.yml
- filename: flowdock-team-inbox-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Team Inbox API
  slug: flowdock-team-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-team-inbox-api-openapi.yml
- filename: flowdock-threads-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Threads API
  slug: flowdock-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-threads-api-openapi.yml
- filename: flowdock-users-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Users API
  slug: flowdock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-users-api-openapi.yml
authorization_urls:
- https://api.flowdock.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Flowdock Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flowdock (Discontinued) publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flowdock (Discontinued) API on a user''s behalf.


  Tokens are issued from https://api.flowdock.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flowdock (Discontinued)
provider_slug: flowdock
schemes:
- flows:
  - authorizationUrl: https://api.flowdock.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.flowdock.com/oauth/token
  name: oauth2
  source: openapi/flowdock-rest-api-openapi.yml
scope_count: 3
scope_names:
- flow
- private
- profile
scopes:
- description: Read and write flow content.
  flows:
  - authorizationCode
  scope: flow
- description: Read and write private conversations.
  flows:
  - authorizationCode
  scope: private
- description: Read user profile.
  flows:
  - authorizationCode
  scope: profile
slug: flowdock-scopes
source_filename: flowdock-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flowdock-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/flowdock-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.flowdock.com/oauth/authorize\n    tokenUrl: https://api.flowdock.com/oauth/token\nscopes:\n- scope: flow\n  description: Read and write flow content.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/flowdock-rest-api-openapi.yml\n- scope: private\n  description: Read and write private conversations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/flowdock-rest-api-openapi.yml\n- scope: profile\n  description: Read user profile.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/flowdock-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/scopes/flowdock-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Team Chat
- Team Inbox
- Collaboration
- Real-Time Messaging
- Integration
- Discontinued
token_urls:
- https://api.flowdock.com/oauth/token
---
