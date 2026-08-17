---
api_specs:
- filename: splashthat-api.postman_collection.json
  format: json
  label: Splash API
  slug: splash-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/splashthat/refs/heads/main/postman/splashthat-api.postman_collection.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Splashthat Scopes
name_suffix: OAuth Scopes
note: 'Splash publishes no OpenAPI and no scopes/permissions reference page, so `derive-oauth-scopes.py` returns nothing. The single scope below is read directly from Splash''s own published token requests and token responses in the "Splash API v2.2" Postman collection: every Access Token and Refresh Token call sends `scope=user`, and every successful token response echoes `"scope": "user"`. No other scope value appears anywhere in the published contract. Splash''s authorization granularity is carried by ROLES and ADMIN PRIVILEGES on the account, not by OAuth scopes.'
overview: 'Splash publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Splash API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Splash
provider_slug: splashthat
schemes: []
scope_count: 1
scope_names:
- user
scopes:
- description: User-level access to the authenticated Splash account — the only scope Splash issues. Grants the token the same reach as the user whose username/password was exchanged, across events, group contacts, contacts, unsubscribes, team manager and forms.
  flows:
  - password
  - refreshToken
  scope: user
slug: splashthat-scopes
source_filename: splashthat-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api-docs.splashthat.com/\nartifact_source: postman/splashthat-api.postman_collection.json\nnote: >\n  Splash publishes no OpenAPI and no scopes/permissions reference page, so\n  `derive-oauth-scopes.py` returns nothing. The single scope below is read\n  directly from Splash's own published token requests and token responses in\n  the \"Splash API v2.2\" Postman collection: every Access Token and Refresh\n  Token call sends `scope=user`, and every successful token response echoes\n  `\"scope\": \"user\"`. No other scope value appears anywhere in the published\n  contract. Splash's authorization granularity is carried by ROLES and\n  ADMIN PRIVILEGES on the account, not by OAuth scopes.\nscheme: SplashOAuth2\ntoken_url: https://api.splashthat.com/oauth/v2/token\nscope_count: 1\nscopes:\n  - scope: user\n    description: >\n      User-level access to the authenticated Splash account — the only scope\n      Splash issues.\
  \ Grants the token the same reach as the user whose\n      username/password was exchanged, across events, group contacts, contacts,\n      unsubscribes, team manager and forms.\n    flows: [password, refreshToken]\n    sources:\n      - postman/splashthat-api.postman_collection.json#Authentication/Access Token\n      - postman/splashthat-api.postman_collection.json#Authentication/Refresh Token\nnon_scope_authorization:\n  - name: Organization admin privilege\n    controls: PUT /contacts/:contact_id/anonymize\n    failure_status: 403\n  - name: Team Users view permission\n    controls: GET /v1/team-manager/users\n    failure_status: 403\n  - name: Team Manager roles\n    note: >\n      Roles are first-class objects (GET /v1/team-manager/roles) assigned per\n      user with group scoping — this, not OAuth scope, is where Splash's\n      permission model actually lives.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splashthat/refs/heads/main/scopes/splashthat-scopes.yml
summary_line: 1 scope
tags:
- Events
- Event Marketing
- Event Management
- Guest Registration
- Ticketing
- Check-In
- Analytics
token_urls: []
---
