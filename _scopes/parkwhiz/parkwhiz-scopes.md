---
authorization_urls:
- https://api.parkwhiz.com/v4/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Parkwhiz Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ParkWhiz publishes 4 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ParkWhiz API on a user''s behalf.


  Tokens are issued from https://api.parkwhiz.com/v4/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ParkWhiz
provider_slug: parkwhiz
schemes:
- description: 'OAuth 2.0. Partner credentials (client_id, client_secret, redirect_uri) are issued by ParkWhiz to approved partners. Scopes: public (default), partner, mobile, internal, data.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.parkwhiz.com/v4/oauth/token
  - authorizationUrl: https://api.parkwhiz.com/v4/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.parkwhiz.com/v4/oauth/token
  name: oauth2
  source: openapi/parkwhiz-openapi.yml
scope_count: 4
scope_names:
- data
- mobile
- partner
- public
scopes:
- description: Access to resources restricted by data licensing.
  flows:
  - clientCredentials
  scope: data
- description: Mobile app user access.
  flows:
  - authorizationCode
  scope: mobile
- description: Partner-level access to bookable inventory and bookings.
  flows:
  - clientCredentials
  scope: partner
- description: Default read access to public resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: public
slug: parkwhiz-scopes
source_filename: parkwhiz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parkwhiz-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/parkwhiz-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.parkwhiz.com/v4/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.parkwhiz.com/v4/oauth/authorize\n    tokenUrl: https://api.parkwhiz.com/v4/oauth/token\n  description: 'OAuth 2.0. Partner credentials (client_id, client_secret, redirect_uri) are\n    issued by ParkWhiz to approved partners. Scopes: public (default), partner, mobile, internal,\n    data.'\nscopes:\n- scope: data\n  description: Access to resources restricted by data licensing.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/parkwhiz-openapi.yml\n- scope: mobile\n  description: Mobile app user access.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/parkwhiz-openapi.yml\n- scope: partner\n  description: Partner-level access to bookable inventory and bookings.\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/parkwhiz-openapi.yml\n- scope: public\n  description: Default read access to public resources.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/parkwhiz-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parkwhiz/refs/heads/main/scopes/parkwhiz-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode
tags:
- Parking
- Mobility
- Reservations
- Bookings
- Transportation
- Location
- Events
token_urls:
- https://api.parkwhiz.com/v4/oauth/token
---
