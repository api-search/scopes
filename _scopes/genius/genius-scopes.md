---
api_specs:
- filename: genius-openapi.yml
  format: yaml
  label: Genius
  slug: genius
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genius/refs/heads/main/openapi/genius-openapi.yml
authorization_urls:
- https://api.genius.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Genius Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Genius publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Genius API on a user''s behalf.


  Tokens are issued from https://api.genius.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Genius
provider_slug: genius
schemes:
- description: 'Genius uses OAuth 2.0 with the authorization-code flow. Apps are

    registered at https://genius.com/api-clients.'
  flows:
  - authorizationUrl: https://api.genius.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.genius.com/oauth/token
  name: GeniusOAuth2
  source: openapi/genius-openapi.yml
scope_count: 4
scope_names:
- create_annotation
- manage_annotation
- me
- vote
scopes:
- description: Create new annotations.
  flows:
  - authorizationCode
  scope: create_annotation
- description: Edit or delete the user's annotations.
  flows:
  - authorizationCode
  scope: manage_annotation
- description: Access account profile of the authenticated user.
  flows:
  - authorizationCode
  scope: me
- description: Upvote, downvote, or remove a vote on annotations.
  flows:
  - authorizationCode
  scope: vote
slug: genius-scopes
source_filename: genius-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/genius-openapi.yml\nschemes:\n- name: GeniusOAuth2\n  source: openapi/genius-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.genius.com/oauth/authorize\n    tokenUrl: https://api.genius.com/oauth/token\n  description: |-\n    Genius uses OAuth 2.0 with the authorization-code flow. Apps are\n    registered at https://genius.com/api-clients.\nscopes:\n- scope: create_annotation\n  description: Create new annotations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/genius-openapi.yml\n- scope: manage_annotation\n  description: Edit or delete the user's annotations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/genius-openapi.yml\n- scope: me\n  description: Access account profile of the authenticated user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/genius-openapi.yml\n- scope: vote\n  description: Upvote, downvote, or remove a vote on annotations.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/genius-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genius/refs/heads/main/scopes/genius-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Music
- Lyrics
- Annotations
- Crowdsourced
- Reference Data
- Public APIs
token_urls:
- https://api.genius.com/oauth/token
---
