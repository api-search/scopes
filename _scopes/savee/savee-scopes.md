---
api_specs:
- filename: savee-boards-api-openapi.yml
  format: yaml
  label: Savee Boards API
  slug: savee-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-boards-api-openapi.yml
- filename: savee-saves-api-openapi.yml
  format: yaml
  label: Savee Saves API
  slug: savee-saves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-saves-api-openapi.yml
- filename: savee-search-api-openapi.yml
  format: yaml
  label: Savee Search API
  slug: savee-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-search-api-openapi.yml
- filename: savee-system-api-openapi.yml
  format: yaml
  label: Savee System API
  slug: savee-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-system-api-openapi.yml
- filename: savee-user-api-openapi.yml
  format: yaml
  label: Savee User API
  slug: savee-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-user-api-openapi.yml
authorization_urls:
- https://savee.com/oauth/authorize/
description: ''
docs: https://docs.savee.com/api/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Savee Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Savee publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Savee API on a user''s behalf.


  Tokens are issued from https://savee.com/api/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Savee
provider_slug: savee
schemes:
- description: '**OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.


    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error="insufficient_scope"` header naming it.'
  flows:
  - authorizationUrl: https://savee.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://savee.com/api/oauth/token/
  name: OAuth2
  source: openapi/savee-boards-api-openapi.yml
- description: '**OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.


    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error="insufficient_scope"` header naming it.'
  flows:
  - authorizationUrl: https://savee.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://savee.com/api/oauth/token/
  name: OAuth2
  source: openapi/savee-saves-api-openapi.yml
- description: '**OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.


    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error="insufficient_scope"` header naming it.'
  flows:
  - authorizationUrl: https://savee.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://savee.com/api/oauth/token/
  name: OAuth2
  source: openapi/savee-search-api-openapi.yml
- description: '**OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.


    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error="insufficient_scope"` header naming it.'
  flows:
  - authorizationUrl: https://savee.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://savee.com/api/oauth/token/
  name: OAuth2
  source: openapi/savee-user-api-openapi.yml
scope_count: 6
scope_names:
- boards:read
- profile:read
- saves:read
- search:read
- saves:write
- boards:write
scopes:
- description: Read the user’s boards and the saves on them
  flows:
  - authorizationCode
  scope: boards:read
- description: Read the user’s username, name, and avatar
  flows:
  - authorizationCode
  scope: profile:read
- description: Read the user’s saves and home feed
  flows:
  - authorizationCode
  scope: saves:read
- description: Search Savee’s public library on the user’s behalf
  flows:
  - authorizationCode
  scope: search:read
- description: Save items to your account and change their privacy
  flows:
  - authorizationCode
  scope: saves:write
- description: Create and edit your boards, and add or remove saves on them
  flows:
  - authorizationCode
  scope: boards:write
slug: savee-scopes
source_filename: savee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/savee-boards-api-openapi.yml, openapi/savee-saves-api-openapi.yml, openapi/savee-search-api-openapi.yml,\n  openapi/savee-user-api-openapi.yml + https://docs.savee.com/api/oauth + https://savee.com/.well-known/oauth-authorization-server\n  (probed 2026-09-03)\nschemes:\n- name: OAuth2\n  source: openapi/savee-boards-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://savee.com/oauth/authorize/\n    tokenUrl: https://savee.com/api/oauth/token/\n  description: |-\n    **OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.\n\n    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error=\"insufficient_scope\"` header naming it.\n- name: OAuth2\n  source: openapi/savee-saves-api-openapi.yml\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://savee.com/oauth/authorize/\n    tokenUrl: https://savee.com/api/oauth/token/\n  description: |-\n    **OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.\n\n    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error=\"insufficient_scope\"` header naming it.\n- name: OAuth2\n  source: openapi/savee-search-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://savee.com/oauth/authorize/\n    tokenUrl: https://savee.com/api/oauth/token/\n  description: |-\n    **OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.\n\n    Missing the scope\
  \ below returns `403` with a `WWW-Authenticate: Bearer error=\"insufficient_scope\"` header naming it.\n- name: OAuth2\n  source: openapi/savee-user-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://savee.com/oauth/authorize/\n    tokenUrl: https://savee.com/api/oauth/token/\n  description: |-\n    **OAuth access token** (`sv_at_…`) — obtained on one of your users’ behalf and limited to the scopes they approved. Use this when you’re building a product other people sign into with Savee. See https://docs.savee.com/api/oauth.\n\n    Missing the scope below returns `403` with a `WWW-Authenticate: Bearer error=\"insufficient_scope\"` header naming it.\nscopes:\n- scope: boards:read\n  description: Read the user’s boards and the saves on them\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/savee-boards-api-openapi.yml\n  - openapi/savee-saves-api-openapi.yml\n  - openapi/savee-search-api-openapi.yml\n  - openapi/savee-user-api-openapi.yml\n  default:\
  \ true\n- scope: profile:read\n  description: Read the user’s username, name, and avatar\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/savee-boards-api-openapi.yml\n  - openapi/savee-saves-api-openapi.yml\n  - openapi/savee-search-api-openapi.yml\n  - openapi/savee-user-api-openapi.yml\n  default: true\n- scope: saves:read\n  description: Read the user’s saves and home feed\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/savee-boards-api-openapi.yml\n  - openapi/savee-saves-api-openapi.yml\n  - openapi/savee-search-api-openapi.yml\n  - openapi/savee-user-api-openapi.yml\n  default: true\n- scope: search:read\n  description: Search Savee’s public library on the user’s behalf\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/savee-boards-api-openapi.yml\n  - openapi/savee-saves-api-openapi.yml\n  - openapi/savee-search-api-openapi.yml\n  - openapi/savee-user-api-openapi.yml\n  default: false\n  note: Not in the default grant; reads the public library, not the\
  \ user's account. Shares the account-wide\n    20/5min + 200/week search budget.\n- scope: saves:write\n  description: Save items to your account and change their privacy\n  flows:\n  - authorizationCode\n  default: false\n  surfaces:\n  - mcp\n  sources:\n  - https://savee.com/.well-known/oauth-authorization-server\n  - https://docs.savee.com/mcp/permissions\n  note: 'MCP-only: gates the save_items write tool. Not used by any REST operation.'\n- scope: boards:write\n  description: Create and edit your boards, and add or remove saves on them\n  flows:\n  - authorizationCode\n  default: false\n  surfaces:\n  - mcp\n  sources:\n  - https://savee.com/.well-known/oauth-authorization-server\n  - https://docs.savee.com/mcp/permissions\n  note: 'MCP-only: gates create_board, update_board and remove_save_from_board. Not used by any REST operation.'\ndocs: https://docs.savee.com/api/oauth\nnotes: 'The authorization-server metadata advertises six scopes; the two write scopes are used only by\n \
  \ the MCP server''s write tools (the REST API has no write surface). Requesting no scope grants the three\n  account-read scopes (profile:read, saves:read, boards:read); search:read is never granted implicitly\n  and must be asked for. Write scopes are marked separately on the consent screen and never granted implicitly.\n  A call missing a scope returns 403 with WWW-Authenticate: Bearer error=\"insufficient_scope\" naming the\n  missing scope(s).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/scopes/savee-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Design
- visual inspiration
- Image
- Creative
- Moodboards
- Artificial Intelligence (AI)
token_urls:
- https://savee.com/api/oauth/token/
---
