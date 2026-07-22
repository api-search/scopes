---
api_specs:
- filename: skyhigh-incidents-openapi-original.yml
  format: yaml
  label: Skyhigh Security SSE Incidents API
  slug: skyhigh-security-sse-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyhigh/refs/heads/main/openapi/skyhigh-incidents-openapi-original.yml
authorization_urls:
- http://com.shn/api/oauth/dialog
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Skyhigh Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Skyhigh Security publishes 3 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Skyhigh Security API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Skyhigh Security
provider_slug: skyhigh
schemes:
- flows:
  - authorizationUrl: http://com.shn/api/oauth/dialog
    flow: implicit
  name: tenantAuth
  source: openapi/skyhigh-incidents-openapi-original.yml
scope_count: 3
scope_names:
- read:data
- read:users
- write:users
scopes:
- description: Grants read access to all URL data used by authorized tenant.
  flows:
  - implicit
  scope: read:data
- description: Grants read access to all users within authorized tenant.
  flows:
  - implicit
  scope: read:users
- description: Grants read/write access to all users within authorized tenant.
  flows:
  - implicit
  scope: write:users
slug: skyhigh-scopes
source_filename: skyhigh-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/skyhigh-incidents-openapi-original.yml\nschemes:\n- name: tenantAuth\n  source: openapi/skyhigh-incidents-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: http://com.shn/api/oauth/dialog\nscopes:\n- scope: read:data\n  description: Grants read access to all URL data used by authorized tenant.\n  flows:\n  - implicit\n  sources:\n  - openapi/skyhigh-incidents-openapi-original.yml\n- scope: read:users\n  description: Grants read access to all users within authorized tenant.\n  flows:\n  - implicit\n  sources:\n  - openapi/skyhigh-incidents-openapi-original.yml\n- scope: write:users\n  description: Grants read/write access to all users within authorized tenant.\n  flows:\n  - implicit\n  sources:\n  - openapi/skyhigh-incidents-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyhigh/refs/heads/main/scopes/skyhigh-scopes.yml
summary_line: 3 scopes · implicit
tags:
- Company
- Cybersecurity
- Security Service Edge
- CASB
- Secure Web Gateway
- Data Loss Prevention
- Cloud Security
- Zero Trust
- SASE
token_urls: []
---
