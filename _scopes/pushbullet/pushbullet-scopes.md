---
api_specs:
- filename: pushbullet-asyncapi.yml
  format: yaml
  label: Pushbullet Realtime Event Stream
  slug: realtime-event-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-asyncapi.yml
- filename: pushbullet-channels-api-openapi.yml
  format: yaml
  label: Pushbullet Channels API
  slug: pushbullet-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-channels-api-openapi.yml
- filename: pushbullet-chats-api-openapi.yml
  format: yaml
  label: Pushbullet Chats API
  slug: pushbullet-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-chats-api-openapi.yml
- filename: pushbullet-devices-api-openapi.yml
  format: yaml
  label: Pushbullet Devices API
  slug: pushbullet-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-devices-api-openapi.yml
- filename: pushbullet-ephemerals-api-openapi.yml
  format: yaml
  label: Pushbullet Ephemerals API
  slug: pushbullet-ephemerals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-ephemerals-api-openapi.yml
- filename: pushbullet-pushes-api-openapi.yml
  format: yaml
  label: Pushbullet Pushes API
  slug: pushbullet-pushes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-pushes-api-openapi.yml
- filename: pushbullet-subscriptions-api-openapi.yml
  format: yaml
  label: Pushbullet Subscriptions API
  slug: pushbullet-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-subscriptions-api-openapi.yml
- filename: pushbullet-texts-api-openapi.yml
  format: yaml
  label: Pushbullet Texts API
  slug: pushbullet-texts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-texts-api-openapi.yml
- filename: pushbullet-upload-api-openapi.yml
  format: yaml
  label: Pushbullet Upload API
  slug: pushbullet-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-upload-api-openapi.yml
- filename: pushbullet-users-api-openapi.yml
  format: yaml
  label: Pushbullet Users API
  slug: pushbullet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-users-api-openapi.yml
authorization_urls:
- https://www.pushbullet.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Pushbullet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pushbullet publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pushbullet API on a user''s behalf.


  Tokens are issued from https://api.pushbullet.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pushbullet
provider_slug: pushbullet
schemes:
- description: OAuth 2.0 for third-party applications.
  flows:
  - authorizationUrl: https://www.pushbullet.com/authorize
    flow: authorizationCode
    tokenUrl: https://api.pushbullet.com/oauth2/token
  name: oauth2
  source: openapi/pushbullet-openapi.yml
scope_count: 1
scope_names:
- everything
scopes:
- description: Full access
  flows:
  - authorizationCode
  scope: everything
slug: pushbullet-scopes
source_filename: pushbullet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pushbullet-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/pushbullet-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.pushbullet.com/authorize\n    tokenUrl: https://api.pushbullet.com/oauth2/token\n  description: OAuth 2.0 for third-party applications.\nscopes:\n- scope: everything\n  description: Full access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pushbullet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/scopes/pushbullet-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Notifications
- Messaging
- Push Notifications
- Device Sync
- SMS
- File Transfer
token_urls:
- https://api.pushbullet.com/oauth2/token
---
