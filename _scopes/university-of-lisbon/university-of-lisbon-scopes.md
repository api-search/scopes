---
api_specs:
- filename: university-of-lisbon-fenixedu-academic-api-openapi.yml
  format: yaml
  label: FenixEdu Academic API (Instituto Superior Tecnico)
  slug: fenixedu-tecnico
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-fenixedu-academic-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Lisbon Scopes
name_suffix: OAuth Scopes
note: Written by API Evangelist. This file records an ABSENCE that was measured, not a scope list. No scope names are invented here.
overview: 'University of Lisbon uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Lisbon
provider_slug: university-of-lisbon
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-lisbon-scopes
source_filename: university-of-lisbon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nname: University of Lisbon — Access Scopes\ngenerated: '2026-09-01'\nmethod: probed\nsource:\n  - https://fenix.tecnico.ulisboa.pt/oauth/userdialog\n  - https://fenixedu.org/dev/api/\nnote: >-\n  Written by API Evangelist. This file records an ABSENCE that was measured, not a\n  scope list. No scope names are invented here.\npublished_scopes: none\nfinding: >-\n  The FenixEdu deployment at Instituto Superior Tecnico runs Bennu OAuth 2.0 with a\n  working authorization and token endpoint, but it publishes no scope vocabulary. The\n  consent dialog at /oauth/userdialog renders per registered application, the human\n  documentation at fenixedu.org/dev/api/ names no scope strings, and there is no\n  discovery document — probed 2026-09-01, no /.well-known/oauth-authorization-server\n  and no /.well-known/openid-configuration under the API host. Consequently\n  components.securitySchemes.fenixOAuth.flows.authorizationCode.scopes in\n  openapi/university-of-lisbon-fenixedu-academic-api-openapi.yml\
  \ is deliberately an\n  empty object rather than a guessed list.\naccess_boundaries_observed:\n  - boundary: anonymous\n    description: >-\n      Institutional metadata, academic terms, contacts, degree and course catalog,\n      campus spaces and blueprints, parking, canteen, shuttle, serialized domain model.\n    evidence: 9 endpoints probed 2026-09-01, all 200 with no Authorization header.\n  - boundary: person-scoped, token required\n    description: >-\n      Personal profile, course enrolments, curriculum, class and evaluation calendars,\n      evaluation enrolment, tuition and payment records.\n    evidence:\n      url: https://fenix.tecnico.ulisboa.pt/api/fenix/v1/person\n      status: 401\n      body: '{\"error\":\"accessTokenInvalidFormat\",\"error_description\":\"Access Token not recognized.\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/scopes/university-of-lisbon-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Portugal
- Europe
- Public Research University
- Course Catalog
- Research Repository
- Library
- Identity Federation
- OAI-PMH
- Open Access
- Erasmus Without Paper
- Metadata
token_urls: []
---
