---
api_specs:
- filename: next-big-idea-club-members-openapi.yml
  format: yaml
  label: Next Big Idea Club Members API
  slug: next-big-idea-club-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/next-big-idea-club/refs/heads/main/openapi/next-big-idea-club-members-openapi.yml
authorization_urls:
- https://nextbigideaclub.com/oauth/authorize/
description: ''
docs: https://nextbigideaclub.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Next Big Idea Club Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Next Big Idea Club publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Next Big Idea Club API on a user''s behalf.


  Tokens are issued from https://nextbigideaclub.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Next Big Idea Club
provider_slug: next-big-idea-club
schemes:
- flows:
  - authorizationUrl: https://nextbigideaclub.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://nextbigideaclub.com/oauth/token/
  name: oauth2
  software: WP OAuth Server
  source: well-known/next-big-idea-club-openid-configuration.json
scope_count: 4
scope_names:
- openid
- profile
- email
- basic
scopes:
- description: Authenticate the user and return an OpenID Connect ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access the member's basic profile information.
  flows:
  - authorizationCode
  scope: profile
- description: Access the member's email address.
  flows:
  - authorizationCode
  scope: email
- description: Basic account access.
  flows:
  - authorizationCode
  scope: basic
slug: next-big-idea-club-scopes
source_filename: next-big-idea-club-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nextbigideaclub.com/.well-known/openid-configuration\ndocs: https://nextbigideaclub.com/.well-known/openid-configuration\nschemes:\n  - name: oauth2\n    software: WP OAuth Server\n    source: well-known/next-big-idea-club-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://nextbigideaclub.com/oauth/authorize/\n        tokenUrl: https://nextbigideaclub.com/oauth/token/\nscopes:\n  - scope: openid\n    description: Authenticate the user and return an OpenID Connect ID token.\n    flows: [authorizationCode]\n    sources: [well-known/next-big-idea-club-openid-configuration.json]\n  - scope: profile\n    description: Access the member's basic profile information.\n    flows: [authorizationCode]\n    sources: [well-known/next-big-idea-club-openid-configuration.json]\n  - scope: email\n    description: Access the member's email address.\n    flows: [authorizationCode]\n\
  \    sources: [well-known/next-big-idea-club-openid-configuration.json]\n  - scope: basic\n    description: Basic account access.\n    flows: [authorizationCode]\n    sources: [well-known/next-big-idea-club-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-big-idea-club/refs/heads/main/scopes/next-big-idea-club-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Books
- Media
- Subscription
- Nonfiction
- Podcast
- Education
- Membership
token_urls:
- https://nextbigideaclub.com/oauth/token/
---
