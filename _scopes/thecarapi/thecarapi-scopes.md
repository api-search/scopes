---
api_specs:
- filename: openapi.json
  format: json
  label: TheCarApi REST API
  slug: thecarapi-rest-api
  spec_type: OpenAPI
  url: https://thecarapi.com/openapi.json
authorization_urls: []
description: ''
docs: https://thecarapi.com/docs/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Thecarapi Scopes
name_suffix: OAuth Scopes
note: TheCarApi publishes a real, named scope reference, but the scopes are attached to an API key rather than issued through an OAuth2 authorization flow. There are no oauth2 securitySchemes in the OpenAPI and no authorization/token endpoints. Scopes are granted per endpoint by the operator; a request to a route the key does not cover returns 403.
overview: 'TheCarApi uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TheCarApi
provider_slug: thecarapi
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: thecarapi-scopes
source_filename: thecarapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://thecarapi.com/docs/authentication\ndocs: https://thecarapi.com/docs/authentication\nmodel: api-key-scopes\noauth2: false\nnote: >-\n  TheCarApi publishes a real, named scope reference, but the scopes are attached to an API key\n  rather than issued through an OAuth2 authorization flow. There are no oauth2 securitySchemes in\n  the OpenAPI and no authorization/token endpoints. Scopes are granted per endpoint by the\n  operator; a request to a route the key does not cover returns 403.\nwildcard: '*'\nwildcard_note: '`*` grants every route. A scope may also be a literal URL rule rather than a group.'\nscope_count: 10\nscopes:\n  - name: search\n    description: Inventory search, filter facets (individually or combined via /api/facets), sources, and the full model catalog.\n  - name: catalog\n    description: Manufacturer and model-group catalog.\n  - name: seo\n    description: Popular searches and brand/model slug resolution.\n\
  \  - name: auctions\n    description: Auction detail, images, price history, and VIN history.\n  - name: details\n    description: Full vehicle details, including upstream fetches.\n  - name: top-offers\n    description: Auctions priced below their market reference.\n  - name: theparking\n    description: European classifieds feed, facets, and models.\n  - name: market\n    description: Cars.bg and auction market price snapshots.\n  - name: calculator\n    description: Import cost calculator and supported countries.\n  - name: ops\n    description: >-\n      Service health, the contract, and the API index. The provider warns that this group also\n      covers internal routes outside the published contract, which are unversioned and may change\n      without a changelog entry.\nlegacy_scopes:\n  - name: public\n    status: legacy-compatibility\n    description: >-\n      Legacy compatibility bundle — search facets, catalog, SEO, auctions, calculator and health —\n      preserved for older\
  \ integrations. New keys are issued against the groups above.\ndefault_grant:\n  enabled_by_default:\n    - /api/search\n    - /api/brands\n    - /api/models\n    - /api/years\n    - /api/fuels\n    - /api/countries\n    - /api/gearboxes\n    - /api/sites\n    - /load-models\n    - /api/facets\n    - /api/catalog/*\n    - /api/seo/*\n    - /api/auction/*\n    - /api/auction-images/*\n    - /api/calculator/*\n    - /api/top-offers\n    - /api/theparking/*\n    - /api/car-details\n    - /api/contract\n    - /api/health\n    - /\n  granted_on_request:\n    - /api/vin/{vin}/history\n    - /api/cars-bg-market\n    - /api/auction-market\n    - /api/listVehicles\n    - /listVehicles\n    - /api/search/auction-ids\n  no_key_required:\n    - /api/health/live\n    - /api/health/ready\ndiscovery:\n  startup_check: GET /api/contract\n  guidance: >-\n    The provider tells clients to call /api/contract once at process start and fail loudly if the\n    surface they depend on is absent — a missing scope\
  \ is a deployment problem, not a runtime one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecarapi/refs/heads/main/scopes/thecarapi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Automotive
- Vehicle Data
- Car Auctions
- Used Cars
- Vehicle Inventory
- Classifieds
- Market Intelligence
- Pricing
- VIN
- Image CDN
- Europe
- Korea
- Japan Auctions
token_urls: []
---
