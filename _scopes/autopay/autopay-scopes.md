---
api_specs:
- filename: autopay-accounting-api-openapi.yml
  format: yaml
  label: Autopay Accounting API
  slug: autopay-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-accounting-api-openapi.yml
- filename: autopay-booking-api-openapi.yml
  format: yaml
  label: Autopay Booking API
  slug: autopay-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-booking-api-openapi.yml
- filename: autopay-customer-club-api-openapi.yml
  format: yaml
  label: Autopay Customer Club API
  slug: autopay-customer-club-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-customer-club-api-openapi.yml
- filename: autopay-fleet-api-openapi.yml
  format: yaml
  label: Autopay Fleet API
  slug: autopay-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-fleet-api-openapi.yml
- filename: autopay-parking-api-openapi.yml
  format: yaml
  label: Autopay Parking API
  slug: autopay-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-parking-api-openapi.yml
- filename: autopay-payment-api-openapi.yml
  format: yaml
  label: Autopay Payment API
  slug: autopay-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-payment-api-openapi.yml
- filename: autopay-permit-api-openapi.yml
  format: yaml
  label: Autopay Permit API
  slug: autopay-permit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-permit-api-openapi.yml
- filename: autopay-statistics-api-openapi.yml
  format: yaml
  label: Autopay Statistics API
  slug: autopay-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-statistics-api-openapi.yml
- filename: autopay-status-api-openapi.yml
  format: yaml
  label: Autopay Status API
  slug: autopay-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-status-api-openapi.yml
- filename: autopay-vehicle-api-openapi.yml
  format: yaml
  label: Autopay Vehicle API
  slug: autopay-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-vehicle-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Autopay Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Autopay publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Autopay API on a user''s behalf.


  Tokens are issued from https://api-auth.autopay.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Autopay
provider_slug: autopay
schemes:
- description: OAuth 2.0 Client Credentials flow. Tokens are minted from the Auth0 token endpoint and used as Bearer tokens with `audience` set to `https://api.autopay.io`. Some endpoints require specific scopes such as `permit_booking`, `customer_club`, or `zone_status`.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-auth.autopay.io/oauth/token
  name: OAuth2
  source: openapi/autopay-openapi.yml
scope_count: 3
scope_names:
- customer_club
- permit_booking
- zone_status
scopes:
- description: Required for Customer Club API operations
  flows:
  - clientCredentials
  scope: customer_club
- description: Required for Booking API operations
  flows:
  - clientCredentials
  scope: permit_booking
- description: Required for Status API operations
  flows:
  - clientCredentials
  scope: zone_status
slug: autopay-scopes
source_filename: autopay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/autopay-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/autopay-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-auth.autopay.io/oauth/token\n  description: OAuth 2.0 Client Credentials flow. Tokens are minted from the Auth0 token endpoint\n    and used as Bearer tokens with `audience` set to `https://api.autopay.io`. Some endpoints\n    require specific scopes such as `permit_booking`, `customer_club`, or `zone_status`.\nscopes:\n- scope: customer_club\n  description: Required for Customer Club API operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/autopay-openapi.yml\n- scope: permit_booking\n  description: Required for Booking API operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/autopay-openapi.yml\n- scope: zone_status\n  description: Required for Status API operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/autopay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/scopes/autopay-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Parking
- Parking Payments
- Fleet Management
- Permits
- Parking Operators
- Norway
token_urls:
- https://api-auth.autopay.io/oauth/token
---
