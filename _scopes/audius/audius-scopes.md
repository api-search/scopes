---
api_specs:
- filename: audius-challenges-api-openapi.yml
  format: yaml
  label: Audius challenges API
  slug: audius-challenges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-challenges-api-openapi.yml
- filename: audius-cid-data-api-openapi.yml
  format: yaml
  label: Audius cid_data API
  slug: audius-cid-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-cid-data-api-openapi.yml
- filename: audius-coins-api-openapi.yml
  format: yaml
  label: Audius coins API
  slug: audius-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-coins-api-openapi.yml
- filename: audius-comments-api-openapi.yml
  format: yaml
  label: Audius comments API
  slug: audius-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-comments-api-openapi.yml
- filename: audius-dashboard-wallet-users-api-openapi.yml
  format: yaml
  label: Audius dashboard_wallet_users API
  slug: audius-dashboard-wallet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-dashboard-wallet-users-api-openapi.yml
- filename: audius-developer-apps-api-openapi.yml
  format: yaml
  label: Audius developer_apps API
  slug: audius-developer-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-developer-apps-api-openapi.yml
- filename: audius-events-api-openapi.yml
  format: yaml
  label: Audius events API
  slug: audius-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-events-api-openapi.yml
- filename: audius-explore-api-openapi.yml
  format: yaml
  label: Audius explore API
  slug: audius-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-explore-api-openapi.yml
- filename: audius-notifications-api-openapi.yml
  format: yaml
  label: Audius notifications API
  slug: audius-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-notifications-api-openapi.yml
- filename: audius-playlists-api-openapi.yml
  format: yaml
  label: Audius playlists API
  slug: audius-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-playlists-api-openapi.yml
- filename: audius-prizes-api-openapi.yml
  format: yaml
  label: Audius prizes API
  slug: audius-prizes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-prizes-api-openapi.yml
- filename: audius-reactions-api-openapi.yml
  format: yaml
  label: Audius reactions API
  slug: audius-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-reactions-api-openapi.yml
- filename: audius-resolve-api-openapi.yml
  format: yaml
  label: Audius resolve API
  slug: audius-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-resolve-api-openapi.yml
- filename: audius-rewards-api-openapi.yml
  format: yaml
  label: Audius rewards API
  slug: audius-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-rewards-api-openapi.yml
- filename: audius-search-api-openapi.yml
  format: yaml
  label: Audius search API
  slug: audius-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-search-api-openapi.yml
- filename: audius-tips-api-openapi.yml
  format: yaml
  label: Audius tips API
  slug: audius-tips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-tips-api-openapi.yml
- filename: audius-tracks-api-openapi.yml
  format: yaml
  label: Audius tracks API
  slug: audius-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-tracks-api-openapi.yml
- filename: audius-transactions-api-openapi.yml
  format: yaml
  label: Audius transactions API
  slug: audius-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-transactions-api-openapi.yml
- filename: audius-users-api-openapi.yml
  format: yaml
  label: Audius users API
  slug: audius-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-users-api-openapi.yml
- filename: audius-wallet-api-openapi.yml
  format: yaml
  label: Audius wallet API
  slug: audius-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-wallet-api-openapi.yml
authorization_urls:
- /v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Audius Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Audius publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Audius API on a user''s behalf.


  Tokens are issued from /v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Audius
provider_slug: audius
schemes:
- description: 'OAuth 2.0 Authorization Code flow with PKCE for third-party applications.


    Allows apps to authenticate users and obtain access tokens scoped to read or read+write permissions on behalf of the user.


    **Scopes:**

    - `read` — Read-only access to the user''s public and private data.

    - `write` — Read and write access, allowing mutations on behalf of the user.


    **PKCE Required:**

    All authorization code requests must include `code_challenge` and `code_challenge_method=S256` parameters.'
  flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: /v1/oauth/token
  name: OAuth2
  source: openapi/audius-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read-only access to user data
  flows:
  - authorizationCode
  scope: read
- description: Read and write access on behalf of the user
  flows:
  - authorizationCode
  scope: write
slug: audius-scopes
source_filename: audius-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/audius-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/audius-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\n  description: |-\n    OAuth 2.0 Authorization Code flow with PKCE for third-party applications.\n\n    Allows apps to authenticate users and obtain access tokens scoped to read or read+write permissions on behalf of the user.\n\n    **Scopes:**\n    - `read` — Read-only access to the user's public and private data.\n    - `write` — Read and write access, allowing mutations on behalf of the user.\n\n    **PKCE Required:**\n    All authorization code requests must include `code_challenge` and `code_challenge_method=S256` parameters.\nscopes:\n- scope: read\n  description: Read-only access to user data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/audius-openapi.yml\n- scope: write\n  description: Read and write access\
  \ on behalf of the user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/audius-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/scopes/audius-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Music
- Streaming
- Decentralized
- Web3
- Open-Source
- Blockchain
token_urls:
- /v1/oauth/token
---
