---
api_specs:
- filename: flowdock-rest-api-openapi.yml
  format: yaml
  label: Flowdock REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-rest-api-openapi.yml
- filename: flowdock-push-api-openapi.yml
  format: yaml
  label: Flowdock Push API (Deprecated)
  slug: push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-push-api-openapi.yml
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
- Integrations
- Discontinued
token_urls:
- https://api.flowdock.com/oauth/token
---
