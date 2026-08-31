---
api_specs:
- filename: university-of-pittsburgh-project-tycho-api-openapi.yml
  format: yaml
  label: Project Tycho API
  slug: project-tycho
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-pittsburgh/refs/heads/main/openapi/university-of-pittsburgh-project-tycho-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Pittsburgh Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Pittsburgh uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Pittsburgh
provider_slug: university-of-pittsburgh
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-pittsburgh-scopes
source_filename: university-of-pittsburgh-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# authorship: API Evangelist. Not published by the University of Pittsburgh.\nx-method: derived\nx-authorship: >-\n  Written by API Evangelist from live probes of the University of Pittsburgh's own public\n  surfaces. Pitt publishes no equivalent document. The `method:` key below is the university\n  pipeline's provenance vocabulary (how we came to hold the facts); x-method above is the\n  authorship vocabulary the provenance manifest reads (who wrote the file).\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-30 of every surface attributed to the University of Pittsburgh, plus the\n  published API reference at https://www.tycho.pitt.edu/dataset/api/.\nprovider: University of Pittsburgh\nproviderId: university-of-pittsburgh\nsummary:\n  oauth_authorization_servers_operated_by_the_institution: 0\n  scoped_surfaces: 0\n  scopes_documented: 0\nscopes: []\ndetail: >-\n  The University of Pittsburgh operates no OAuth 2.0 authorization server on a public\
  \ surface and\n  publishes no scope model. There is nothing to enumerate here, and this file exists to say so\n  rather than to be filled.\n\n  Each institution-operated surface uses an all-or-nothing credential instead of scopes. Project\n  Tycho issues one API key per registered account, carried in the query string, granting the same\n  read access to every path; the published reference names no scope, permission or role. The WPRDC\n  CKAN Action API is anonymously readable with no credential and offers no public write path. The\n  University Library System's OAI-PMH providers are anonymously harvestable, and OAI-PMH has no\n  authorization model of its own. The OJS REST API alongside them is closed entirely — HTTP 403\n  api.403.unauthorized to any unauthenticated caller — behind a per-user token issued inside each\n  journal, not a scoped grant.\n\n  Pitt Passport (https://passport.pitt.edu/idp/shibboleth) is a SAML 2.0 identity provider, and SAML\n  attribute release is the nearest\
  \ thing to a scope model the university publishes. It is not an\n  OAuth scope model and it governs attributes released to relying service providers, not access to\n  an API, so it is recorded in authentication/ rather than fabricated into a scope list here.\nprobes:\n- url: https://www.pitt.edu/.well-known/oauth-authorization-server\n  status: 404\n- url: https://developer.pitt.edu\n  status: 0\n  note: Does not resolve.\n- url: https://apis.pitt.edu\n  status: 0\n  note: Does not resolve.\n- url: https://www.tycho.pitt.edu/dataset/api/\n  status: 200\n  note: The full published API reference; contains no scope, role or permission vocabulary.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-pittsburgh/refs/heads/main/scopes/university-of-pittsburgh-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United States
- Public Research University
- Research Data
- Open Data
- Epidemiology
- Public Health
- Civic Data
- Scholarly Publishing
- Institutional Repository
- Library
- Identity Federation
- OAI-PMH
- Open Access
token_urls: []
---
