---
api_specs:
- filename: stackexchange-access-tokens-api-openapi.yml
  format: yaml
  label: Stack Exchange Access Tokens API
  slug: stackexchange-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-access-tokens-api-openapi.yml
- filename: stackexchange-answers-api-openapi.yml
  format: yaml
  label: Stack Exchange Answers API
  slug: stackexchange-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-answers-api-openapi.yml
- filename: stackexchange-badges-api-openapi.yml
  format: yaml
  label: Stack Exchange Badges API
  slug: stackexchange-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-badges-api-openapi.yml
- filename: stackexchange-comments-api-openapi.yml
  format: yaml
  label: Stack Exchange Comments API
  slug: stackexchange-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-comments-api-openapi.yml
- filename: stackexchange-events-api-openapi.yml
  format: yaml
  label: Stack Exchange Events API
  slug: stackexchange-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-events-api-openapi.yml
- filename: stackexchange-filters-api-openapi.yml
  format: yaml
  label: Stack Exchange Filters API
  slug: stackexchange-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-filters-api-openapi.yml
- filename: stackexchange-info-api-openapi.yml
  format: yaml
  label: Stack Exchange Info API
  slug: stackexchange-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-info-api-openapi.yml
- filename: stackexchange-me-api-openapi.yml
  format: yaml
  label: Stack Exchange Me API
  slug: stackexchange-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-me-api-openapi.yml
- filename: stackexchange-posts-api-openapi.yml
  format: yaml
  label: Stack Exchange Posts API
  slug: stackexchange-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-posts-api-openapi.yml
- filename: stackexchange-questions-api-openapi.yml
  format: yaml
  label: Stack Exchange Questions API
  slug: stackexchange-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-questions-api-openapi.yml
- filename: stackexchange-revisions-api-openapi.yml
  format: yaml
  label: Stack Exchange Revisions API
  slug: stackexchange-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-revisions-api-openapi.yml
- filename: stackexchange-search-api-openapi.yml
  format: yaml
  label: Stack Exchange Search API
  slug: stackexchange-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-search-api-openapi.yml
- filename: stackexchange-sites-api-openapi.yml
  format: yaml
  label: Stack Exchange Sites API
  slug: stackexchange-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-sites-api-openapi.yml
- filename: stackexchange-suggested-edits-api-openapi.yml
  format: yaml
  label: Stack Exchange Suggested Edits API
  slug: stackexchange-suggested-edits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-suggested-edits-api-openapi.yml
- filename: stackexchange-tags-api-openapi.yml
  format: yaml
  label: Stack Exchange Tags API
  slug: stackexchange-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-tags-api-openapi.yml
- filename: stackexchange-users-api-openapi.yml
  format: yaml
  label: Stack Exchange Users API
  slug: stackexchange-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/openapi/stackexchange-users-api-openapi.yml
authorization_urls:
- https://stackoverflow.com/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Stackexchange Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Stack Exchange publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Stack Exchange API on a user''s behalf.


  Tokens are issued from https://stackoverflow.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stack Exchange
provider_slug: stackexchange
schemes:
- description: 'OAuth 2.0 explicit or implicit flow. Apps register on stackapps.com.

    Read methods do not require auth; write methods require `write_access`.

    `private_info` is needed for /me/notifications, /me/inbox, and similar

    private surfaces. `no_expiry` issues tokens that never expire.'
  flows:
  - authorizationUrl: https://stackoverflow.com/oauth
    flow: authorizationCode
    tokenUrl: https://stackoverflow.com/oauth/access_token
  name: oauth2
  source: openapi/stackexchange-api-v2-3.yaml
scope_count: 4
scope_names:
- no_expiry
- private_info
- read_inbox
- write_access
scopes:
- description: Issue a token that never expires.
  flows:
  - authorizationCode
  scope: no_expiry
- description: Access endpoints that return personal information.
  flows:
  - authorizationCode
  scope: private_info
- description: Access the authenticated user's inbox.
  flows:
  - authorizationCode
  scope: read_inbox
- description: Vote, post, comment, flag, accept on the user's behalf.
  flows:
  - authorizationCode
  scope: write_access
slug: stackexchange-scopes
source_filename: stackexchange-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stackexchange-api-v2-3.yaml\nschemes:\n- name: oauth2\n  source: openapi/stackexchange-api-v2-3.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://stackoverflow.com/oauth\n    tokenUrl: https://stackoverflow.com/oauth/access_token\n  description: |-\n    OAuth 2.0 explicit or implicit flow. Apps register on stackapps.com.\n    Read methods do not require auth; write methods require `write_access`.\n    `private_info` is needed for /me/notifications, /me/inbox, and similar\n    private surfaces. `no_expiry` issues tokens that never expire.\nscopes:\n- scope: no_expiry\n  description: Issue a token that never expires.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stackexchange-api-v2-3.yaml\n- scope: private_info\n  description: Access endpoints that return personal information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stackexchange-api-v2-3.yaml\n- scope: read_inbox\n\
  \  description: Access the authenticated user's inbox.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stackexchange-api-v2-3.yaml\n- scope: write_access\n  description: Vote, post, comment, flag, accept on the user's behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/stackexchange-api-v2-3.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackexchange/refs/heads/main/scopes/stackexchange-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Q And A
- Developer Community
- Knowledge Graph
- Stack Overflow
- Stack Exchange
- Reputation
- Tags
- Community
- MCP
- AI Grounding
token_urls:
- https://stackoverflow.com/oauth/access_token
---
