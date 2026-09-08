---
api_specs:
- filename: university-of-waterloo-academicorganizations-api-openapi.yml
  format: yaml
  label: University of Waterloo AcademicOrganizations API
  slug: university-of-waterloo-academicorganizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-academicorganizations-api-openapi.yml
- filename: university-of-waterloo-account-api-openapi.yml
  format: yaml
  label: University of Waterloo Account API
  slug: university-of-waterloo-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-account-api-openapi.yml
- filename: university-of-waterloo-classschedules-api-openapi.yml
  format: yaml
  label: University of Waterloo ClassSchedules API
  slug: university-of-waterloo-classschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-classschedules-api-openapi.yml
- filename: university-of-waterloo-courses-api-openapi.yml
  format: yaml
  label: University of Waterloo Courses API
  slug: university-of-waterloo-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-courses-api-openapi.yml
- filename: university-of-waterloo-examschedules-api-openapi.yml
  format: yaml
  label: University of Waterloo ExamSchedules API
  slug: university-of-waterloo-examschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-examschedules-api-openapi.yml
- filename: university-of-waterloo-foodservices-api-openapi.yml
  format: yaml
  label: University of Waterloo FoodServices API
  slug: university-of-waterloo-foodservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-foodservices-api-openapi.yml
- filename: university-of-waterloo-holidaydates-api-openapi.yml
  format: yaml
  label: University of Waterloo HolidayDates API
  slug: university-of-waterloo-holidaydates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-holidaydates-api-openapi.yml
- filename: university-of-waterloo-importantdates-api-openapi.yml
  format: yaml
  label: University of Waterloo ImportantDates API
  slug: university-of-waterloo-importantdates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-importantdates-api-openapi.yml
- filename: university-of-waterloo-locations-api-openapi.yml
  format: yaml
  label: University of Waterloo Locations API
  slug: university-of-waterloo-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-locations-api-openapi.yml
- filename: university-of-waterloo-subjects-api-openapi.yml
  format: yaml
  label: University of Waterloo Subjects API
  slug: university-of-waterloo-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-subjects-api-openapi.yml
- filename: university-of-waterloo-terms-api-openapi.yml
  format: yaml
  label: University of Waterloo Terms API
  slug: university-of-waterloo-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-terms-api-openapi.yml
- filename: university-of-waterloo-wcms-api-openapi.yml
  format: yaml
  label: University of Waterloo Wcms API
  slug: university-of-waterloo-wcms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-wcms-api-openapi.yml
authorization_urls: []
description: The University of Waterloo Open Data API has no authorization scopes. Its only security scheme is a single API key in the X-API-KEY header, applied globally to all 48 operations, and there is no OAuth flow, no consent surface and no per-resource authorization boundary. This file records that absence explicitly so the gap is measured rather than inferred from a missing file.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: University Of Waterloo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Waterloo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Waterloo
provider_slug: university-of-waterloo
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-waterloo-scopes
source_filename: university-of-waterloo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: University of Waterloo\nproviderId: university-of-waterloo\ngenerated: '2026-09-01'\nmethod: derived\nsource: >-\n  https://openapi.data.uwaterloo.ca/swagger/v1/swagger.json (fetched 2026-09-01) — the live\n  first-party contract — plus live probes of https://openapi.data.uwaterloo.ca/v3/.\ndescription: >-\n  The University of Waterloo Open Data API has no authorization scopes. Its only security scheme is\n  a single API key in the X-API-KEY header, applied globally to all 48 operations, and there is no\n  OAuth flow, no consent surface and no per-resource authorization boundary. This file records that\n  absence explicitly so the gap is measured rather than inferred from a missing file.\nscopes: []\nsecurity_schemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Custom API key authentication\n  scopes: []\n  applied: >-\n    Globally, via a top-level security requirement\
  \ of [{apiKey: []}]. Every operation inherits it;\n    no operation declares its own.\nauthorization_model: >-\n  Binary. A valid key grants read access to the whole published surface; an absent or unissued key\n  is rejected with 401 on every path. Waterloo's separate, gated SourceAPI applies authorization\n  out of band — access is granted per data set by the responsible data stewards through a Jira\n  service-desk request, not through scopes carried in a token.\ngaps:\n- No OAuth 2.0 or OpenID Connect flow on the public Open Data API.\n- >-\n  No scope, role or claim vocabulary is published, so a client cannot request or reason about least\n  privilege.\n- >-\n  Key issuance is self-serve (POST /v3/Account/Register) and unscoped, so every issued key carries\n  identical authority.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/scopes/university-of-waterloo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Open Data
- Canada
- Ontario
- Research
- Research Data
- Course Catalog
- Identity Federation
- Research Repository
- Campus Life
token_urls: []
---
