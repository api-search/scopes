---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hidden Road Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hidden Road uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hidden Road
provider_slug: hidden-road
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hidden-road-scopes
source_filename: hidden-road-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  https://portal.ops.hiddenroad.com/assets/index-b9a72e77.js (HTTP 200, unauthenticated\n  first-party bundle) and https://auth.hiddenroad.com/.well-known/openid-configuration (HTTP 200)\ndocs: null\ndocs_note: >-\n  Hidden Road publishes NO scopes or permissions reference. The API scopes below were read\n  verbatim out of the Operational Portal's own public JavaScript bundle, where they appear in\n  the Auth0 token request alongside audience \"https://api.hiddenroad.com/v0/\". Treat the list as\n  a floor, not a complete vocabulary: it is only the set the ops portal itself requests, so\n  scopes for the metrics (Risk) and atm (Automated Treasury Management) services are almost\n  certainly defined and simply not present in this bundle.\nauthorization_server: https://auth.hiddenroad.com/\naudience: https://api.hiddenroad.com/v0/\nflows:\n- client_credentials\n- authorization_code\napi_scopes:\n- scope: 'otc:read'\n  service:\
  \ otc\n  access: read\n  description: >-\n    Read access to the OTC surface under https://api.hiddenroad.com/v0/otc/. Verbatim from the\n    portal bundle; Hidden Road publishes no description of its own.\n- scope: 'otc:write'\n  service: otc\n  access: write\n  description: >-\n    Write access to the OTC surface. This is the only confirmed write scope on the API and the\n    reason the reversibility question in conventions/ matters for this provider.\n- scope: 'accountactivity:*'\n  service: accountactivity\n  access: wildcard\n  description: >-\n    Wildcard grant over the Account Activity API (balances, trades, positions, fees). A `*`\n    scope is coarse: an integrator cannot request read-only account activity with the vocabulary\n    as published.\noidc_scopes:\n  requested_by_portal: [openid, profile, email]\n  supported:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n\
  \  - identities\n  - phone\n  - address\nservices_without_published_scopes:\n- service: metrics\n  path: https://api.hiddenroad.com/v0/metrics/\n  product: Risk API\n  status: 401 (route confirmed live, scope vocabulary unknown)\n- service: atm\n  path: https://api.hiddenroad.com/v0/atm/\n  product: Automated Treasury Management API\n  status: 401 (route confirmed live, scope vocabulary unknown)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hidden-road/refs/heads/main/scopes/hidden-road-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Financial Services
- Prime Brokerage
- Clearing
- Digital Assets
- Foreign Exchange
- Capital Markets
- Trading
- Institutional Finance
- Collateral Management
- Risk Management
- Regulated
token_urls: []
---
