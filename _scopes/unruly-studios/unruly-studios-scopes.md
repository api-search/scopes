---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Unruly Studios Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Unruly Studios publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unruly Studios API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unruly Studios
provider_slug: unruly-studios
schemes: []
scope_count: 9
scope_names:
- api
- read_api
- read_user
- read_repository
- write_repository
- sudo
- openid
- profile
- email
scopes:
- description: Full read/write access to the API, including all groups, projects, and the container/package registries.
  flows: []
  scope: api
- description: Read-only access to the API, including all groups and projects.
  flows: []
  scope: read_api
- description: Read-only access to the authenticated user's profile via the /user endpoint and related read-only endpoints.
  flows: []
  scope: read_user
- description: Read-only access to repositories on private projects (clone/read files) using Git-over-HTTP or the Repository Files API.
  flows: []
  scope: read_repository
- description: Read-write access to repositories on private projects (push/commit files) using Git-over-HTTP or the Repository Files API.
  flows: []
  scope: write_repository
- description: Perform API actions as any user in the system (admin only).
  flows: []
  scope: sudo
- description: Authenticate using OpenID Connect; grants access to the userinfo endpoint and ID token.
  flows: []
  scope: openid
- description: Read the user's profile data (name, nickname, picture) via OpenID Connect.
  flows: []
  scope: profile
- description: Read the user's primary email address via OpenID Connect.
  flows: []
  scope: email
slug: unruly-studios-scopes
source_filename: unruly-studios-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://gamelocker.unruly-studios.com/.well-known/openid-configuration\nnotes: >-\n  OAuth scopes advertised by the GitLab OAuth/OIDC server on the Gamelocker\n  host (scopes_supported). These are GitLab's standard scopes; descriptions\n  follow GitLab's documented meanings.\nauthorization_server: https://gamelocker.unruly-studios.com\nscopes:\n- name: api\n  description: Full read/write access to the API, including all groups, projects, and the container/package registries.\n- name: read_api\n  description: Read-only access to the API, including all groups and projects.\n- name: read_user\n  description: Read-only access to the authenticated user's profile via the /user endpoint and related read-only endpoints.\n- name: read_repository\n  description: Read-only access to repositories on private projects (clone/read files) using Git-over-HTTP or the Repository Files API.\n- name: write_repository\n  description: Read-write\
  \ access to repositories on private projects (push/commit files) using Git-over-HTTP or the Repository Files API.\n- name: sudo\n  description: Perform API actions as any user in the system (admin only).\n- name: openid\n  description: Authenticate using OpenID Connect; grants access to the userinfo endpoint and ID token.\n- name: profile\n  description: Read the user's profile data (name, nickname, picture) via OpenID Connect.\n- name: email\n  description: Read the user's primary email address via OpenID Connect.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unruly-studios/refs/heads/main/scopes/unruly-studios-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Education
- STEM
- EdTech
- Coding
- Kids
- Learning
- Hardware
token_bound: false
token_urls: []
---
