---
api_specs:
- filename: beeper-accounts-api-openapi.yml
  format: yaml
  label: Beeper Accounts API
  slug: beeper-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-accounts-api-openapi.yml
- filename: beeper-app-api-openapi.yml
  format: yaml
  label: Beeper App API
  slug: beeper-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-app-api-openapi.yml
- filename: beeper-chats-api-openapi.yml
  format: yaml
  label: Beeper Chats API
  slug: beeper-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-chats-api-openapi.yml
- filename: beeper-contacts-api-openapi.yml
  format: yaml
  label: Beeper Contacts API
  slug: beeper-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-contacts-api-openapi.yml
- filename: beeper-files-api-openapi.yml
  format: yaml
  label: Beeper Files API
  slug: beeper-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-files-api-openapi.yml
- filename: beeper-messages-api-openapi.yml
  format: yaml
  label: Beeper Messages API
  slug: beeper-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-messages-api-openapi.yml
- filename: beeper-server-api-openapi.yml
  format: yaml
  label: Beeper Server API
  slug: beeper-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-server-api-openapi.yml
authorization_urls:
- http://localhost:23373/oauth/authorize
description: ''
docs: https://developers.beeper.com/desktop-api/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Beeper Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beeper publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beeper API on a user''s behalf.


  Tokens are issued from http://localhost:23373/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beeper
provider_slug: beeper
schemes:
- description: OAuth2 Authorization Code flow with PKCE for obtaining bearer access tokens. Used by MCP servers to authenticate clients.
  flows:
  - authorizationUrl: http://localhost:23373/oauth/authorize
    flow: authorizationCode
    tokenUrl: http://localhost:23373/oauth/token
  name: oauth2
  source: openapi/beeper-desktop-api-openapi-original.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to messages, chats, and accounts
  flows:
  - authorizationCode
  scope: read
- description: Write access to send messages, edit messages, react to messages, archive chats, and set reminders
  flows:
  - authorizationCode
  scope: write
slug: beeper-scopes
source_filename: beeper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/beeper-desktop-api-openapi-original.yml\ndocs: https://developers.beeper.com/desktop-api/authentication\nschemes:\n- name: oauth2\n  source: openapi/beeper-desktop-api-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: http://localhost:23373/oauth/authorize\n    tokenUrl: http://localhost:23373/oauth/token\n  description: OAuth2 Authorization Code flow with PKCE for obtaining bearer access tokens.\n    Used by MCP servers to authenticate clients.\nscopes:\n- scope: read\n  description: Read access to messages, chats, and accounts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/beeper-desktop-api-openapi-original.yml\n- scope: write\n  description: Write access to send messages, edit messages, react to messages, archive chats,\n    and set reminders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/beeper-desktop-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/scopes/beeper-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Consumer
- Messaging
- Chat
- Communication
- Matrix
- MCP
- Desktop
- Aggregator
token_urls:
- http://localhost:23373/oauth/token
---
