---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Blogger Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Blogger publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Blogger API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Blogger
provider_slug: google-blogger
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/blogger.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/blogger
- https://www.googleapis.com/auth/blogger.readonly
scopes:
- description: Manage your Blogger account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/blogger
- description: View your Blogger account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/blogger.readonly
slug: google-blogger-scopes
source_filename: google-blogger-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blogger.yml\nschemes:\n- name: oauth2\n  source: openapi/blogger.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/blogger\n  description: Manage your Blogger account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/blogger.yml\n- scope: https://www.googleapis.com/auth/blogger.readonly\n  description: View your Blogger account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/blogger.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-blogger/refs/heads/main/scopes/google-blogger-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Blogging
- CMS
- Comments
- Google
- Pages
- Posts
- Publishing
token_urls:
- https://oauth2.googleapis.com/token
---
