---
authorization_urls: []
description: ''
docs: https://github.com/appdotnet/api-spec/tree/new-docs/content/reference/authentication
flows:
- authorizationCode
- implicit
- password
kind: oauth-scopes
layout: scope
method: searched
name: Appnet Scopes
name_suffix: OAuth Scopes
note: Scopes apply only to user tokens (not app tokens) and are requested on the initial access-token request. The granted scopes are returned on each response via the X-OAuth-Scopes header. The `basic` scope is always granted on creation of a user token.
overview: 'App.net publishes 9 OAuth 2.0 scopes via the authorizationCode, implicit, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the App.net API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: App.net
provider_slug: appnet
schemes:
- authorizationUrl: https://account.app.net/oauth/authenticate
  flows:
  - authorizationCode
  - implicit
  - password
  name: OAuth2
  tokenUrl: https://account.app.net/oauth/access_token
scope_count: 9
scope_names:
- basic
- stream
- write_post
- follow
- public_messages
- messages
- update_profile
- files
- export
scopes:
- description: See basic information about this user. Always granted on user-token creation.
  flows: []
  scope: basic
- description: Read this user's stream.
  flows: []
  scope: stream
- description: Create a new post as this user.
  flows: []
  scope: write_post
- description: Add or remove follows (or mutes) for this user.
  flows: []
  scope: follow
- description: Send and receive public messages as this user.
  flows: []
  scope: public_messages
- description: Send and receive public and private messages as this user.
  flows: []
  scope: messages
- description: Update a user's name, images, and other profile information.
  flows: []
  scope: update_profile
- description: Manage a user's files. Not required for uploading files.
  flows: []
  scope: files
- description: Bulk export all of this user's App.net data. Intended for backup services only; users are shown an extra warning due to the sensitivity of this data.
  flows: []
  scope: export
slug: appnet-scopes
source_filename: appnet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/appdotnet/api-spec/blob/new-docs/content/reference/authentication/index.md\ndocs: https://github.com/appdotnet/api-spec/tree/new-docs/content/reference/authentication\nnote: >-\n  Scopes apply only to user tokens (not app tokens) and are requested on the initial\n  access-token request. The granted scopes are returned on each response via the\n  X-OAuth-Scopes header. The `basic` scope is always granted on creation of a user token.\nschemes:\n- name: OAuth2\n  authorizationUrl: https://account.app.net/oauth/authenticate\n  tokenUrl: https://account.app.net/oauth/access_token\n  flows: [authorizationCode, implicit, password]\nscopes:\n- scope: basic\n  description: See basic information about this user. Always granted on user-token creation.\n- scope: stream\n  description: Read this user's stream.\n- scope: write_post\n  description: Create a new post as this user.\n- scope: follow\n  description: Add or\
  \ remove follows (or mutes) for this user.\n- scope: public_messages\n  description: Send and receive public messages as this user.\n- scope: messages\n  description: Send and receive public and private messages as this user.\n- scope: update_profile\n  description: Update a user's name, images, and other profile information.\n- scope: files\n  description: Manage a user's files. Not required for uploading files.\n- scope: export\n  description: >-\n    Bulk export all of this user's App.net data. Intended for backup services only;\n    users are shown an extra warning due to the sensitivity of this data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appnet/refs/heads/main/scopes/appnet-scopes.yml
summary_line: 9 scopes · authorizationCode/implicit/password
tags:
- Company
- Social
- Microblogging
- Messaging
- Real Time
- Streaming
- Developer Platform
- OAuth
- Defunct
token_urls: []
---
