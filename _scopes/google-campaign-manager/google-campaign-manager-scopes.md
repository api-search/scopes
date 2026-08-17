---
api_specs:
- filename: google-campaign-manager-ads-api-openapi.yml
  format: yaml
  label: Google Campaign Manager Ads API
  slug: google-campaign-manager-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-ads-api-openapi.yml
- filename: google-campaign-manager-campaigns-api-openapi.yml
  format: yaml
  label: Google Campaign Manager Campaigns API
  slug: google-campaign-manager-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-campaigns-api-openapi.yml
- filename: google-campaign-manager-placements-api-openapi.yml
  format: yaml
  label: Google Campaign Manager Placements API
  slug: google-campaign-manager-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-placements-api-openapi.yml
- filename: google-campaign-manager-reports-api-openapi.yml
  format: yaml
  label: Google Campaign Manager Reports API
  slug: google-campaign-manager-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-reports-api-openapi.yml
authorization_urls: []
description: OAuth 2.0 scopes for the Campaign Manager 360 API. Baseline derived from the OpenAPI securitySchemes, then upgraded from the provider's own v5 Discovery Document (auth.oauth2.scopes, revision 20260721, HTTP 200 on 2026-08-13) — which declares a third scope the OpenAPI documents omit.
docs: https://developers.google.com/doubleclick-advertisers/authorizing
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Campaign Manager Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Campaign Manager publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Campaign Manager API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schemes: []
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/dfatrafficking
- https://www.googleapis.com/auth/dfareporting
- https://www.googleapis.com/auth/ddmconversions
scopes:
- description: View and manage your DoubleClick Campaign Manager's (DCM) display ad campaigns
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/dfatrafficking
- description: View and manage DoubleClick for Advertisers reports
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/dfareporting
- description: Manage DoubleClick Digital Marketing conversions
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/ddmconversions
slug: google-campaign-manager-scopes
source_filename: google-campaign-manager-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://dfareporting.googleapis.com/$discovery/rest?version=v5\ndocs: https://developers.google.com/doubleclick-advertisers/authorizing\nprovider: Google Campaign Manager\nproviderId: google-campaign-manager\ndescription: >-\n  OAuth 2.0 scopes for the Campaign Manager 360 API. Baseline derived from the\n  OpenAPI securitySchemes, then upgraded from the provider's own v5 Discovery\n  Document (auth.oauth2.scopes, revision 20260721, HTTP 200 on 2026-08-13) —\n  which declares a third scope the OpenAPI documents omit.\nscheme:\n  name: OAuth2\n  type: oauth2\n  flows:\n    - flow: authorizationCode\n      authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n      tokenUrl: https://oauth2.googleapis.com/token\n  service_account: supported (JWT bearer with domain-wide delegation)\n  description: >-\n    OAuth 2.0 is the only path to Campaign Manager 360 data. The Google API key\n    parameter does not authorise access\
  \ to user data on this API.\nscopes:\n  - scope: https://www.googleapis.com/auth/dfatrafficking\n    description: View and manage your DoubleClick Campaign Manager's (DCM) display ad campaigns\n    flows: [authorizationCode]\n    grants: >-\n      Read and write across the trafficking tree — accounts, advertisers,\n      campaigns, ads, creatives, placements, sites, event tags, targeting.\n    sources:\n      - https://dfareporting.googleapis.com/$discovery/rest?version=v5\n      - openapi/google-campaign-manager-ads-api-openapi.yml\n      - openapi/google-campaign-manager-campaigns-api-openapi.yml\n      - openapi/google-campaign-manager-placements-api-openapi.yml\n  - scope: https://www.googleapis.com/auth/dfareporting\n    description: View and manage DoubleClick for Advertisers reports\n    flows: [authorizationCode]\n    grants: >-\n      Report definitions, report runs, generated files, dimension values,\n      compatible fields.\n    sources:\n      - https://dfareporting.googleapis.com/$discovery/rest?version=v5\n\
  \      - openapi/google-campaign-manager-reports-api-openapi.yml\n  - scope: https://www.googleapis.com/auth/ddmconversions\n    description: Manage DoubleClick Digital Marketing conversions\n    flows: [authorizationCode]\n    grants: >-\n      Offline conversion upload and update (conversions.batchinsert,\n      conversions.batchupdate).\n    sources:\n      - https://dfareporting.googleapis.com/$discovery/rest?version=v5\n    note: >-\n      Declared by the provider's Discovery Document but absent from the OpenAPI\n      documents in this repository, which cover only the trafficking and\n      reporting subsets.\nsummary:\n  scope_count: 3\n  granularity: coarse\n  granularity_note: >-\n    Three scopes cover 67 resource collections. There is no read-only scope and\n    no per-resource scope — a token that can list campaigns can also delete\n    them. Least privilege is not expressible through this API's scope model;\n    it has to be enforced through Campaign Manager 360 user roles\
  \ instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/scopes/google-campaign-manager-scopes.yml
summary_line: 3 scopes
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
- Ad Serving
- Ad Trafficking
- Attribution
- Conversion Tracking
- Marketing
- Media Buying
- Google Marketing Platform
token_urls: []
---
