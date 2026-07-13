---
api_specs:
- filename: hostaway-listings-api-openapi.yml
  format: yaml
  label: Hostaway Listings API
  slug: hostaway-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-listings-api-openapi.yml
- filename: hostaway-reservations-api-openapi.yml
  format: yaml
  label: Hostaway Reservations API
  slug: hostaway-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-reservations-api-openapi.yml
- filename: hostaway-calendar-api-openapi.yml
  format: yaml
  label: Hostaway Calendar API
  slug: hostaway-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-calendar-api-openapi.yml
- filename: hostaway-webhooks-api-openapi.yml
  format: yaml
  label: Hostaway Webhooks API
  slug: hostaway-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hostaway Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hostaway publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hostaway API on a user''s behalf.


  Tokens are issued from https://api.hostaway.com/v1/accessTokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hostaway
provider_slug: hostaway
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.hostaway.com/v1/accessTokens
  name: OAuth2ClientCredentials
  source: openapi/hostaway-calendar-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.hostaway.com/v1/accessTokens
  name: OAuth2ClientCredentials
  source: openapi/hostaway-listings-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.hostaway.com/v1/accessTokens
  name: OAuth2ClientCredentials
  source: openapi/hostaway-reservations-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.hostaway.com/v1/accessTokens
  name: OAuth2ClientCredentials
  source: openapi/hostaway-webhooks-api-openapi.yml
scope_count: 1
scope_names:
- general
scopes:
- description: General API access scope
  flows:
  - clientCredentials
  scope: general
slug: hostaway-scopes
source_filename: hostaway-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hostaway-calendar-api-openapi.yml, openapi/hostaway-listings-api-openapi.yml,\n  openapi/hostaway-reservations-api-openapi.yml, openapi/hostaway-webhooks-api-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/hostaway-calendar-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hostaway.com/v1/accessTokens\n- name: OAuth2ClientCredentials\n  source: openapi/hostaway-listings-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hostaway.com/v1/accessTokens\n- name: OAuth2ClientCredentials\n  source: openapi/hostaway-reservations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hostaway.com/v1/accessTokens\n- name: OAuth2ClientCredentials\n  source: openapi/hostaway-webhooks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hostaway.com/v1/accessTokens\nscopes:\n- scope: general\n\
  \  description: General API access scope\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hostaway-calendar-api-openapi.yml\n  - openapi/hostaway-listings-api-openapi.yml\n  - openapi/hostaway-reservations-api-openapi.yml\n  - openapi/hostaway-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/scopes/hostaway-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Vacation Rentals
- Short-Term Rentals
- Property Management
- Channel Manager
- Airbnb
- Vrbo
- Booking.com
- Expedia
- SaaS
token_urls:
- https://api.hostaway.com/v1/accessTokens
---
