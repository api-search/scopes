---
authorization_urls: []
description: ''
docs: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Breeze Airways Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Breeze Airways uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/Selling/r3.x/Auth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Breeze Airways
provider_slug: breeze-airways
schemes:
- flows:
  - expires_in: 00:30:00
    flow: clientCredentials
    grant_type: client_credentials
    tokenUrl: /api/Selling/r3.x/Auth
  name: OAuth2ClientCredentials
  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication
scope_count: 0
scope_names: []
scopes: []
slug: breeze-airways-scopes
source_filename: breeze-airways-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\ndocs: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\napi: Breeze Airways NDC Gateway\nnotes: >-\n  Breeze does not publish a scopes or permissions reference page, and the token\n  request does not accept a scope parameter — the client-credentials exchange\n  returns a JWT whose aud (audience) claim enumerates the services the session is\n  authorized against. Those audience values are recorded below as the provider's\n  de facto authorization surface. They are token AUDIENCES, not requestable OAuth\n  scopes; nothing here is inferred beyond the sample tokens published on the Breeze\n  authentication documentation page.\nschemes:\n- name: OAuth2ClientCredentials\n  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/Selling/r3.x/Auth\n    grant_type: client_credentials\n\
  \    expires_in: 00:30:00\nscopes: []\ntoken_audiences:\n- audience: shopping\n  kind: jwt-aud-claim\n  description: Shopping routes — AirlineProfile and AirShopping.\n  routes:\n  - /api/Shopping/r3.x/v21.3/AirlineProfile\n  - /api/Shopping/r3.x/v21.3/AirShopping\n- audience: selling\n  kind: jwt-aud-claim\n  description: Selling routes — offer pricing, ancillary and seat selection, order creation.\n  routes:\n  - /api/Selling/r3.x/v21.3/OfferPrice\n  - /api/Selling/r3.x/v21.3/ServiceList\n  - /api/Selling/r3.x/v21.3/SeatAvailability\n  - /api/Selling/r3.x/v21.3/OrderCreate\n- audience: servicing\n  kind: jwt-aud-claim\n  description: Servicing routes — order retrieve, quote, reshop and change.\n  routes:\n  - /api/Servicing/r3.x/v21.3/OrderRetrieve\n  - /api/Servicing/r3.x/v21.3/OrderQuote\n  - /api/Servicing/r3.x/v21.3/OrderReshop\n  - /api/Servicing/r3.x/v21.3/OrderChange\n  - /api/Servicing/r3.x/v21.3/ServiceList\n  - /api/Servicing/r3.x/v21.3/SeatAvailability\n- audience: orderchangenotification\n\
  \  kind: jwt-aud-claim\n  description: >-\n    Order change notification audience present in every issued token. Breeze\n    publishes no documentation for a notification/push surface at the B2B portal,\n    so the delivery contract for this audience is undocumented publicly.\n  routes: []\nrole_codes:\n  parameter: role\n  applies_to: /api/Selling/r3.x/Auth?role={rolecode}\n  observed_values:\n  - NDCO\n  description: >-\n    An optional role code narrows the token to a reservation-system agent role and\n    halves the token request latency. NDCO is the role code visible in the published\n    sample tokens. Breeze publishes no full role-code reference; codes are issued\n    per partner.\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze-airways/refs/heads/main/scopes/breeze-airways-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Airlines
- Travel
- Aviation
- NDC
- Distribution
- Booking
- Reservations
- Travel Agencies
- IATA
token_urls:
- /api/Selling/r3.x/Auth
---
