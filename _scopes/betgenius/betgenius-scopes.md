---
api_specs:
- filename: betgenius-bookingv1-api-openapi.yml
  format: yaml
  label: BetGenius Booking V1 API
  slug: betgenius-bookingv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-bookingv1-api-openapi.yml
- filename: betgenius-bookingv2-api-openapi.yml
  format: yaml
  label: BetGenius Booking V2 API
  slug: betgenius-bookingv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-bookingv2-api-openapi.yml
- filename: betgenius-fixtures-api-openapi.yml
  format: yaml
  label: BetGenius Fixtures API
  slug: betgenius-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-fixtures-api-openapi.yml
- filename: betgenius-regions-api-openapi.yml
  format: yaml
  label: BetGenius Regions API
  slug: betgenius-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-regions-api-openapi.yml
authorization_urls: []
description: ''
docs: https://geniussports.atlassian.net/wiki/spaces/BID/pages/3925901961/Match+State+Platform+APIs+Authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Betgenius Scopes
name_suffix: OAuth Scopes
note: 'Genius Sports publishes no scopes reference page. `derive-oauth-scopes.py` found nothing, because none of the three OpenAPI files in openapi/ declares an oauth2 securityScheme — Booking uses HTTP Basic and Video-v3 uses a Cognito authorizer modelled as an apiKey. The scopes below are the ones the platform actually issues: they were read out of the decoded `scope` claim of the example access token the BetGenius Integration Documents publish on the authentication page. They are therefore real, provider-published values, but they are an EXAMPLE token''s grant — not a complete catalogue, and the descriptions are read from the endpoint each scope guards, not from a provider-written definition. Treat this as evidence that the scope model exists and what its naming convention is, not as an exhaustive list.'
overview: 'BetGenius publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the BetGenius API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BetGenius
provider_slug: betgenius
schemes: []
scope_count: 10
scope_names:
- matchstateapi/global
- matchstateapi/live.read
- matchstateapi/live.post
- matchstateapi/schedule.read
- matchstateapi/schedule.post
- matchstateapi/granularity.read
- matchstateapi/granularity.post
- matchstateapi/sport.10
- matchstateapi/source.livestats
- matchstateapi/source.isd
scopes:
- description: Global access marker on the Match State Platform resource server.
  flows: []
  scope: matchstateapi/global
- description: Read live match state / live access tokens.
  flows: []
  scope: matchstateapi/live.read
- description: Publish live match state (feed-provider side).
  flows: []
  scope: matchstateapi/live.post
- description: Read the fixture coverage schedule (Schedule API GET).
  flows: []
  scope: matchstateapi/schedule.read
- description: Publish fixture coverage schedule entries (feed-provider side).
  flows: []
  scope: matchstateapi/schedule.post
- description: Read match-state source-id granularity settings.
  flows: []
  scope: matchstateapi/granularity.read
- description: Write match-state source-id granularity settings.
  flows: []
  scope: matchstateapi/granularity.post
- description: Per-sport entitlement — sport id 10 is Football (soccer). Sport entitlements are granted individually.
  flows: []
  scope: matchstateapi/sport.10
- description: Per-source entitlement for the LiveStats data source.
  flows: []
  scope: matchstateapi/source.livestats
- description: Per-source entitlement for the ISD data source.
  flows: []
  scope: matchstateapi/source.isd
slug: betgenius-scopes
source_filename: betgenius-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://geniussports.atlassian.net/wiki/spaces/BID/pages/3925901961/Match+State+Platform+APIs+Authentication\ndocs: https://geniussports.atlassian.net/wiki/spaces/BID/pages/3925901961/Match+State+Platform+APIs+Authentication\nnote: >-\n  Genius Sports publishes no scopes reference page. `derive-oauth-scopes.py` found nothing, because\n  none of the three OpenAPI files in openapi/ declares an oauth2 securityScheme — Booking uses HTTP\n  Basic and Video-v3 uses a Cognito authorizer modelled as an apiKey. The scopes below are the ones\n  the platform actually issues: they were read out of the decoded `scope` claim of the example\n  access token the BetGenius Integration Documents publish on the authentication page. They are\n  therefore real, provider-published values, but they are an EXAMPLE token's grant — not a complete\n  catalogue, and the descriptions are read from the endpoint each scope guards, not from a\n  provider-written\
  \ definition. Treat this as evidence that the scope model exists and what its\n  naming convention is, not as an exhaustive list.\nscheme:\n  name: OAuth2\n  flow: clientCredentials\n  token_url: https://auth.api.geniussports.com/oauth2/token\n  issuer: Amazon Cognito user pool in eu-west-1 (cognito-idp.eu-west-1.amazonaws.com)\n  applies_to: Match State Platform APIs, Access Control API, Schedule API, Statistics API\nnaming_convention: '<resource-server>/<resource>.<action>  e.g. matchstateapi/schedule.read'\ncompleteness: partial\nscopes:\n  - scope: matchstateapi/global\n    description: Global access marker on the Match State Platform resource server.\n  - scope: matchstateapi/live.read\n    description: Read live match state / live access tokens.\n  - scope: matchstateapi/live.post\n    description: Publish live match state (feed-provider side).\n  - scope: matchstateapi/schedule.read\n    description: Read the fixture coverage schedule (Schedule API GET).\n  - scope: matchstateapi/schedule.post\n\
  \    description: Publish fixture coverage schedule entries (feed-provider side).\n  - scope: matchstateapi/granularity.read\n    description: Read match-state source-id granularity settings.\n  - scope: matchstateapi/granularity.post\n    description: Write match-state source-id granularity settings.\n  - scope: matchstateapi/sport.10\n    description: Per-sport entitlement — sport id 10 is Football (soccer). Sport entitlements are granted individually.\n  - scope: matchstateapi/source.livestats\n    description: Per-source entitlement for the LiveStats data source.\n  - scope: matchstateapi/source.isd\n    description: Per-source entitlement for the ISD data source.\nobservations:\n  - >-\n    Entitlement is two-dimensional: a client is granted resource scopes (live/schedule/granularity,\n    read vs post) AND scalar entitlement scopes for each sport (`sport.<id>`) and each data source\n    (`source.<name>`). A sportsbook licensed for Football but not American Football carries\n    `sport.10`\
  \ and not `sport.17`.\n  - >-\n    Scopes are not requested per-call — the client_credentials grant returns whatever the issued\n    client is entitled to. There is no consent screen and no scope negotiation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/scopes/betgenius-scopes.yml
summary_line: 10 scopes
tags:
- Sportsbook
- Sports Betting
- Sports Data
- Odds Feeds
- Trading Services
- Risk Management
- Live Streaming
- In-Play Betting
- BetBuilder
- Player Engagement
- Marketing Technology
- Gambling
token_urls: []
---
