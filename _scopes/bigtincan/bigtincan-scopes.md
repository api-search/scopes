---
api_specs:
- filename: bigtincan-admin-api-openapi.yml
  format: yaml
  label: Bigtincan Admin API
  slug: bigtincan-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-admin-api-openapi.yml
- filename: bigtincan-bookmark-api-openapi.yml
  format: yaml
  label: Bigtincan Bookmark API
  slug: bigtincan-bookmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-bookmark-api-openapi.yml
- filename: bigtincan-channel-api-openapi.yml
  format: yaml
  label: Bigtincan Channel API
  slug: bigtincan-channel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-channel-api-openapi.yml
- filename: bigtincan-crm-api-openapi.yml
  format: yaml
  label: Bigtincan CRM API
  slug: bigtincan-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-crm-api-openapi.yml
- filename: bigtincan-event-api-openapi.yml
  format: yaml
  label: Bigtincan Event API
  slug: bigtincan-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-event-api-openapi.yml
- filename: bigtincan-file-api-openapi.yml
  format: yaml
  label: Bigtincan File API
  slug: bigtincan-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-file-api-openapi.yml
- filename: bigtincan-form-api-openapi.yml
  format: yaml
  label: Bigtincan Form API
  slug: bigtincan-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-form-api-openapi.yml
- filename: bigtincan-group-api-openapi.yml
  format: yaml
  label: Bigtincan Group API
  slug: bigtincan-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-group-api-openapi.yml
- filename: bigtincan-history-api-openapi.yml
  format: yaml
  label: Bigtincan History API
  slug: bigtincan-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-history-api-openapi.yml
- filename: bigtincan-links-api-openapi.yml
  format: yaml
  label: Bigtincan Links API
  slug: bigtincan-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-links-api-openapi.yml
- filename: bigtincan-public-file-share-api-openapi.yml
  format: yaml
  label: Bigtincan Public File Share API
  slug: bigtincan-public-file-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-public-file-share-api-openapi.yml
- filename: bigtincan-search-api-openapi.yml
  format: yaml
  label: Bigtincan Search API
  slug: bigtincan-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-search-api-openapi.yml
- filename: bigtincan-settings-api-openapi.yml
  format: yaml
  label: Bigtincan Settings API
  slug: bigtincan-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-settings-api-openapi.yml
- filename: bigtincan-story-api-openapi.yml
  format: yaml
  label: Bigtincan Story API
  slug: bigtincan-story-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-story-api-openapi.yml
- filename: bigtincan-tab-api-openapi.yml
  format: yaml
  label: Bigtincan Tab API
  slug: bigtincan-tab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-tab-api-openapi.yml
- filename: bigtincan-tag-api-openapi.yml
  format: yaml
  label: Bigtincan Tag API
  slug: bigtincan-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-tag-api-openapi.yml
- filename: bigtincan-user-api-openapi.yml
  format: yaml
  label: Bigtincan User API
  slug: bigtincan-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-user-api-openapi.yml
- filename: bigtincan-user-metadata-api-openapi.yml
  format: yaml
  label: Bigtincan User Metadata API
  slug: bigtincan-user-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/openapi/bigtincan-user-metadata-api-openapi.yml
authorization_urls:
- https://pubapi.bigtincan.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bigtincan Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bigtincan uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://pubapi.bigtincan.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bigtincan
provider_slug: bigtincan
schemes:
- description: 'Client ID + Client Secret + API Key exchanged at /services/oauth2/token with grant_type=password. Returns access_token + refresh_token. The As-User header is available only with this flow. Source: https://pubapi.bigtincan.com/doc/interactive/'
  flows:
  - flow: password
    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token
  name: oauth2_password
  source: openapi/bigtincan-hub-api-openapi.json
- description: 'Interactive Bigtincan Hub user login. The As-User header is disabled for this flow. Source: https://pubapi.bigtincan.com/doc/interactive/'
  flows:
  - authorizationUrl: https://pubapi.bigtincan.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token
  name: oauth2_authorization_code
  source: openapi/bigtincan-hub-api-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: bigtincan-scopes
source_filename: bigtincan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/bigtincan-hub-api-openapi.json\nschemes:\n- name: oauth2_password\n  source: openapi/bigtincan-hub-api-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token\n  description: 'Client ID + Client Secret + API Key exchanged at /services/oauth2/token with\n    grant_type=password. Returns access_token + refresh_token. The As-User header is available\n    only with this flow. Source: https://pubapi.bigtincan.com/doc/interactive/'\n- name: oauth2_authorization_code\n  source: openapi/bigtincan-hub-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://pubapi.bigtincan.com/services/oauth2/authorize\n    tokenUrl: https://pubapi.bigtincan.com/services/oauth2/token\n  description: 'Interactive Bigtincan Hub user login. The As-User header is disabled for this\n    flow. Source: https://pubapi.bigtincan.com/doc/interactive/'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/scopes/bigtincan-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Sales Enablement
- Content Management
- Training
- Coaching
- Buyer Engagement
- Analytics
- CRM Integration
- Digital Sales Rooms
token_urls:
- https://pubapi.bigtincan.com/services/oauth2/token
---
