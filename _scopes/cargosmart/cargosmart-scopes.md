---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cargosmart Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CargoSmart publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CargoSmart API on a user''s behalf.


  Tokens are issued from https://auth.cargosmart.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CargoSmart
provider_slug: cargosmart
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.cargosmart.com/oauth/token
  name: oauth2
  source: openapi/cargosmart-shipment-tracking-openapi.yml
scope_count: 4
scope_names:
- bookings:read
- bookings:write
- documents:read
- tracking:read
scopes:
- description: Read booking data
  flows:
  - clientCredentials
  scope: bookings:read
- description: Create and manage bookings
  flows:
  - clientCredentials
  scope: bookings:write
- description: Read shipping documents
  flows:
  - clientCredentials
  scope: documents:read
- description: Read shipment tracking data
  flows:
  - clientCredentials
  scope: tracking:read
slug: cargosmart-scopes
source_filename: cargosmart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cargosmart-shipment-tracking-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cargosmart-shipment-tracking-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.cargosmart.com/oauth/token\nscopes:\n- scope: bookings:read\n  description: Read booking data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cargosmart-shipment-tracking-openapi.yml\n- scope: bookings:write\n  description: Create and manage bookings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cargosmart-shipment-tracking-openapi.yml\n- scope: documents:read\n  description: Read shipping documents\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cargosmart-shipment-tracking-openapi.yml\n- scope: tracking:read\n  description: Read shipment tracking data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cargosmart-shipment-tracking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/scopes/cargosmart-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Booking
- Container
- Documentation
- GSBN
- IQAX
- Logistics
- Maritime
- Ocean Freight
- Schedule
- Shipping
- Supply Chain
- Tracking
- Visibility
- Vessel
token_urls:
- https://auth.cargosmart.com/oauth/token
---
