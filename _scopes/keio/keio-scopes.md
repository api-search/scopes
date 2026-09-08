---
api_specs:
- filename: keio-koara-oai-pmh-openapi.yml
  format: yaml
  label: KOARA OAI-PMH Metadata API
  slug: koara-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/openapi/keio-koara-oai-pmh-openapi.yml
- filename: keio-iiif-openapi.yml
  format: yaml
  label: Keio Media Center Digital Collections IIIF API
  slug: iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/openapi/keio-iiif-openapi.yml
authorization_urls: []
description: 'Keio University defines no authorization scopes on any surface it operates itself. This file records that as a measured absence rather than leaving the artifact out, because the reason matters: the two institution-operated APIs — KOARA''s OAI-PMH interface and the Media Center''s IIIF endpoints — are fully anonymous, and an anonymous API has no scope model by construction, not by omission. There is nothing to divide because there is nothing to grant.


  The only scope vocabulary reachable anywhere in the estate belongs to Keio''s Okta tenant, and it is Okta''s standard OpenID Connect scope set rather than anything Keio authored. It is recorded below with its operator marked, so that it is never read as institutional engineering.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Keio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Keio University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Keio University
provider_slug: keio
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: keio-scopes
source_filename: keio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nauthorship: API Evangelist\nprobe_basis: live probe sweep of Keio University surfaces, 2026-09-01\nsource: >-\n  Live probes on 2026-09-01 of every Keio surface recorded in apis.yml, plus the OpenID Connect\n  discovery document at https://keio.okta.com/.well-known/openid-configuration (HTTP 200).\nprovider: Keio University\nproviderId: keio\ndescription: >-\n  Keio University defines no authorization scopes on any surface it operates itself. This file\n  records that as a measured absence rather than leaving the artifact out, because the reason\n  matters: the two institution-operated APIs — KOARA's OAI-PMH interface and the Media Center's\n  IIIF endpoints — are fully anonymous, and an anonymous API has no scope model by construction,\n  not by omission. There is nothing to divide because there is nothing to grant.\n\n\n  The only scope vocabulary reachable anywhere in the estate belongs to Keio's Okta tenant, and it\n  is Okta's\
  \ standard OpenID Connect scope set rather than anything Keio authored. It is recorded\n  below with its operator marked, so that it is never read as institutional engineering.\n\ninstitution_operated:\n  scopes: []\n  detail: >-\n    No scopes. KOARA OAI-PMH and the IIIF Presentation and Image APIs accept unauthenticated\n    requests and return complete responses; there is no Authorization header, no token, no consent\n    screen and therefore no scope.\n\ntenant_operated:\n  - surface: Keio Okta tenant\n    issuer: https://keio.okta.com\n    x-operator: tenant\n    x-operator-evidence: >-\n      keio.okta.com is Keio's tenant on the Okta identity platform. The scopes advertised are\n      Okta's platform vocabulary, identical for every Okta org, and are not authored by Keio.\n    source: examples/keio-okta-openid-configuration.json\n    scopes_advertised_note: >-\n      The discovery document advertises the standard OpenID Connect scope set (openid, profile,\n      email, address, phone,\
  \ offline_access) together with Okta's org-level scopes. Because these\n      are the platform's and not the institution's, they are described rather than enumerated as\n      Keio's own — enumerating a vendor's scope list under an institution's slug is the same\n      attribution error this pipeline exists to prevent.\n    obtainable_by_public: false\n    obtainable_detail: >-\n      A client_id is created only by Keio IT staff. The discovery document is readable; the\n      authorization it describes is not reachable by an unaffiliated caller.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/scopes/keio-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Japan
- Research
- Institutional Repository
- Research Repository
- Identity Federation
- Digital Collections
- IIIF
- OAI-PMH
- Open Access
- Cultural Heritage
token_urls: []
---
