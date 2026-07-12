---
authorization_urls:
- https://thewall.tibber.com/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Tibber Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tibber publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tibber API on a user''s behalf.


  Tokens are issued from https://thewall.tibber.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tibber
provider_slug: tibber
schemes:
- description: OAuth 2.0 Authorization Code Flow with optional PKCE.
  flows:
  - authorizationUrl: https://thewall.tibber.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://thewall.tibber.com/connect/token
  name: oauth2
  source: openapi/tibber-data-api-openapi.yml
scope_count: 11
scope_names:
- data-api-chargers-read
- data-api-energy-systems-read
- data-api-homes-read
- data-api-inverters-read
- data-api-thermostats-read
- data-api-user-read
- data-api-vehicles-read
- email
- offline_access
- openid
- profile
scopes:
- description: Read EV chargers and EVSE equipment.
  flows:
  - authorizationCode
  scope: data-api-chargers-read
- description: Read home batteries and hybrid systems.
  flows:
  - authorizationCode
  scope: data-api-energy-systems-read
- description: List the user's homes.
  flows:
  - authorizationCode
  scope: data-api-homes-read
- description: Read solar inverters.
  flows:
  - authorizationCode
  scope: data-api-inverters-read
- description: Read thermostats, heat pumps, and space heaters.
  flows:
  - authorizationCode
  scope: data-api-thermostats-read
- description: Basic user context (required baseline).
  flows:
  - authorizationCode
  scope: data-api-user-read
- description: Read connected electric vehicles.
  flows:
  - authorizationCode
  scope: data-api-vehicles-read
- description: User email.
  flows:
  - authorizationCode
  scope: email
- description: Issue refresh tokens.
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID identity.
  flows:
  - authorizationCode
  scope: openid
- description: User profile.
  flows:
  - authorizationCode
  scope: profile
slug: tibber-scopes
source_filename: tibber-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tibber-data-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/tibber-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://thewall.tibber.com/connect/authorize\n    tokenUrl: https://thewall.tibber.com/connect/token\n  description: OAuth 2.0 Authorization Code Flow with optional PKCE.\nscopes:\n- scope: data-api-chargers-read\n  description: Read EV chargers and EVSE equipment.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: data-api-energy-systems-read\n  description: Read home batteries and hybrid systems.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: data-api-homes-read\n  description: List the user's homes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: data-api-inverters-read\n  description: Read solar inverters.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: data-api-thermostats-read\n  description: Read thermostats, heat pumps, and space heaters.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: data-api-user-read\n  description: Basic user context (required baseline).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: data-api-vehicles-read\n  description: Read connected electric vehicles.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: email\n  description: User email.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: offline_access\n  description: Issue refresh tokens.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n- scope: openid\n  description: OpenID identity.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n\
  - scope: profile\n  description: User profile.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tibber-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/scopes/tibber-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Energy
- SmartHome
- SmartMeter
- ElectricityPricing
- ElectricVehicleCharging
- HeatPump
- SolarInverter
- HomeBattery
- GraphQL
- OAuth2
- Nordic
token_urls:
- https://thewall.tibber.com/connect/token
---
