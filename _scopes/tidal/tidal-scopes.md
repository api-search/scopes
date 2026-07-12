---
authorization_urls:
- https://login.tidal.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Tidal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TIDAL publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the TIDAL API on a user''s behalf.


  Tokens are issued from https://auth.tidal.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TIDAL
provider_slug: tidal
schemes:
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-catalog-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-catalog-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-claims-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-claims-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-commerce-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-commerce-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-playback-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-playback-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-playlists-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-playlists-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-recommendations-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-recommendations-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-search-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-search-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-social-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-social-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-user-collections-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-user-collections-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code
  flows:
  - authorizationUrl: https://login.tidal.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Authorization_Code_PKCE
  source: openapi/tidal-users-api-openapi.yml
- description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.tidal.com/v1/oauth2/token
  name: Client_Credentials
  source: openapi/tidal-users-api-openapi.yml
scope_count: 12
scope_names:
- collection.read
- collection.write
- entitlements.read
- playback
- playlists.read
- playlists.write
- r_usr
- recommendations.read
- search.read
- search.write
- user.read
- w_usr
scopes:
- description: Read access to a user's "My Collection".
  flows:
  - authorizationCode
  scope: collection.read
- description: Write access to a user's "My Collection".
  flows:
  - authorizationCode
  scope: collection.write
- description: Read access to what functionality a user is entitled to access on TIDAL, such as whether they can stream music, use DJ add-ons and similar.
  flows:
  - authorizationCode
  scope: entitlements.read
- description: Required to play media content and control playback.
  flows:
  - authorizationCode
  scope: playback
- description: Required to list playlists created by a user.
  flows:
  - authorizationCode
  scope: playlists.read
- description: Write access to a user's playlists.
  flows:
  - authorizationCode
  scope: playlists.write
- description: Read access to all end user data
  flows:
  - authorizationCode
  scope: r_usr
- description: Read access to a user’s personal recommendations.
  flows:
  - authorizationCode
  scope: recommendations.read
- description: Required to read personalized search results.
  flows:
  - authorizationCode
  scope: search.read
- description: Required to update personalized search results, e.g. delete search history.
  flows:
  - authorizationCode
  scope: search.write
- description: Read access to a user's account information, such as country and email address.
  flows:
  - authorizationCode
  scope: user.read
- description: Write user
  flows:
  - authorizationCode
  scope: w_usr
slug: tidal-scopes
source_filename: tidal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tidal-catalog-api-openapi.yml, openapi/tidal-claims-api-openapi.yml, openapi/tidal-commerce-api-openapi.yml,\n  openapi/tidal-playback-api-openapi.yml, openapi/tidal-playlists-api-openapi.yml, openapi/tidal-recommendations-api-openapi.yml,\n  openapi/tidal-search-api-openapi.yml, openapi/tidal-social-api-openapi.yml, openapi/tidal-user-collections-api-openapi.yml,\n  openapi/tidal-users-api-openapi.yml\nschemes:\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-catalog-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-catalog-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n \
  \ description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-claims-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-claims-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-commerce-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n\
  - name: Client_Credentials\n  source: openapi/tidal-commerce-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-playback-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-playback-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-playlists-api-openapi.yml\n  flows:\n  -\
  \ flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-playlists-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-recommendations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-recommendations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-search-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-search-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-social-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n\
  \  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-social-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n- name: Authorization_Code_PKCE\n  source: openapi/tidal-user-collections-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-user-collections-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\n\
  - name: Authorization_Code_PKCE\n  source: openapi/tidal-users-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tidal.com/authorize\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-authorization-code\n- name: Client_Credentials\n  source: openapi/tidal-users-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tidal.com/v1/oauth2/token\n  description: See https://developer.tidal.com/documentation/authorization/authorization-client-credentials\nscopes:\n- scope: collection.read\n  description: Read access to a user's \"My Collection\".\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n\
  \  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: collection.write\n  description: Write access to a user's \"My Collection\".\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: entitlements.read\n  description: Read access to what functionality a user is entitled to access on TIDAL, such\n    as whether they can stream music, use DJ add-ons and similar.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n\
  \  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: playback\n  description: Required to play media content and control playback.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: playlists.read\n\
  \  description: Required to list playlists created by a user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: playlists.write\n  description: Write access to a user's playlists.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n\
  \  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: r_usr\n  description: Read access to all end user data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: recommendations.read\n  description: Read access to a user’s personal recommendations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n\
  \  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: search.read\n  description: Required to read personalized search results.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: search.write\n  description: Required to update personalized search results, e.g. delete search history.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n\
  \  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n- scope: user.read\n  description: Read access to a user's account information, such as country and email address.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n\
  - scope: w_usr\n  description: Write user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tidal-catalog-api-openapi.yml\n  - openapi/tidal-claims-api-openapi.yml\n  - openapi/tidal-commerce-api-openapi.yml\n  - openapi/tidal-playback-api-openapi.yml\n  - openapi/tidal-playlists-api-openapi.yml\n  - openapi/tidal-recommendations-api-openapi.yml\n  - openapi/tidal-search-api-openapi.yml\n  - openapi/tidal-social-api-openapi.yml\n  - openapi/tidal-user-collections-api-openapi.yml\n  - openapi/tidal-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/scopes/tidal-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Music
- Streaming
- Hi-Fi
- HiRes Lossless
- Audio
- Block
- Square
token_urls:
- https://auth.tidal.com/v1/oauth2/token
---
