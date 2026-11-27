---
api_specs:
- filename: nogpets-com-account-api-openapi.yml
  format: yaml
  label: NogPets Account API
  slug: nogpets-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-account-api-openapi.yml
- filename: nogpets-com-booking-api-openapi.yml
  format: yaml
  label: NogPets Booking API
  slug: nogpets-com-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-booking-api-openapi.yml
- filename: nogpets-com-business-api-openapi.yml
  format: yaml
  label: NogPets Business API
  slug: nogpets-com-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-business-api-openapi.yml
- filename: nogpets-com-directory-api-openapi.yml
  format: yaml
  label: NogPets Directory API
  slug: nogpets-com-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-directory-api-openapi.yml
- filename: nogpets-com-run-api-openapi.yml
  format: yaml
  label: NogPets Run API
  slug: nogpets-com-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-run-api-openapi.yml
- filename: nogpets-com-services-api-openapi.yml
  format: yaml
  label: NogPets Services API
  slug: nogpets-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-services-api-openapi.yml
- filename: nogpets-com-shop-api-openapi.yml
  format: yaml
  label: NogPets Shop API
  slug: nogpets-com-shop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogpets-com/openapi/nogpets-com-shop-api-openapi.yml
authorization_urls:
- https://api.nogpets.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: NogPets Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NogPets publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the NogPets API on a user''s behalf.


  Tokens are issued from https://api.nogpets.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NogPets
provider_slug: nogpets-com
schemes:
- description: OAuth 2.1, authorization code with PKCE (S256), public clients. Register with `POST /oauth/register` (RFC 7591). Access tokens last an hour; refresh tokens rotate.
  flows:
  - authorizationUrl: https://api.nogpets.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.nogpets.com/oauth/token
  name: oauth2
  source: openapi/nogpets-com-openapi.json
scope_count: 8
scope_names:
- addresses
- bookings:read
- bookings:write
- business:manage
- business:write
- orders:write
- pets
- profile
scopes:
- description: See and add your addresses
  flows:
  - authorizationCode
  scope: addresses
- description: See your bookings
  flows:
  - authorizationCode
  scope: bookings:read
- description: Book, move, cancel and get payment links for your bookings
  flows:
  - authorizationCode
  scope: bookings:write
- description: Run your pet business on NogPets
  flows:
  - authorizationCode
  scope: business:manage
- description: Set up and manage your pet business on NogPets
  flows:
  - authorizationCode
  scope: business:write
- description: Place shop orders for you to pay
  flows:
  - authorizationCode
  scope: orders:write
- description: See and add your pets
  flows:
  - authorizationCode
  scope: pets
- description: See your name, email and phone
  flows:
  - authorizationCode
  scope: profile
slug: nogpets-com-scopes
source_filename: nogpets-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nogpets-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/nogpets-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.nogpets.com/oauth/authorize\n    tokenUrl: https://api.nogpets.com/oauth/token\n  description: OAuth 2.1, authorization code with PKCE (S256), public clients. Register with\n    `POST /oauth/register` (RFC 7591). Access tokens last an hour; refresh tokens rotate.\nscopes:\n- scope: addresses\n  description: See and add your addresses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nogpets-com-openapi.json\n- scope: bookings:read\n  description: See your bookings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nogpets-com-openapi.json\n- scope: bookings:write\n  description: Book, move, cancel and get payment links for your bookings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nogpets-com-openapi.json\n- scope: business:manage\n\
  \  description: Run your pet business on NogPets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nogpets-com-openapi.json\n- scope: business:write\n  description: Set up and manage your pet business on NogPets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nogpets-com-openapi.json\n- scope: orders:write\n  description: Place shop orders for you to pay\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nogpets-com-openapi.json\n- scope: pets\n  description: See and add your pets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nogpets-com-openapi.json\n- scope: profile\n  description: See your name, email and phone\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nogpets-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nogpets-com/scopes/nogpets-com-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Grooming
- Dog Walks
- Pet Sitting
- Pet Services
- WhatsApp Booking
- South Africa
token_bound: false
token_urls:
- https://api.nogpets.com/oauth/token
---
