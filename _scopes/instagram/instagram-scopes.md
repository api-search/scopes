---
api_specs:
- filename: instagram-graph-api.yaml
  format: yaml
  label: Instagram API with Instagram Login
  slug: instagram-api-with-instagram-login
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-graph-api.yaml
- filename: instagram-graph-api.yaml
  format: yaml
  label: Instagram API with Facebook Login
  slug: instagram-api-with-facebook-login
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-graph-api.yaml
authorization_urls:
- https://www.facebook.com/dialog/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Instagram Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Instagram publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Instagram API on a user''s behalf.


  Tokens are issued from https://graph.facebook.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Instagram
provider_slug: instagram
schemes:
- description: OAuth 2.0 authentication via Instagram Login or Facebook Login.
  flows:
  - authorizationUrl: https://www.facebook.com/dialog/oauth
    flow: authorizationCode
    tokenUrl: https://graph.facebook.com/oauth/access_token
  name: oauth2
  source: openapi/instagram-graph-api.yaml
scope_count: 7
scope_names:
- instagram_basic
- instagram_content_publish
- instagram_manage_comments
- instagram_manage_insights
- instagram_manage_messages
- pages_read_engagement
- pages_show_list
scopes:
- description: Read user profile and media.
  flows:
  - authorizationCode
  scope: instagram_basic
- description: Publish content on behalf of the user.
  flows:
  - authorizationCode
  scope: instagram_content_publish
- description: Manage comments on media.
  flows:
  - authorizationCode
  scope: instagram_manage_comments
- description: Access insights and analytics.
  flows:
  - authorizationCode
  scope: instagram_manage_insights
- description: Manage Instagram Direct messages.
  flows:
  - authorizationCode
  scope: instagram_manage_messages
- description: Read engagement data from pages.
  flows:
  - authorizationCode
  scope: pages_read_engagement
- description: Show list of pages managed by user.
  flows:
  - authorizationCode
  scope: pages_show_list
slug: instagram-scopes
source_filename: instagram-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instagram-graph-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/instagram-graph-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.facebook.com/dialog/oauth\n    tokenUrl: https://graph.facebook.com/oauth/access_token\n  description: OAuth 2.0 authentication via Instagram Login or Facebook Login.\nscopes:\n- scope: instagram_basic\n  description: Read user profile and media.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/instagram-graph-api.yaml\n- scope: instagram_content_publish\n  description: Publish content on behalf of the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/instagram-graph-api.yaml\n- scope: instagram_manage_comments\n  description: Manage comments on media.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/instagram-graph-api.yaml\n- scope: instagram_manage_insights\n  description: Access insights and analytics.\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - openapi/instagram-graph-api.yaml\n- scope: instagram_manage_messages\n  description: Manage Instagram Direct messages.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/instagram-graph-api.yaml\n- scope: pages_read_engagement\n  description: Read engagement data from pages.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/instagram-graph-api.yaml\n- scope: pages_show_list\n  description: Show list of pages managed by user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/instagram-graph-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/scopes/instagram-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
token_urls:
- https://graph.facebook.com/oauth/access_token
---
