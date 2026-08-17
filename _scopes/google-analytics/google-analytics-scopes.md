---
api_specs:
- filename: google-analytics-accounts-api-openapi.yml
  format: yaml
  label: Google Analytics accounts API
  slug: google-analytics-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-accounts-api-openapi.yml
- filename: google-analytics-accountsummaries-api-openapi.yml
  format: yaml
  label: Google Analytics accountSummaries API
  slug: google-analytics-accountsummaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-accountsummaries-api-openapi.yml
- filename: google-analytics-data-api-openapi.yml
  format: yaml
  label: Google Analytics data API
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-data-api-openapi.yml
- filename: google-analytics-events-api-openapi.yml
  format: yaml
  label: Google Analytics Events API
  slug: google-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-events-api-openapi.yml
- filename: google-analytics-management-api-openapi.yml
  format: yaml
  label: Google Analytics management API
  slug: google-analytics-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-management-api-openapi.yml
- filename: google-analytics-metadata-api-openapi.yml
  format: yaml
  label: Google Analytics metadata API
  slug: google-analytics-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-metadata-api-openapi.yml
- filename: google-analytics-properties-api-openapi.yml
  format: yaml
  label: Google Analytics properties API
  slug: google-analytics-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-properties-api-openapi.yml
- filename: google-analytics-provisioning-api-openapi.yml
  format: yaml
  label: Google Analytics provisioning API
  slug: google-analytics-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-provisioning-api-openapi.yml
- filename: google-analytics-reports-api-openapi.yml
  format: yaml
  label: Google Analytics reports API
  slug: google-analytics-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-reports-api-openapi.yml
- filename: google-analytics-user-deletion-api-openapi.yml
  format: yaml
  label: Google Analytics User Deletion API
  slug: google-analytics-user-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-user-deletion-api-openapi.yml
- filename: google-analytics-useractivity-api-openapi.yml
  format: yaml
  label: Google Analytics userActivity API
  slug: google-analytics-useractivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-useractivity-api-openapi.yml
- filename: google-analytics-userdeletion-api-openapi.yml
  format: yaml
  label: Google Analytics userDeletion API
  slug: google-analytics-userdeletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-userdeletion-api-openapi.yml
- filename: google-analytics-validation-api-openapi.yml
  format: yaml
  label: Google Analytics Validation API
  slug: google-analytics-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-validation-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.google.com/identity/protocols/oauth2/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Analytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Analytics publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Analytics API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Analytics
provider_slug: google-analytics
schemes: []
scope_count: 7
scope_names:
- https://www.googleapis.com/auth/analytics
- https://www.googleapis.com/auth/analytics.readonly
- https://www.googleapis.com/auth/analytics.edit
- https://www.googleapis.com/auth/analytics.manage.users
- https://www.googleapis.com/auth/analytics.manage.users.readonly
- https://www.googleapis.com/auth/analytics.provision
- https://www.googleapis.com/auth/analytics.user.deletion
scopes:
- description: View and manage your Google Analytics data
  flows: []
  scope: https://www.googleapis.com/auth/analytics
- description: See and download your Google Analytics data (rendered as "View your Google Analytics data" in the v3 scope table)
  flows: []
  scope: https://www.googleapis.com/auth/analytics.readonly
- description: Edit Google Analytics management entities
  flows: []
  scope: https://www.googleapis.com/auth/analytics.edit
- description: Manage Google Analytics Account users by email address
  flows: []
  scope: https://www.googleapis.com/auth/analytics.manage.users
- description: View Google Analytics user permissions
  flows: []
  scope: https://www.googleapis.com/auth/analytics.manage.users.readonly
- description: Create a new Google Analytics account along with its default property and view
  flows: []
  scope: https://www.googleapis.com/auth/analytics.provision
- description: Manage Google Analytics user deletion requests
  flows: []
  scope: https://www.googleapis.com/auth/analytics.user.deletion
slug: google-analytics-scopes
source_filename: google-analytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developers.google.com/identity/protocols/oauth2/scopes (Google's canonical\n  OAuth 2.0 scope reference, sections \"Google Analytics API, v3\" and \"Google\n  Analytics Data API, v1beta\"; fetched 2026-08-13, HTTP 200), cross-checked against\n  the auth.oauth2.scopes blocks of discovery/google-analytics-admin-api.json,\n  discovery/google-analytics-data-api.json and\n  discovery/google-analytics-management-api-v3.json\ndocs: https://developers.google.com/identity/protocols/oauth2/scopes\nprovider: Google Analytics\nproviderId: google-analytics\nsupersedes: >-\n  The 2026-07-11 derived version of this file, which listed the OAuth flows from the\n  OpenAPI securitySchemes but carried no scope strings at all.\nauthorization_server:\n  issuer: https://accounts.google.com\n  authorization_endpoint: https://accounts.google.com/o/oauth2/v2/auth\n  token_endpoint: https://oauth2.googleapis.com/token\n  revocation_endpoint:\
  \ https://oauth2.googleapis.com/revoke\n  metadata: well-known/google-analytics-oauth-authorization-server.json\n  flows:\n    - authorization_code\n    - refresh_token\n    - device_code\n    - jwt_bearer (service accounts)\nscope_count: 7\nscopes:\n  - scope: https://www.googleapis.com/auth/analytics\n    description: View and manage your Google Analytics data\n    grants: read+write\n    apis:\n      - Google Analytics Data API (v1beta)\n      - Google Analytics Management API (v3, sunset)\n  - scope: https://www.googleapis.com/auth/analytics.readonly\n    description: >-\n      See and download your Google Analytics data (rendered as \"View your Google\n      Analytics data\" in the v3 scope table)\n    grants: read\n    apis:\n      - Google Analytics Data API (v1beta)\n      - Google Analytics Admin API (v1beta)\n      - Google Analytics Management API (v3, sunset)\n    note: >-\n      The scope Google's own MCP server requires. Sufficient for every reporting\n      call and for\
  \ reading Admin API configuration.\n  - scope: https://www.googleapis.com/auth/analytics.edit\n    description: Edit Google Analytics management entities\n    grants: write\n    apis:\n      - Google Analytics Admin API (v1beta)\n      - Google Analytics Management API (v3, sunset)\n    note: >-\n      Required for every Admin API create / patch / delete / archive method — custom\n      dimensions, custom metrics, data streams, key events, links.\n  - scope: https://www.googleapis.com/auth/analytics.manage.users\n    description: Manage Google Analytics Account users by email address\n    grants: write\n    apis:\n      - Google Analytics Management API (v3, sunset)\n      - Google Analytics Admin API access bindings (v1alpha)\n  - scope: https://www.googleapis.com/auth/analytics.manage.users.readonly\n    description: View Google Analytics user permissions\n    grants: read\n    apis:\n      - Google Analytics Management API (v3, sunset)\n      - Google Analytics Admin API access bindings\
  \ (v1alpha)\n  - scope: https://www.googleapis.com/auth/analytics.provision\n    description: Create a new Google Analytics account along with its default property and view\n    grants: write\n    apis:\n      - Google Analytics Admin API (accounts.provisionAccountTicket)\n      - Google Analytics Management API (v3, sunset)\n  - scope: https://www.googleapis.com/auth/analytics.user.deletion\n    description: Manage Google Analytics user deletion requests\n    grants: write\n    apis:\n      - Google Analytics User Deletion API (v3, sunset)\n      - Google Analytics Admin API v1alpha properties.submitUserDeletion\nby_api:\n  - api: Google Analytics Data API v1beta\n    host: https://analyticsdata.googleapis.com\n    scopes:\n      - https://www.googleapis.com/auth/analytics\n      - https://www.googleapis.com/auth/analytics.readonly\n    source: discovery/google-analytics-data-api.json\n  - api: Google Analytics Admin API v1beta\n    host: https://analyticsadmin.googleapis.com\n    scopes:\n\
  \      - https://www.googleapis.com/auth/analytics.edit\n      - https://www.googleapis.com/auth/analytics.readonly\n    source: discovery/google-analytics-admin-api.json\n  - api: Google Analytics Management API v3 (sunset 2024-07-01)\n    host: https://analytics.googleapis.com/analytics/v3\n    scopes:\n      - https://www.googleapis.com/auth/analytics\n      - https://www.googleapis.com/auth/analytics.edit\n      - https://www.googleapis.com/auth/analytics.readonly\n      - https://www.googleapis.com/auth/analytics.manage.users\n      - https://www.googleapis.com/auth/analytics.manage.users.readonly\n      - https://www.googleapis.com/auth/analytics.provision\n      - https://www.googleapis.com/auth/analytics.user.deletion\n    source: discovery/google-analytics-management-api-v3.json\n  - api: Measurement Protocol (GA4)\n    host: https://www.google-analytics.com/mp\n    scopes: []\n    note: >-\n      No OAuth. Authenticated by an api_secret query parameter minted per data stream\n\
  \      in the Google Analytics UI.\ngranularity_note: >-\n  Scopes are coarse. There is no per-property, per-resource or per-method scope: any\n  token carrying analytics.readonly can read every property the underlying identity\n  can reach, and analytics.edit can reconfigure all of them. Least-privilege for an\n  agent has to be enforced by which Google identity it impersonates, not by which\n  scope it holds.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/scopes/google-analytics-scopes.yml
summary_line: 7 scopes
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
token_urls: []
---
