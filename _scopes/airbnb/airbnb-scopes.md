---
api_specs:
- filename: airbnb-homes-api-openapi.yml
  format: yaml
  label: Airbnb Homes API
  slug: homes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-homes-api-openapi.yml
- filename: airbnb-activities-api-openapi.yml
  format: yaml
  label: Airbnb Activities API
  slug: activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-activities-api-openapi.yml
- filename: airbnb-webhooks-asyncapi.yml
  format: yaml
  label: Airbnb Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/asyncapi/airbnb-webhooks-asyncapi.yml
authorization_urls:
- https://www.airbnb.com/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Airbnb Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'airbnb publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the airbnb API on a user''s behalf.


  Tokens are issued from https://api.airbnb.com/v2/oauth2/authorizations.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: airbnb
provider_slug: airbnb
schemes:
- description: Airbnb uses OAuth 2.0 for authentication. Partners must register their application to receive a client ID and secret, then obtain access tokens through the authorization code flow.
  flows:
  - authorizationUrl: https://www.airbnb.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://api.airbnb.com/v2/oauth2/authorizations
  name: oauth2
  source: openapi/airbnb-activities-api-openapi.yml
- description: Airbnb uses OAuth 2.0 for authentication. Partners must register their application to receive a client ID and secret, then obtain access tokens through the authorization code flow. Access tokens expire after 24 hours and must be refreshed.
  flows:
  - authorizationUrl: https://www.airbnb.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://api.airbnb.com/v2/oauth2/authorizations
  name: oauth2
  source: openapi/airbnb-homes-api-openapi.yml
scope_count: 13
scope_names:
- bookings:read
- bookings:write
- calendar:read
- calendar:write
- experiences:read
- experiences:write
- listings:read
- listings:write
- messages:read
- messages:write
- reservations:read
- reservations:write
- reviews:read
scopes:
- description: Read booking information
  flows:
  - authorizationCode
  scope: bookings:read
- description: Confirm and cancel bookings
  flows:
  - authorizationCode
  scope: bookings:write
- description: Read calendar availability
  flows:
  - authorizationCode
  scope: calendar:read
- description: Update calendar availability and pricing
  flows:
  - authorizationCode
  scope: calendar:write
- description: Read experience information
  flows:
  - authorizationCode
  scope: experiences:read
- description: Create and update experiences
  flows:
  - authorizationCode
  scope: experiences:write
- description: Read listing information
  flows:
  - authorizationCode
  scope: listings:read
- description: Create and update listings
  flows:
  - authorizationCode
  scope: listings:write
- description: Read booking messages
  flows:
  - authorizationCode
  scope: messages:read
- description: Send messages to guests
  flows:
  - authorizationCode
  scope: messages:write
- description: Read reservation information
  flows:
  - authorizationCode
  scope: reservations:read
- description: Accept, deny, and cancel reservations
  flows:
  - authorizationCode
  scope: reservations:write
- description: Read reviews
  flows:
  - authorizationCode
  scope: reviews:read
slug: airbnb-scopes
source_filename: airbnb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airbnb-activities-api-openapi.yml, openapi/airbnb-homes-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/airbnb-activities-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.airbnb.com/oauth2/auth\n    tokenUrl: https://api.airbnb.com/v2/oauth2/authorizations\n  description: Airbnb uses OAuth 2.0 for authentication. Partners must register their application\n    to receive a client ID and secret, then obtain access tokens through the authorization code\n    flow.\n- name: oauth2\n  source: openapi/airbnb-homes-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.airbnb.com/oauth2/auth\n    tokenUrl: https://api.airbnb.com/v2/oauth2/authorizations\n  description: Airbnb uses OAuth 2.0 for authentication. Partners must register their application\n    to receive a client ID and secret, then obtain access tokens through the authorization\
  \ code\n    flow. Access tokens expire after 24 hours and must be refreshed.\nscopes:\n- scope: bookings:read\n  description: Read booking information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-activities-api-openapi.yml\n- scope: bookings:write\n  description: Confirm and cancel bookings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-activities-api-openapi.yml\n- scope: calendar:read\n  description: Read calendar availability\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-homes-api-openapi.yml\n- scope: calendar:write\n  description: Update calendar availability and pricing\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-homes-api-openapi.yml\n- scope: experiences:read\n  description: Read experience information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-activities-api-openapi.yml\n- scope: experiences:write\n  description: Create and update experiences\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/airbnb-activities-api-openapi.yml\n- scope: listings:read\n  description: Read listing information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-homes-api-openapi.yml\n- scope: listings:write\n  description: Create and update listings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-homes-api-openapi.yml\n- scope: messages:read\n  description: Read booking messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-activities-api-openapi.yml\n  - openapi/airbnb-homes-api-openapi.yml\n- scope: messages:write\n  description: Send messages to guests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-activities-api-openapi.yml\n  - openapi/airbnb-homes-api-openapi.yml\n- scope: reservations:read\n  description: Read reservation information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-homes-api-openapi.yml\n- scope: reservations:write\n  description: Accept, deny, and cancel reservations\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-homes-api-openapi.yml\n- scope: reviews:read\n  description: Read reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/airbnb-homes-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/scopes/airbnb-scopes.yml
summary_line: 13 scopes · authorizationCode
tags: []
token_urls:
- https://api.airbnb.com/v2/oauth2/authorizations
---
