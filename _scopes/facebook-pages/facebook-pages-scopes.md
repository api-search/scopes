---
authorization_urls:
- https://www.facebook.com/v22.0/dialog/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Facebook Pages Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Facebook Pages API publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Facebook Pages API API on a user''s behalf.


  Tokens are issued from https://graph.facebook.com/v22.0/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Facebook Pages API
provider_slug: facebook-pages
schemes:
- description: 'OAuth 2.0 Page access token. Granted scopes determine which

    endpoints can be called. Send as a Bearer token or as the

    access_token query parameter.'
  flows:
  - authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth
    flow: authorizationCode
    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token
  name: PageAccessToken
  source: openapi/facebook-pages-openapi.yml
scope_count: 7
scope_names:
- pages_manage_engagement
- pages_manage_metadata
- pages_manage_posts
- pages_messaging
- pages_read_engagement
- pages_read_user_content
- pages_show_list
scopes:
- description: Moderate comments and reactions
  flows:
  - authorizationCode
  scope: pages_manage_engagement
- description: Manage Page settings and subscribed apps
  flows:
  - authorizationCode
  scope: pages_manage_metadata
- description: Publish and edit posts
  flows:
  - authorizationCode
  scope: pages_manage_posts
- description: Send and receive Messenger messages
  flows:
  - authorizationCode
  scope: pages_messaging
- description: Read Page content and engagement
  flows:
  - authorizationCode
  scope: pages_read_engagement
- description: Read user-generated content on a Page
  flows:
  - authorizationCode
  scope: pages_read_user_content
- description: List Pages the user manages
  flows:
  - authorizationCode
  scope: pages_show_list
slug: facebook-pages-scopes
source_filename: facebook-pages-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/facebook-pages-openapi.yml\nschemes:\n- name: PageAccessToken\n  source: openapi/facebook-pages-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth\n    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token\n  description: |-\n    OAuth 2.0 Page access token. Granted scopes determine which\n    endpoints can be called. Send as a Bearer token or as the\n    access_token query parameter.\nscopes:\n- scope: pages_manage_engagement\n  description: Moderate comments and reactions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-pages-openapi.yml\n- scope: pages_manage_metadata\n  description: Manage Page settings and subscribed apps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-pages-openapi.yml\n- scope: pages_manage_posts\n  description: Publish and edit posts\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/facebook-pages-openapi.yml\n- scope: pages_messaging\n  description: Send and receive Messenger messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-pages-openapi.yml\n- scope: pages_read_engagement\n  description: Read Page content and engagement\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-pages-openapi.yml\n- scope: pages_read_user_content\n  description: Read user-generated content on a Page\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-pages-openapi.yml\n- scope: pages_show_list\n  description: List Pages the user manages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-pages-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-pages/refs/heads/main/scopes/facebook-pages-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Social Media
- Facebook
- Meta Graph API
- Pages
- Content Publishing
- Social Insights
token_urls:
- https://graph.facebook.com/v22.0/oauth/access_token
---
