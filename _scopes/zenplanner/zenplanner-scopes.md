---
api_specs:
- filename: zenplanner-classes-api-openapi.yml
  format: yaml
  label: Zen Planner Classes API
  slug: zenplanner-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-classes-api-openapi.yml
- filename: zenplanner-groups-api-openapi.yml
  format: yaml
  label: Zen Planner Groups API
  slug: zenplanner-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-groups-api-openapi.yml
- filename: zenplanner-locations-api-openapi.yml
  format: yaml
  label: Zen Planner Locations API
  slug: zenplanner-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-locations-api-openapi.yml
- filename: zenplanner-memberships-api-openapi.yml
  format: yaml
  label: Zen Planner Memberships API
  slug: zenplanner-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-memberships-api-openapi.yml
- filename: zenplanner-people-api-openapi.yml
  format: yaml
  label: Zen Planner People API
  slug: zenplanner-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-people-api-openapi.yml
- filename: zenplanner-programs-api-openapi.yml
  format: yaml
  label: Zen Planner Programs API
  slug: zenplanner-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-programs-api-openapi.yml
- filename: zenplanner-prospects-api-openapi.yml
  format: yaml
  label: Zen Planner Prospects API
  slug: zenplanner-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-prospects-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Zenplanner Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
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
  source: openapi/zenplanner-classes-api-openapi.yml
- description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens from https://operations.oauth2.partners.daxko.com/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token
  name: oauth2
  source: openapi/zenplanner-groups-api-openapi.yml
- description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens from https://operations.oauth2.partners.daxko.com/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token
  name: oauth2
  source: openapi/zenplanner-locations-api-openapi.yml
- description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens from https://operations.oauth2.partners.daxko.com/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token
  name: oauth2
  source: openapi/zenplanner-memberships-api-openapi.yml
- description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens from https://operations.oauth2.partners.daxko.com/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token
  name: oauth2
  source: openapi/zenplanner-people-api-openapi.yml
- description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens from https://operations.oauth2.partners.daxko.com/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token
  name: oauth2
  source: openapi/zenplanner-programs-api-openapi.yml
- description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens from https://operations.oauth2.partners.daxko.com/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token
  name: oauth2
  source: openapi/zenplanner-prospects-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: zenplanner-scopes
source_filename: zenplanner-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/zenplanner-classes-api-openapi.yml, openapi/zenplanner-groups-api-openapi.yml,\n  openapi/zenplanner-locations-api-openapi.yml, openapi/zenplanner-memberships-api-openapi.yml,\n  openapi/zenplanner-people-api-openapi.yml, openapi/zenplanner-programs-api-openapi.yml, openapi/zenplanner-prospects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/zenplanner-classes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\n- name: oauth2\n  source: openapi/zenplanner-groups-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n\
  \  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\n- name: oauth2\n  source: openapi/zenplanner-locations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\n- name: oauth2\n  source: openapi/zenplanner-memberships-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token\
  \ and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\n- name: oauth2\n  source: openapi/zenplanner-people-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\n- name: oauth2\n  source: openapi/zenplanner-programs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\n- name: oauth2\n  source: openapi/zenplanner-prospects-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
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
token_bound: false
token_urls:
- https://api.partners.daxko.com/v3/partners/oauth2/token
---
