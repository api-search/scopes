---
authorization_urls:
- https://accounts.snapchat.com/accounts/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Snapchat Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Snapchat publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Snapchat API on a user''s behalf.


  Tokens are issued from https://accounts.snapchat.com/login/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Snapchat
provider_slug: snapchat
schemes:
- description: OAuth 2.0 authorization. Access tokens are obtained via the authorization code flow and expire after 3600 seconds. Refresh tokens can be used to obtain new access tokens.
  flows:
  - authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token
  name: bearerAuth
  source: openapi/snapchat-ads-api-openapi.yml
scope_count: 1
scope_names:
- snapchat-marketing-api
scopes:
- description: Access to the Snapchat Marketing API
  flows:
  - authorizationCode
  scope: snapchat-marketing-api
slug: snapchat-scopes
source_filename: snapchat-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snapchat-ads-api-openapi.yml\nschemes:\n- name: bearerAuth\n  source: openapi/snapchat-ads-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth\n    tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token\n  description: OAuth 2.0 authorization. Access tokens are obtained via the authorization code\n    flow and expire after 3600 seconds. Refresh tokens can be used to obtain new access tokens.\nscopes:\n- scope: snapchat-marketing-api\n  description: Access to the Snapchat Marketing API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/snapchat-ads-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/scopes/snapchat-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Advertising
- AR
- Augmented Reality
- Marketing
- Messaging
- Social Media
token_urls:
- https://accounts.snapchat.com/login/oauth2/access_token
---
