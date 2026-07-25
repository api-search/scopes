---
api_specs:
- filename: university-of-auckland-altmetric-api-openapi.yml
  format: yaml
  label: University of Auckland altmetric API
  slug: university-of-auckland-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-altmetric-api-openapi.yml
- filename: university-of-auckland-articles-api-openapi.yml
  format: yaml
  label: University of Auckland articles API
  slug: university-of-auckland-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-articles-api-openapi.yml
- filename: university-of-auckland-authors-api-openapi.yml
  format: yaml
  label: University of Auckland authors API
  slug: university-of-auckland-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-authors-api-openapi.yml
- filename: university-of-auckland-collections-api-openapi.yml
  format: yaml
  label: University of Auckland collections API
  slug: university-of-auckland-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-collections-api-openapi.yml
- filename: university-of-auckland-institutions-api-openapi.yml
  format: yaml
  label: University of Auckland institutions API
  slug: university-of-auckland-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-institutions-api-openapi.yml
- filename: university-of-auckland-oauth-api-openapi.yml
  format: yaml
  label: University of Auckland oauth API
  slug: university-of-auckland-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-oauth-api-openapi.yml
- filename: university-of-auckland-other-api-openapi.yml
  format: yaml
  label: University of Auckland other API
  slug: university-of-auckland-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-other-api-openapi.yml
- filename: university-of-auckland-profiles-api-openapi.yml
  format: yaml
  label: University of Auckland profiles API
  slug: university-of-auckland-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-profiles-api-openapi.yml
- filename: university-of-auckland-projects-api-openapi.yml
  format: yaml
  label: University of Auckland projects API
  slug: university-of-auckland-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-projects-api-openapi.yml
- filename: university-of-auckland-symplectic-api-openapi.yml
  format: yaml
  label: University of Auckland symplectic API
  slug: university-of-auckland-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: University Of Auckland Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Auckland publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Auckland API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Auckland
provider_slug: university-of-auckland
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/university-of-auckland-figshare-rest.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: university-of-auckland-scopes
source_filename: university-of-auckland-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-auckland-figshare-rest.yaml\nschemes:\n- name: OAuth2\n  source: openapi/university-of-auckland-figshare-rest.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/university-of-auckland-figshare-rest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/scopes/university-of-auckland-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- New Zealand
token_urls:
- https://api.figshare.com/v2/token
---
