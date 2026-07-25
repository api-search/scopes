---
api_specs:
- filename: macquarie-altmetric-api-openapi.yml
  format: yaml
  label: Macquarie University altmetric API
  slug: macquarie-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-altmetric-api-openapi.yml
- filename: macquarie-articles-api-openapi.yml
  format: yaml
  label: Macquarie University articles API
  slug: macquarie-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-articles-api-openapi.yml
- filename: macquarie-authors-api-openapi.yml
  format: yaml
  label: Macquarie University authors API
  slug: macquarie-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-authors-api-openapi.yml
- filename: macquarie-collections-api-openapi.yml
  format: yaml
  label: Macquarie University collections API
  slug: macquarie-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-collections-api-openapi.yml
- filename: macquarie-institutions-api-openapi.yml
  format: yaml
  label: Macquarie University institutions API
  slug: macquarie-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-institutions-api-openapi.yml
- filename: macquarie-oauth-api-openapi.yml
  format: yaml
  label: Macquarie University oauth API
  slug: macquarie-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-oauth-api-openapi.yml
- filename: macquarie-other-api-openapi.yml
  format: yaml
  label: Macquarie University other API
  slug: macquarie-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-other-api-openapi.yml
- filename: macquarie-profiles-api-openapi.yml
  format: yaml
  label: Macquarie University profiles API
  slug: macquarie-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-profiles-api-openapi.yml
- filename: macquarie-projects-api-openapi.yml
  format: yaml
  label: Macquarie University projects API
  slug: macquarie-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-projects-api-openapi.yml
- filename: macquarie-symplectic-api-openapi.yml
  format: yaml
  label: Macquarie University symplectic API
  slug: macquarie-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Macquarie Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Macquarie University publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Macquarie University API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Macquarie University
provider_slug: macquarie
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/macquarie-rdr-figshare.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: macquarie-scopes
source_filename: macquarie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/macquarie-rdr-figshare.yaml\nschemes:\n- name: OAuth2\n  source: openapi/macquarie-rdr-figshare.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/macquarie-rdr-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/scopes/macquarie-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research Data
- Library
- Australia
token_urls:
- https://api.figshare.com/v2/token
---
