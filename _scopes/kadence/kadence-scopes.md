---
api_specs:
- filename: kadence-bookable-day-api-openapi.yml
  format: yaml
  label: Kadence Bookable Day API
  slug: kadence-bookable-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-day-api-openapi.yml
- filename: kadence-bookable-onsite-pass-api-openapi.yml
  format: yaml
  label: Kadence Bookable Onsite Pass API
  slug: kadence-bookable-onsite-pass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-onsite-pass-api-openapi.yml
- filename: kadence-bookable-space-api-openapi.yml
  format: yaml
  label: Kadence Bookable Space API
  slug: kadence-bookable-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-bookable-space-api-openapi.yml
- filename: kadence-booking-api-openapi.yml
  format: yaml
  label: Kadence Booking API
  slug: kadence-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-booking-api-openapi.yml
- filename: kadence-building-api-openapi.yml
  format: yaml
  label: Kadence Building API
  slug: kadence-building-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-building-api-openapi.yml
- filename: kadence-floor-api-openapi.yml
  format: yaml
  label: Kadence Floor API
  slug: kadence-floor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-floor-api-openapi.yml
- filename: kadence-neighborhood-api-openapi.yml
  format: yaml
  label: Kadence Neighborhood API
  slug: kadence-neighborhood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-neighborhood-api-openapi.yml
- filename: kadence-space-api-openapi.yml
  format: yaml
  label: Kadence Space API
  slug: kadence-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-space-api-openapi.yml
- filename: kadence-user-api-openapi.yml
  format: yaml
  label: Kadence User API
  slug: kadence-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-user-api-openapi.yml
- filename: kadence-visit-api-openapi.yml
  format: yaml
  label: Kadence Visit API
  slug: kadence-visit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-visit-api-openapi.yml
- filename: kadence-visitor-api-openapi.yml
  format: yaml
  label: Kadence Visitor API
  slug: kadence-visitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-visitor-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Kadence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kadence publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kadence API on a user''s behalf.


  Tokens are issued from https://login.onkadence.co/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kadence
provider_slug: kadence
schemes:
- description: OAuth 2.0 client credentials Grant
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.onkadence.co/oauth2/token
  name: oauth
  source: openapi/kadence-public-api-openapi.yml
scope_count: 1
scope_names:
- public
scopes:
- description: Public API access
  flows:
  - clientCredentials
  scope: public
slug: kadence-scopes
source_filename: kadence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kadence-public-api-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/kadence-public-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.onkadence.co/oauth2/token\n  description: OAuth 2.0 client credentials Grant\nscopes:\n- scope: public\n  description: Public API access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/kadence-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/scopes/kadence-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Workplace
- Hybrid Work
- Desk Booking
- Room Booking
- Space Management
- Visitor Management
- Workplace Analytics
- Facilities
- Authentication
token_urls:
- https://login.onkadence.co/oauth2/token
---
