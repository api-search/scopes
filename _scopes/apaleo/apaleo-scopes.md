---
api_specs:
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Booking API
  slug: booking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Rate Plan API
  slug: rateplan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Finance API
  slug: finance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Settings API
  slug: settings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
- filename: apaleo-openapi.yml
  format: yaml
  label: apaleo Webhook API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/openapi/apaleo-openapi.yml
authorization_urls:
- https://identity.apaleo.com/connect/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Apaleo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'apaleo publishes 10 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the apaleo API on a user''s behalf.


  Tokens are issued from https://identity.apaleo.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: apaleo
provider_slug: apaleo
schemes:
- description: apaleo uses OAuth 2.0. Obtain a bearer access token from the apaleo identity provider and send it in the Authorization header as 'Bearer {token}'. The client-credentials and authorization-code grants are supported.
  flows:
  - flow: clientCredentials
    tokenUrl: https://identity.apaleo.com/connect/token
  - authorizationUrl: https://identity.apaleo.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.apaleo.com/connect/token
  name: oauth2
  source: openapi/apaleo-openapi.yml
scope_count: 10
scope_names:
- availability.manage
- availability.read
- folios.manage
- folios.read
- rates.manage
- rates.read
- reservations.manage
- reservations.read
- setup.manage
- setup.read
scopes:
- description: Manage availability
  flows:
  - authorizationCode
  - clientCredentials
  scope: availability.manage
- description: Read availability
  flows:
  - authorizationCode
  - clientCredentials
  scope: availability.read
- description: Manage folios, payments, and invoices
  flows:
  - authorizationCode
  - clientCredentials
  scope: folios.manage
- description: Read folios and finance data
  flows:
  - authorizationCode
  - clientCredentials
  scope: folios.read
- description: Manage rate plans and rates
  flows:
  - authorizationCode
  - clientCredentials
  scope: rates.manage
- description: Read rate plans and rates
  flows:
  - authorizationCode
  - clientCredentials
  scope: rates.read
- description: Create and manage reservations and bookings
  flows:
  - authorizationCode
  - clientCredentials
  scope: reservations.manage
- description: Read reservations and bookings
  flows:
  - authorizationCode
  - clientCredentials
  scope: reservations.read
- description: Manage inventory and configuration
  flows:
  - authorizationCode
  - clientCredentials
  scope: setup.manage
- description: Read inventory and configuration
  flows:
  - authorizationCode
  - clientCredentials
  scope: setup.read
slug: apaleo-scopes
source_filename: apaleo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apaleo-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/apaleo-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.apaleo.com/connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://identity.apaleo.com/connect/authorize\n    tokenUrl: https://identity.apaleo.com/connect/token\n  description: apaleo uses OAuth 2.0. Obtain a bearer access token from the apaleo identity\n    provider and send it in the Authorization header as 'Bearer {token}'. The client-credentials\n    and authorization-code grants are supported.\nscopes:\n- scope: availability.manage\n  description: Manage availability\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n- scope: availability.read\n  description: Read availability\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n- scope: folios.manage\n\
  \  description: Manage folios, payments, and invoices\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n- scope: folios.read\n  description: Read folios and finance data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n- scope: rates.manage\n  description: Manage rate plans and rates\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n- scope: rates.read\n  description: Read rate plans and rates\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n- scope: reservations.manage\n  description: Create and manage reservations and bookings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n- scope: reservations.read\n  description: Read reservations and bookings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n\
  - scope: setup.manage\n  description: Manage inventory and configuration\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n- scope: setup.read\n  description: Read inventory and configuration\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/apaleo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apaleo/refs/heads/main/scopes/apaleo-scopes.yml
summary_line: 10 scopes · clientCredentials/authorizationCode
tags:
- Hospitality
- PMS
- Property Management
- Hotels
- API-First
token_urls:
- https://identity.apaleo.com/connect/token
---
