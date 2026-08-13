---
api_specs:
- filename: egym-mms-api-v2-openapi.yml
  format: yaml
  label: EGYM MMS API V2
  slug: mms-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-mms-api-v2-openapi.yml
- filename: egym-mms-api-v1-openapi.yml
  format: yaml
  label: EGYM MMS API v1
  slug: mms-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-mms-api-v1-openapi.yml
- filename: egym-data-hub-openapi.yml
  format: yaml
  label: EGYM Data Hub API
  slug: data-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-data-hub-openapi.yml
- filename: egym-data-export-openapi.yml
  format: yaml
  label: EGYM Data Export API
  slug: data-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-data-export-openapi.yml
- filename: egym-equipment-vendor-standalone-openapi.yml
  format: yaml
  label: EGYM Equipment Vendor API (standalone clients)
  slug: equipment-vendor-standalone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-equipment-vendor-standalone-openapi.yml
- filename: egym-equipment-vendor-server-openapi.yml
  format: yaml
  label: EGYM Equipment Vendor API (server-to-server)
  slug: equipment-vendor-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-equipment-vendor-server-openapi.yml
- filename: egym-user-connect-openapi.yml
  format: yaml
  label: EGYM User Connect API
  slug: user-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-user-connect-openapi.yml
- filename: egym-canonical-groupx-classes-openapi.yml
  format: yaml
  label: EGYM Canonical GroupX Classes API (blueprint)
  slug: canonical-groupx-classes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-canonical-groupx-classes-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Egym Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EGYM uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EGYM
provider_slug: egym
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /api/v1/oauth/token
  name: partner
  source: openapi/egym-equipment-vendor-standalone-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: egym-scopes
source_filename: egym-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/egym-equipment-vendor-standalone-openapi.yml\nschemes:\n- name: partner\n  source: openapi/egym-equipment-vendor-standalone-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/v1/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/scopes/egym-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Fitness
- Health
- Wellness
- Corporate Wellness
- Connected Equipment
- Gym Management
- Member Management
- Check-In
- Measurements
- Workouts
- Analytics
- Webhooks
- Germany
token_urls:
- /api/v1/oauth/token
---
