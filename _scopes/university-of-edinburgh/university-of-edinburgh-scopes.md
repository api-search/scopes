---
api_specs:
- filename: university-of-edinburgh-elm-api-openapi.yml
  format: yaml
  label: ELM — Edinburgh Language Models API
  slug: elm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-elm-api-openapi.yml
- filename: university-of-edinburgh-catalogue-api-openapi.yml
  format: yaml
  label: University of Edinburgh Catalogue API
  slug: university-of-edinburgh-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-catalogue-api-openapi.yml
- filename: university-of-edinburgh-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Edinburgh OAI PMH API
  slug: university-of-edinburgh-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-oai-pmh-api-openapi.yml
- filename: university-of-edinburgh-repository-api-openapi.yml
  format: yaml
  label: University of Edinburgh Repository API
  slug: university-of-edinburgh-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-repository-api-openapi.yml
authorization_urls: []
description: 'Authorization scopes across institution-operated University of Edinburgh surfaces. Recorded as an explicit negative finding: none of the publicly reachable surfaces publish a scope vocabulary, and the one surface that would have one (the Choreo API gateway at api.ed.ac.uk) exposes no discovery document to anonymous callers.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Edinburgh Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Edinburgh uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Edinburgh
provider_slug: university-of-edinburgh
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-edinburgh-scopes
source_filename: university-of-edinburgh-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: University of Edinburgh — Scopes\ndescription: >-\n  Authorization scopes across institution-operated University of Edinburgh surfaces.\n  Recorded as an explicit negative finding: none of the publicly reachable surfaces\n  publish a scope vocabulary, and the one surface that would have one (the Choreo\n  API gateway at api.ed.ac.uk) exposes no discovery document to anonymous callers.\ngenerated: '2026-08-19'\nmethod: probed\nsource: https://api.ed.ac.uk/.well-known/openid-configuration\n\nscopes: []\n\nfindings:\n- surface: Edinburgh DataShare / ERA DSpace REST\n  scopes_published: false\n  detail: >-\n    DSpace 8 authorizes by resource policy and group membership, not by OAuth scope.\n    The API exposes /authorizations and /resourcepolicies rather than a scope list.\n  evidence:\n  - url: https://datashare.ed.ac.uk/server/api\n    status: 200\n    observed: '_links include authorizations and resourcepolicies, no scope resource'\n- surface: EIDF Data Catalogue (CKAN)\n\
  \  scopes_published: false\n  detail: CKAN uses API tokens and organisation roles; no scope vocabulary is published.\n- surface: Enterprise API gateway (api.ed.ac.uk)\n  scopes_published: unknown\n  detail: >-\n    A WSO2 Choreo gateway normally publishes OAuth2 scopes per API, but no OIDC\n    discovery document or developer portal is reachable anonymously, so no scope can\n    be recorded. Marked unknown rather than false — the absence is our visibility\n    limit, not a demonstrated institutional fact.\n  evidence:\n  - url: https://api.ed.ac.uk/.well-known/openid-configuration\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/scopes/university-of-edinburgh-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Scotland
- Russell Group
- Research Repository
- Open Data
- Identity Federation
- Research Computing
- OAI-PMH
- Artificial Intelligence
token_urls: []
---
