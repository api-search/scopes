---
api_specs:
- filename: cardiff-courses-api-openapi.yml
  format: yaml
  label: Cardiff University Courses API
  slug: cardiff-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-courses-api-openapi.yml
- filename: cardiff-clearing-adjustments-api-openapi.yml
  format: yaml
  label: Cardiff University Clearing Adjustments API
  slug: cardiff-clearing-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-clearing-adjustments-api-openapi.yml
- filename: cardiff-groups-api-openapi.yml
  format: yaml
  label: Cardiff University Groups API
  slug: cardiff-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-groups-api-openapi.yml
- filename: cardiff-modules-api-openapi.yml
  format: yaml
  label: Cardiff University Modules API
  slug: cardiff-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-modules-api-openapi.yml
- filename: cardiff-assessments-api-openapi.yml
  format: yaml
  label: Cardiff University Assessments API
  slug: cardiff-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-assessments-api-openapi.yml
- filename: cardiff-occurrences-api-openapi.yml
  format: yaml
  label: Cardiff University Occurrences API
  slug: cardiff-occurrences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-occurrences-api-openapi.yml
- filename: cardiff-rollover-api-openapi.yml
  format: yaml
  label: Cardiff University Rollover API
  slug: cardiff-rollover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-rollover-api-openapi.yml
- filename: cardiff-schools-api-openapi.yml
  format: yaml
  label: Cardiff University Schools API
  slug: cardiff-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-schools-api-openapi.yml
- filename: cardiff-subjects-api-openapi.yml
  format: yaml
  label: Cardiff University Subjects API
  slug: cardiff-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-subjects-api-openapi.yml
- filename: cardiff-levels-api-openapi.yml
  format: yaml
  label: Cardiff University Levels API
  slug: cardiff-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-levels-api-openapi.yml
- filename: cardiff-semesters-api-openapi.yml
  format: yaml
  label: Cardiff University Semesters API
  slug: cardiff-semesters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-semesters-api-openapi.yml
- filename: cardiff-qualifications-api-openapi.yml
  format: yaml
  label: Cardiff University Qualifications API
  slug: cardiff-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-qualifications-api-openapi.yml
- filename: cardiff-years-api-openapi.yml
  format: yaml
  label: Cardiff University Years API
  slug: cardiff-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-years-api-openapi.yml
- filename: cardiff-publications-api-openapi.yml
  format: yaml
  label: Cardiff University Publications API
  slug: cardiff-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-publications-api-openapi.yml
- filename: cardiff-default-api-openapi.yml
  format: yaml
  label: Cardiff University Echo Default API
  slug: cardiff-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-default-api-openapi.yml
- filename: cardiff-test-api-openapi.yml
  format: yaml
  label: Cardiff University Echo Test API
  slug: cardiff-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-test-api-openapi.yml
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
- Public Research University
- United Kingdom
- Wales
- Russell Group
- Open Data
- Course Catalog
- Research Repository
- Identity Federation
- Research Computing
- Publications
token_urls: []
---
