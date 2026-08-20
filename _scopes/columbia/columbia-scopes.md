---
api_specs:
- filename: columbia-library-hours-openapi.yml
  format: yaml
  label: Columbia University Libraries Hours API
  slug: library-hours
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/columbia/refs/heads/main/openapi/columbia-library-hours-openapi.yml
authorization_urls: []
description: 'Columbia University publishes no authorization scopes. This file records that as a measured absence rather than leaving the artifact off, because the reason for the absence is itself the finding: Columbia operates no OAuth 2.0 authorization server, no OpenID Connect provider and no API key programme, so there is no place a scope could be declared.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Columbia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Columbia University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Columbia University
provider_slug: columbia
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: columbia-scopes
source_filename: columbia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes of every Columbia University surface reachable without a credential on 2026-08-19,\n  plus Columbia's published Shibboleth IdP metadata.\nprovider: Columbia University\nproviderId: columbia\ndescription: >-\n  Columbia University publishes no authorization scopes. This file records that as a measured\n  absence rather than leaving the artifact off, because the reason for the absence is itself the\n  finding: Columbia operates no OAuth 2.0 authorization server, no OpenID Connect provider and no\n  API key programme, so there is no place a scope could be declared.\nscopes: []\nx-operator: institution\nfindings:\n- surface: Columbia University Libraries Hours API\n  baseURL: https://hours.library.columbia.edu/api/v1\n  x-operator: institution\n  scopes_declared: 0\n  assessment: >-\n    Read-only and fully anonymous. Both operations explicitly skip authentication and\n    authorization in Columbia's own source;\
  \ there is nothing to scope. An absent scope model is\n    the correct design here, not a gap.\n- surface: Columbia Shibboleth Identity Provider\n  baseURL: https://shibboleth.columbia.edu/idp\n  x-operator: institution\n  scopes_declared: 0\n  assessment: >-\n    SAML 2.0, which uses attribute release policy rather than OAuth scopes. The published metadata\n    declares a shibmd:Scope of columbia.edu — that is the SAML security-domain scope, an entirely\n    different concept from an authorization scope, and it is deliberately not counted here. No\n    attribute release policy or entity category (REFEDS R&S, CoCo) is declared in the published\n    metadata.\n- surface: Columbia Open Data Service\n  baseURL: https://opendataservice.columbia.edu/\n  x-operator: institution\n  scopes_declared: 0\n  assessment: >-\n    Access is binary: a Columbia UNI grants it, anything else does not. There are no tiers,\n    no per-feed permissions published, and no scope vocabulary.\n- surface: CourseWorks\
  \ (Instructure Canvas)\n  baseURL: https://courseworks2.columbia.edu/api/v1\n  x-operator: tenant\n  scopes_declared: 0\n  assessment: >-\n    Canvas does implement a developer-key scope model, but it is Instructure's vocabulary and is\n    not published by Columbia. Deliberately not credited to the institution.\nsummary:\n  total_scopes: 0\n  oauth_authorization_server: false\n  openid_connect: false\n  api_key_programme: false\nnotes: >-\n  Zero is the true number. This file exists so that the zero is legible and sourced, rather than\n  being read as an artifact that was never generated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/columbia/refs/heads/main/scopes/columbia-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Ivy League
- Private Research University
- United States
- New York
- Identity Federation
- Library
- Open Data
- Research Repository
- Research Data
- Course Catalog
- Campus Life
token_urls: []
---
