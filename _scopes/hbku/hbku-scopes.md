---
api_specs:
- filename: hbku-altmetric-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University altmetric API
  slug: hbku-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-altmetric-api-openapi.yml
- filename: hbku-articles-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University articles API
  slug: hbku-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-articles-api-openapi.yml
- filename: hbku-authors-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University authors API
  slug: hbku-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-authors-api-openapi.yml
- filename: hbku-collections-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University collections API
  slug: hbku-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-collections-api-openapi.yml
- filename: hbku-institutions-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University institutions API
  slug: hbku-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-institutions-api-openapi.yml
- filename: hbku-oauth-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University oauth API
  slug: hbku-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-oauth-api-openapi.yml
- filename: hbku-other-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University other API
  slug: hbku-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-other-api-openapi.yml
- filename: hbku-profiles-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University profiles API
  slug: hbku-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-profiles-api-openapi.yml
- filename: hbku-projects-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University projects API
  slug: hbku-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-projects-api-openapi.yml
- filename: hbku-symplectic-api-openapi.yml
  format: yaml
  label: Hamad Bin Khalifa University symplectic API
  slug: hbku-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hbku Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hamad Bin Khalifa University publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hamad Bin Khalifa University API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hamad Bin Khalifa University
provider_slug: hbku
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/hbku-figshare-api.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: hbku-scopes
source_filename: hbku-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hbku-figshare-api.yaml\nschemes:\n- name: OAuth2\n  source: openapi/hbku-figshare-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hbku-figshare-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/scopes/hbku-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Qatar
- Middle East
token_urls:
- https://api.figshare.com/v2/token
---
