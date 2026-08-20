---
api_specs:
- filename: quorum-divisionorders-api-openapi.yml
  format: yaml
  label: Quorum Software DivisionOrders API
  slug: quorum-divisionorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-divisionorders-api-openapi.yml
- filename: quorum-leases-api-openapi.yml
  format: yaml
  label: Quorum Software Leases API
  slug: quorum-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-leases-api-openapi.yml
- filename: quorum-owners-api-openapi.yml
  format: yaml
  label: Quorum Software Owners API
  slug: quorum-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-owners-api-openapi.yml
- filename: quorum-tracts-api-openapi.yml
  format: yaml
  label: Quorum Software Tracts API
  slug: quorum-tracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-tracts-api-openapi.yml
- filename: quorum-wells-api-openapi.yml
  format: yaml
  label: Quorum Software Wells API
  slug: quorum-wells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-wells-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Quorum Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Quorum Software publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Quorum Software API on a user''s behalf.


  Tokens are issued from https://auth.quorumsoftware.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Quorum Software
provider_slug: quorum
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.quorumsoftware.com/oauth2/token
  name: oauth2
  source: openapi/quorum-land-management-openapi.yml
scope_count: 2
scope_names:
- land.read
- land.write
scopes:
- description: Read land management data
  flows:
  - clientCredentials
  scope: land.read
- description: Write land management data
  flows:
  - clientCredentials
  scope: land.write
slug: quorum-scopes
source_filename: quorum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quorum-land-management-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/quorum-land-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.quorumsoftware.com/oauth2/token\nscopes:\n- scope: land.read\n  description: Read land management data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/quorum-land-management-openapi.yml\n- scope: land.write\n  description: Write land management data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/quorum-land-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/scopes/quorum-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Energy
- Oil and Gas
- Upstream
- Land Management
- Royalty Accounting
- Production Reporting
token_urls:
- https://auth.quorumsoftware.com/oauth2/token
---
