---
api_specs:
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner People API
  slug: zenplanner-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Memberships API
  slug: zenplanner-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Classes API
  slug: zenplanner-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Locations API
  slug: zenplanner-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Programs API
  slug: zenplanner-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Prospects API
  slug: zenplanner-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Groups API
  slug: zenplanner-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.partners.daxko.com/tutorials/authentication/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Zenplanner Scopes
name_suffix: OAuth Scopes
note: The Daxko Partners platform (which hosts the Zen Planner API) does not publish named OAuth permission scopes - its client_credentials token flow uses the scope field as a customer/client identifier rather than a permissions scope, per https://docs.partners.daxko.com/tutorials/authentication/.
overview: 'Zen Planner uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.partners.daxko.com/v3/partners/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zen Planner
provider_slug: zenplanner
schemes:
- description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens from https://operations.oauth2.partners.daxko.com/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token
  name: oauth2
  source: openapi/zenplanner-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: zenplanner-scopes
source_filename: zenplanner-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenplanner-openapi.yml\ndocs: https://docs.partners.daxko.com/tutorials/authentication/\nnote: The Daxko Partners platform (which hosts the Zen Planner API) does not publish\n  named OAuth permission scopes - its client_credentials token flow uses the scope\n  field as a customer/client identifier rather than a permissions scope, per\n  https://docs.partners.daxko.com/tutorials/authentication/.\nschemes:\n- name: oauth2\n  source: openapi/zenplanner-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/scopes/zenplanner-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fitness
- Gym Management
- Studio Management
- Martial Arts
- Membership
- Scheduling
- Class Booking
- Daxko
token_urls:
- https://api.partners.daxko.com/v3/partners/oauth2/token
---
