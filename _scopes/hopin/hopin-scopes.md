---
api_specs:
- filename: hopin-bank-questions-api-openapi.yml
  format: yaml
  label: RingCentral Events Bank Questions API
  slug: hopin-bank-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-bank-questions-api-openapi.yml
- filename: hopin-booths-api-openapi.yml
  format: yaml
  label: RingCentral Events Booths API
  slug: hopin-booths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-booths-api-openapi.yml
- filename: hopin-data-subscriptions-api-openapi.yml
  format: yaml
  label: RingCentral Events Data Subscriptions API
  slug: hopin-data-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-data-subscriptions-api-openapi.yml
- filename: hopin-events-api-openapi.yml
  format: yaml
  label: RingCentral Events Events API
  slug: hopin-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-events-api-openapi.yml
- filename: hopin-health-api-openapi.yml
  format: yaml
  label: RingCentral Events Health API
  slug: hopin-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-health-api-openapi.yml
- filename: hopin-magic-links-api-openapi.yml
  format: yaml
  label: RingCentral Events Magic Links API
  slug: hopin-magic-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-magic-links-api-openapi.yml
- filename: hopin-organizations-api-openapi.yml
  format: yaml
  label: RingCentral Events Organizations API
  slug: hopin-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-organizations-api-openapi.yml
- filename: hopin-registrations-api-openapi.yml
  format: yaml
  label: RingCentral Events Registrations API
  slug: hopin-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-registrations-api-openapi.yml
- filename: hopin-reports-api-openapi.yml
  format: yaml
  label: RingCentral Events Reports API
  slug: hopin-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-reports-api-openapi.yml
- filename: hopin-schedule-items-api-openapi.yml
  format: yaml
  label: RingCentral Events Schedule Items API
  slug: hopin-schedule-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-schedule-items-api-openapi.yml
- filename: hopin-sessions-api-openapi.yml
  format: yaml
  label: RingCentral Events Sessions API
  slug: hopin-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-sessions-api-openapi.yml
- filename: hopin-stages-api-openapi.yml
  format: yaml
  label: RingCentral Events Stages API
  slug: hopin-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-stages-api-openapi.yml
- filename: hopin-templates-api-openapi.yml
  format: yaml
  label: RingCentral Events Templates API
  slug: hopin-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-templates-api-openapi.yml
- filename: hopin-tickets-api-openapi.yml
  format: yaml
  label: RingCentral Events Tickets API
  slug: hopin-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-tickets-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hopin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RingCentral Events publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RingCentral Events API on a user''s behalf.


  Tokens are issued from https://api.events.ringcentral.com/v1/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RingCentral Events
provider_slug: hopin
schemes:
- description: OAuth 2.0 Client Credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.events.ringcentral.com/v1/auth/token
  name: oauth2
  source: openapi/openapi.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to resources
  flows:
  - clientCredentials
  scope: read
- description: Write access to resources
  flows:
  - clientCredentials
  scope: write
slug: hopin-scopes
source_filename: hopin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nschemes:\n- name: oauth2\n  source: openapi/openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.events.ringcentral.com/v1/auth/token\n  description: OAuth 2.0 Client Credentials flow\nscopes:\n- scope: read\n  description: Read access to resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openapi.json\n- scope: write\n  description: Write access to resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/scopes/hopin-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Events
- Virtual Events
- Hybrid Events
- Webinars
- Event Management
- Registration
- Sessions
- Networking
token_urls:
- https://api.events.ringcentral.com/v1/auth/token
---
