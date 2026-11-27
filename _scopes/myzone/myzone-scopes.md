---
api_specs:
- filename: myzone-accounts-api-openapi.yml
  format: yaml
  label: Myzone Accounts API
  slug: myzone-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-accounts-api-openapi.yml
- filename: myzone-biometrics-api-openapi.yml
  format: yaml
  label: Myzone Biometrics API
  slug: myzone-biometrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-biometrics-api-openapi.yml
- filename: myzone-challenges-api-openapi.yml
  format: yaml
  label: Myzone Challenges API
  slug: myzone-challenges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-challenges-api-openapi.yml
- filename: myzone-classes-and-booking-api-openapi.yml
  format: yaml
  label: Myzone Classes And Booking API
  slug: myzone-classes-and-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-classes-and-booking-api-openapi.yml
- filename: myzone-facilities-api-openapi.yml
  format: yaml
  label: Myzone Facilities API
  slug: myzone-facilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-facilities-api-openapi.yml
- filename: myzone-groups-api-openapi.yml
  format: yaml
  label: Myzone Groups API
  slug: myzone-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-groups-api-openapi.yml
- filename: myzone-moves-api-openapi.yml
  format: yaml
  label: Myzone Moves API
  slug: myzone-moves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-moves-api-openapi.yml
- filename: myzone-reports-api-openapi.yml
  format: yaml
  label: Myzone Reports API
  slug: myzone-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-reports-api-openapi.yml
- filename: myzone-webhooks-api-openapi.yml
  format: yaml
  label: Myzone Webhooks API
  slug: myzone-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-webhooks-api-openapi.yml
authorization_urls:
- https://auth.myzone.org/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Myzone Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Myzone publishes 15 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Myzone API on a user''s behalf.


  Tokens are issued from https://auth.myzone.org/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Myzone
provider_slug: myzone
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.myzone.org/access_token
  - authorizationUrl: https://auth.myzone.org/authorize
    flow: authorizationCode
    tokenUrl: https://auth.myzone.org/access_token
  name: OAuth2
  source: openapi/myzone-external-api-openapi.yml
scope_count: 15
scope_names:
- delete:classes_and_bookings
- delete:groups
- read:accounts
- read:biometrics
- read:challenges
- read:classes_and_bookings
- read:facilities
- read:groups
- read:moves
- read:moves:hr
- read:reports
- write:accounts
- write:biometrics
- write:classes_and_bookings
- write:groups
scopes:
- description: client has delete access to classes and bookings api
  flows:
  - authorizationCode
  - clientCredentials
  scope: delete:classes_and_bookings
- description: client has delete access to groups api
  flows:
  - authorizationCode
  - clientCredentials
  scope: delete:groups
- description: client has read access to account api
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:accounts
- description: client has read access to biometrics api
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:biometrics
- description: client has read access to challenges api
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:challenges
- description: client has read access to classes and bookings api
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:classes_and_bookings
- description: client has read access to facilities api
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:facilities
- description: client has read access to groups api
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:groups
- description: client has read access to moves api
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:moves
- description: client has read access to heart rate data
  flows:
  - clientCredentials
  scope: read:moves:hr
- description: client has read access to reports api
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:reports
- description: client has write access to accounts api
  flows:
  - authorizationCode
  - clientCredentials
  scope: write:accounts
- description: client has write access to biometrics api
  flows:
  - authorizationCode
  - clientCredentials
  scope: write:biometrics
- description: client has write access to classes and bookings api
  flows:
  - authorizationCode
  - clientCredentials
  scope: write:classes_and_bookings
- description: client has write access to groups api
  flows:
  - authorizationCode
  - clientCredentials
  scope: write:groups
slug: myzone-scopes
source_filename: myzone-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/myzone-external-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/myzone-external-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.myzone.org/access_token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.myzone.org/authorize\n    tokenUrl: https://auth.myzone.org/access_token\nscopes:\n- scope: delete:classes_and_bookings\n  description: client has delete access to classes and bookings api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: delete:groups\n  description: client has delete access to groups api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: read:accounts\n  description: client has read access to account api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n\
  - scope: read:biometrics\n  description: client has read access to biometrics api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: read:challenges\n  description: client has read access to challenges api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: read:classes_and_bookings\n  description: client has read access to classes and bookings api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: read:facilities\n  description: client has read access to facilities api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: read:groups\n  description: client has read access to groups api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope:\
  \ read:moves\n  description: client has read access to moves api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: read:moves:hr\n  description: client has read access to heart rate data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: read:reports\n  description: client has read access to reports api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: write:accounts\n  description: client has write access to accounts api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: write:biometrics\n  description: client has write access to biometrics api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: write:classes_and_bookings\n  description: client has write\
  \ access to classes and bookings api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n- scope: write:groups\n  description: client has write access to groups api\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/myzone-external-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/myzone/scopes/myzone-scopes.yml
summary_line: 15 scopes · clientCredentials/authorizationCode
tags:
- Fitness
- MotivationTechnology
- Wearables
- Gym Management
- Software-as-a-Service
- Company
token_bound: false
token_urls:
- https://auth.myzone.org/access_token
---
