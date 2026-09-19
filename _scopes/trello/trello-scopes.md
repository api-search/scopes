---
api_specs:
- filename: trello-webhooks-asyncapi.yml
  format: yaml
  label: Trello Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/asyncapi/trello-webhooks-asyncapi.yml
- filename: trello-actions-api-openapi.yml
  format: yaml
  label: trello Actions API
  slug: trello-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-actions-api-openapi.yml
- filename: trello-boards-api-openapi.yml
  format: yaml
  label: trello Boards API
  slug: trello-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-boards-api-openapi.yml
- filename: trello-cards-api-openapi.yml
  format: yaml
  label: trello Cards API
  slug: trello-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-cards-api-openapi.yml
- filename: trello-checklists-api-openapi.yml
  format: yaml
  label: trello Checklists API
  slug: trello-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-checklists-api-openapi.yml
- filename: trello-labels-api-openapi.yml
  format: yaml
  label: trello Labels API
  slug: trello-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-labels-api-openapi.yml
- filename: trello-lists-api-openapi.yml
  format: yaml
  label: trello Lists API
  slug: trello-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-lists-api-openapi.yml
- filename: trello-members-api-openapi.yml
  format: yaml
  label: trello Members API
  slug: trello-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-members-api-openapi.yml
- filename: trello-notifications-api-openapi.yml
  format: yaml
  label: trello Notifications API
  slug: trello-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-notifications-api-openapi.yml
- filename: trello-organizations-api-openapi.yml
  format: yaml
  label: trello Organizations API
  slug: trello-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-organizations-api-openapi.yml
- filename: trello-plugins-api-openapi.yml
  format: yaml
  label: trello Plugins API
  slug: trello-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-plugins-api-openapi.yml
- filename: trello-search-api-openapi.yml
  format: yaml
  label: trello Search API
  slug: trello-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-search-api-openapi.yml
- filename: trello-tokens-api-openapi.yml
  format: yaml
  label: trello Tokens API
  slug: trello-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-tokens-api-openapi.yml
- filename: trello-webhooks-api-openapi.yml
  format: yaml
  label: trello Webhooks API
  slug: trello-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-webhooks-api-openapi.yml
- filename: trello-custom-fields-api-openapi.yml
  format: yaml
  label: Trello Custom Fields API
  slug: trello-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-custom-fields-api-openapi.yml
- filename: trello-rest-api-openapi.json
  format: json
  label: Trello REST API
  slug: trello-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-rest-api-openapi.json
authorization_urls:
- https://auth.atlassian.com/authorize
description: Trello OAuth 2.0 3LO scopes. OAuth 2.0 reached GA for Trello on 2026-09-15; these ten scopes replace the three coarse legacy Trello Auth scopes (read, write, account), which remain live on the 1/authorize route. Scope-to-resource mapping for the webhook surface is documented by Trello and recorded per scope below.
docs: https://developer.atlassian.com/cloud/trello/guides/rest-api/oauth-2-getting-started/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Trello Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Trello publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Trello API on a user''s behalf.


  Tokens are issued from https://auth.atlassian.com/authorize/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Trello
provider_slug: trello
schemes:
- flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.atlassian.com/authorize/oauth/token
  name: OAuth2
  source: openapi/trello-rest-api-openapi.json
scope_count: 10
scope_names:
- read:board:trello
- read:enterprise:trello
- read:member:trello
- read:organization:trello
- write:board:membership:trello
- write:board:trello
- write:enterprise:trello
- write:member:trello
- write:organization:membership:trello
- write:organization:trello
scopes:
- description: Read cards, lists, and comments in boards.
  flows:
  - authorizationCode
  scope: read:board:trello
- description: Read enterprises.
  flows:
  - authorizationCode
  scope: read:enterprise:trello
- description: Read email address, public name, public avatar, and memberships of boards, workspaces, and enterprises.
  flows:
  - authorizationCode
  scope: read:member:trello
- description: Read workspaces.
  flows:
  - authorizationCode
  scope: read:organization:trello
- description: Add, remove, or modify memberships on boards.
  flows:
  - authorizationCode
  scope: write:board:membership:trello
- description: Create and update cards, lists, and comments in boards.
  flows:
  - authorizationCode
  scope: write:board:trello
- description: Update and manage enterprises.
  flows:
  - authorizationCode
  scope: write:enterprise:trello
- description: Upload custom emojis and stickers, star boards, and save searches.
  flows:
  - authorizationCode
  scope: write:member:trello
- description: Add, remove, or modify memberships on workspaces.
  flows:
  - authorizationCode
  scope: write:organization:membership:trello
- description: Update workspaces.
  flows:
  - authorizationCode
  scope: write:organization:trello
slug: trello-scopes
source_filename: trello-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  openapi/trello-rest-api-openapi.json (components.securitySchemes.OAuth2) confirmed against\n  https://developer.atlassian.com/cloud/trello/guides/rest-api/oauth-2-getting-started/ and\n  https://developer.atlassian.com/cloud/trello/guides/rest-api/webhooks/\ndocs: https://developer.atlassian.com/cloud/trello/guides/rest-api/oauth-2-getting-started/\ndescription: >-\n  Trello OAuth 2.0 3LO scopes. OAuth 2.0 reached GA for Trello on 2026-09-15; these ten\n  scopes replace the three coarse legacy Trello Auth scopes (read, write, account), which\n  remain live on the 1/authorize route. Scope-to-resource mapping for the webhook surface is\n  documented by Trello and recorded per scope below.\nlegacy_scopes:\n  mechanism: Trello Auth 1/authorize route (and OAuth 1.0a)\n  docs: https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/\n  scopes:\n  - scope: read\n    description: Reading of boards, organizations\
  \ and other objects on behalf of the user.\n  - scope: write\n    description: Writing of boards, organizations and other objects on behalf of the user.\n  - scope: account\n    description: >-\n      Read the member email address, write member info, and mark notifications read. Member\n      emails are only accessible when this scope is granted, and only for the granting user.\n  expiration_options: [1hour, 1day, 30days, never]\n  status: >-\n    Still supported. Announced 2025-04-16 as the mechanism OAuth 2.0 would replace, but no\n    removal date has been published.\nschemes:\n- name: OAuth2\n  source: openapi/trello-rest-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/authorize/oauth/token\nscopes:\n- scope: read:board:trello\n  description: Read cards, lists, and comments in boards.\n  webhook_models: [Board, List, Card]\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n\
  - scope: read:enterprise:trello\n  description: Read enterprises.\n  webhook_models: [Enterprise]\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n- scope: read:member:trello\n  description: Read email address, public name, public avatar, and memberships of boards, workspaces,\n    and enterprises.\n  webhook_models: [Member]\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n- scope: read:organization:trello\n  description: Read workspaces.\n  webhook_models: [Organization]\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n- scope: write:board:membership:trello\n  description: Add, remove, or modify memberships on boards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n- scope: write:board:trello\n  description: Create and update cards, lists, and comments in boards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n\
  - scope: write:enterprise:trello\n  description: Update and manage enterprises.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n- scope: write:member:trello\n  description: Upload custom emojis and stickers, star boards, and save searches.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n- scope: write:organization:membership:trello\n  description: Add, remove, or modify memberships on workspaces.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\n- scope: write:organization:trello\n  description: Update workspaces.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/trello-rest-api-openapi.json\nrestrictions:\n  power_up_clients: >-\n    Power-Up OAuth 2.0 clients are workspace-restricted. Any model they act on - including a\n    webhook's idModel - must belong to a workspace the access token was authorized for, or\n    the request fails with 403. OAuth 2.0 clients\
  \ of non-Power-Up apps carry no such\n    restriction.\n  source: https://developer.atlassian.com/cloud/trello/guides/rest-api/webhooks/\ntoken_lifetime:\n  short_lived: true\n  refresh: true\n  note: OAuth 2.0 tokens have limited lifetimes by default and must be periodically refreshed.\n  source: https://developer.atlassian.com/cloud/trello/guides/rest-api/oauth-2-getting-started/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/scopes/trello-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Project Management
- Kanban
- Task Management
- Collaboration
- Productivity
- Workflows
- Boards
- Atlassian
token_urls:
- https://auth.atlassian.com/authorize/oauth/token
---
