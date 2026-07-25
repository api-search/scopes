---
api_specs:
- filename: kings-college-london-altmetric-api-openapi.yml
  format: yaml
  label: King's College London altmetric API
  slug: kings-college-london-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-altmetric-api-openapi.yml
- filename: kings-college-london-articles-api-openapi.yml
  format: yaml
  label: King's College London articles API
  slug: kings-college-london-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-articles-api-openapi.yml
- filename: kings-college-london-authors-api-openapi.yml
  format: yaml
  label: King's College London authors API
  slug: kings-college-london-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-authors-api-openapi.yml
- filename: kings-college-london-collections-api-openapi.yml
  format: yaml
  label: King's College London collections API
  slug: kings-college-london-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-collections-api-openapi.yml
- filename: kings-college-london-institutions-api-openapi.yml
  format: yaml
  label: King's College London institutions API
  slug: kings-college-london-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-institutions-api-openapi.yml
- filename: kings-college-london-oauth-api-openapi.yml
  format: yaml
  label: King's College London oauth API
  slug: kings-college-london-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-oauth-api-openapi.yml
- filename: kings-college-london-other-api-openapi.yml
  format: yaml
  label: King's College London other API
  slug: kings-college-london-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-other-api-openapi.yml
- filename: kings-college-london-profiles-api-openapi.yml
  format: yaml
  label: King's College London profiles API
  slug: kings-college-london-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-profiles-api-openapi.yml
- filename: kings-college-london-projects-api-openapi.yml
  format: yaml
  label: King's College London projects API
  slug: kings-college-london-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-projects-api-openapi.yml
- filename: kings-college-london-symplectic-api-openapi.yml
  format: yaml
  label: King's College London symplectic API
  slug: kings-college-london-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/openapi/kings-college-london-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Kings College London Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'King''s College London publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the King''s College London API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: King's College London
provider_slug: kings-college-london
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/kings-college-london-figshare-repository.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: kings-college-london-scopes
source_filename: kings-college-london-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kings-college-london-figshare-repository.yaml\nschemes:\n- name: OAuth2\n  source: openapi/kings-college-london-figshare-repository.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kings-college-london-figshare-repository.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/scopes/kings-college-london-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- OAI-PMH
- Library
- United Kingdom
token_urls:
- https://api.figshare.com/v2/token
---
