---
api_specs:
- filename: maersk-line-airbookings-api-openapi.yml
  format: yaml
  label: Maersk AirBookings API
  slug: maersk-line-airbookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-airbookings-api-openapi.yml
- filename: maersk-line-billoflading-api-openapi.yml
  format: yaml
  label: Maersk BillOfLading API
  slug: maersk-line-billoflading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-billoflading-api-openapi.yml
- filename: maersk-line-bookings-api-openapi.yml
  format: yaml
  label: Maersk Bookings API
  slug: maersk-line-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-bookings-api-openapi.yml
- filename: maersk-line-containers-api-openapi.yml
  format: yaml
  label: Maersk Containers API
  slug: maersk-line-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-containers-api-openapi.yml
- filename: maersk-line-demurragedetention-api-openapi.yml
  format: yaml
  label: Maersk DemurrageDetention API
  slug: maersk-line-demurragedetention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-demurragedetention-api-openapi.yml
- filename: maersk-line-locations-api-openapi.yml
  format: yaml
  label: Maersk Locations API
  slug: maersk-line-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-locations-api-openapi.yml
- filename: maersk-line-offers-api-openapi.yml
  format: yaml
  label: Maersk Offers API
  slug: maersk-line-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-offers-api-openapi.yml
- filename: maersk-line-schedules-api-openapi.yml
  format: yaml
  label: Maersk Schedules API
  slug: maersk-line-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-schedules-api-openapi.yml
- filename: maersk-line-tracking-api-openapi.yml
  format: yaml
  label: Maersk Tracking API
  slug: maersk-line-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-tracking-api-openapi.yml
- filename: maersk-line-vgm-api-openapi.yml
  format: yaml
  label: Maersk VGM API
  slug: maersk-line-vgm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-vgm-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Maersk Line Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Maersk publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Maersk API on a user''s behalf.


  Tokens are issued from https://api.maersk.com/customer-identity/oauth/v2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Maersk
provider_slug: maersk-line
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token
  name: OAuth2
  source: openapi/maersk-bill-of-lading-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token
  name: OAuth2
  source: openapi/maersk-ocean-booking-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token
  name: OAuth2
  source: openapi/maersk-track-and-trace-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token
  name: OAuth2
  source: openapi/maersk-vgm-api-openapi.yml
scope_count: 4
scope_names:
- booking
- ebl
- read
- vgm
scopes:
- description: Manage bookings.
  flows:
  - clientCredentials
  scope: booking
- description: Read and update eBL documents.
  flows:
  - clientCredentials
  scope: ebl
- description: Read access to tracking data.
  flows:
  - clientCredentials
  scope: read
- description: Submit VGM declarations.
  flows:
  - clientCredentials
  scope: vgm
slug: maersk-line-scopes
source_filename: maersk-line-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maersk-bill-of-lading-api-openapi.yml, openapi/maersk-ocean-booking-api-openapi.yml,\n  openapi/maersk-track-and-trace-api-openapi.yml, openapi/maersk-vgm-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/maersk-bill-of-lading-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token\n- name: OAuth2\n  source: openapi/maersk-ocean-booking-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token\n- name: OAuth2\n  source: openapi/maersk-track-and-trace-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token\n- name: OAuth2\n  source: openapi/maersk-vgm-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.maersk.com/customer-identity/oauth/v2/access_token\n\
  scopes:\n- scope: booking\n  description: Manage bookings.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/maersk-ocean-booking-api-openapi.yml\n- scope: ebl\n  description: Read and update eBL documents.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/maersk-bill-of-lading-api-openapi.yml\n- scope: read\n  description: Read access to tracking data.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/maersk-track-and-trace-api-openapi.yml\n- scope: vgm\n  description: Submit VGM declarations.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/maersk-vgm-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/scopes/maersk-line-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Shipping
- Logistics
- Container Shipping
- Ocean Freight
- Air Freight
- Supply Chain
- DCSA
- Maritime
token_urls:
- https://api.maersk.com/customer-identity/oauth/v2/access_token
---
