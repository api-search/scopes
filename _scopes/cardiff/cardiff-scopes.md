---
api_specs:
- filename: cardiff-courses.yaml
  format: yaml
  label: Courses
  slug: courses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-courses.yaml
- filename: cardiff-modules.yaml
  format: yaml
  label: Modules
  slug: modules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-modules.yaml
- filename: cardiff-lookups.yaml
  format: yaml
  label: Lookups
  slug: lookups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-lookups.yaml
- filename: cardiff-publications.yaml
  format: yaml
  label: Publications
  slug: publications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-publications.yaml
- filename: cardiff-echo.yaml
  format: yaml
  label: EchoTest
  slug: echo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-echo.yaml
authorization_urls:
- https://api.data.cardiff.ac.uk/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Cardiff Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cardiff University publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cardiff University API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cardiff University
provider_slug: cardiff
schemes:
- flows:
  - authorizationUrl: https://api.data.cardiff.ac.uk/authorize
    flow: implicit
  name: default
  source: openapi/cardiff-courses.yaml
- flows:
  - authorizationUrl: https://api.data.cardiff.ac.uk/authorize
    flow: implicit
  name: default
  source: openapi/cardiff-echo.yaml
- flows:
  - authorizationUrl: https://api.data.cardiff.ac.uk/authorize
    flow: implicit
  name: default
  source: openapi/cardiff-lookups.yaml
- flows:
  - authorizationUrl: https://api.data.cardiff.ac.uk/authorize
    flow: implicit
  name: default
  source: openapi/cardiff-modules.yaml
- flows:
  - authorizationUrl: https://api.data.cardiff.ac.uk/authorize
    flow: implicit
  name: default
  source: openapi/cardiff-publications.yaml
scope_count: 2
scope_names:
- clearing
- lc_rollover
scopes:
- description: Allows users to see clearing data.
  flows:
  - implicit
  scope: clearing
- description: ''
  flows:
  - implicit
  scope: lc_rollover
slug: cardiff-scopes
source_filename: cardiff-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cardiff-courses.yaml, openapi/cardiff-echo.yaml, openapi/cardiff-lookups.yaml,\n  openapi/cardiff-modules.yaml, openapi/cardiff-publications.yaml\nschemes:\n- name: default\n  source: openapi/cardiff-courses.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.data.cardiff.ac.uk/authorize\n- name: default\n  source: openapi/cardiff-echo.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.data.cardiff.ac.uk/authorize\n- name: default\n  source: openapi/cardiff-lookups.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.data.cardiff.ac.uk/authorize\n- name: default\n  source: openapi/cardiff-modules.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.data.cardiff.ac.uk/authorize\n- name: default\n  source: openapi/cardiff-publications.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.data.cardiff.ac.uk/authorize\nscopes:\n- scope:\
  \ clearing\n  description: Allows users to see clearing data.\n  flows:\n  - implicit\n  sources:\n  - openapi/cardiff-courses.yaml\n- scope: lc_rollover\n  flows:\n  - implicit\n  sources:\n  - openapi/cardiff-modules.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/scopes/cardiff-scopes.yml
summary_line: 2 scopes · implicit
tags:
- Education
- Higher Education
- University
- United Kingdom
- Wales
- Open Data
- Courses
- Research
token_urls: []
---
