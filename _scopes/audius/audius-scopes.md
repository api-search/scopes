---
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
- Open Source
- Blockchain
token_urls:
- /v1/oauth/token
---
