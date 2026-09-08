---
api_specs:
- filename: hebrew-university-of-jerusalem-shnaton-course-catalog-openapi.yml
  format: yaml
  label: Shnaton Course Catalog API
  slug: shnaton-course-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hebrew-university-of-jerusalem/refs/heads/main/openapi/hebrew-university-of-jerusalem-shnaton-course-catalog-openapi.yml
authorization_urls: []
description: 'Authorization scopes across the Hebrew University of Jerusalem''s programmable surfaces. There are none to record for the institution-operated API, and saying so is the finding rather than a gap: the Shnaton course catalog API is entirely unauthenticated, so it has no authorization model, no consent surface and no scope vocabulary. This file exists to state that positively so the absence is not later mistaken for something unmeasured.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hebrew University Of Jerusalem Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hebrew University of Jerusalem uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hebrew University of Jerusalem
provider_slug: hebrew-university-of-jerusalem
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hebrew-university-of-jerusalem-scopes
source_filename: hebrew-university-of-jerusalem-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# x-method: derived\n# x-source-url: https://shnaton.huji.ac.il/api\n# Authored by API Evangelist from live probes of the Hebrew University of Jerusalem's own\n# hosts. NOT published by the institution. See `method:` below for how it was obtained.\nspecification: API Evangelist Scopes\nspecificationVersion: '0.1'\nprovider: Hebrew University of Jerusalem\nproviderId: hebrew-university-of-jerusalem\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probing of https://shnaton.huji.ac.il/api on 2026-09-01, and inspection of the\n  SAML 2.0 metadata at https://idp.cc.huji.ac.il/simplesaml/saml2/idp/metadata.php.\ndescription: >-\n  Authorization scopes across the Hebrew University of Jerusalem's programmable surfaces.\n  There are none to record for the institution-operated API, and saying so is the finding\n  rather than a gap: the Shnaton course catalog API is entirely unauthenticated, so it has\n  no authorization model, no consent surface and no scope vocabulary.\
  \ This file exists to\n  state that positively so the absence is not later mistaken for something unmeasured.\n\nscopes: []\n\nx-scope-model:\n  - surface: Shnaton Course Catalog API\n    baseURL: https://shnaton.huji.ac.il/api\n    x-operator: institution\n    model: none\n    detail: >-\n      No authentication means no authorization. Every operation is public and read-only;\n      no write operation of any kind was found in the catalog's own JavaScript client, which\n      issues only GET and a POST used as a search verb. The effective scope of an anonymous\n      caller is the entire published course catalog for every academic year the university\n      lists, currently 2020 through 2027.\n    effective_grant: read:everything-published\n    write_operations: none\n\n  - surface: Hebrew University SAML Identity Provider\n    entityID: https://idp.cc.huji.ac.il/simplesaml/saml2/idp/metadata.php\n    x-operator: institution\n    model: saml-attribute-release\n    detail: >-\n      Authorization\
  \ on the institution's authenticated estate is expressed as SAML attribute\n      release from the university's IdP to each service provider, not as OAuth scopes. The\n      metadata published at the entityID is an IDPSSODescriptor; it declares the SSO bindings\n      and signing key but does not itself publish a per-service attribute-release policy, so\n      no scope vocabulary can be read from it without access the university does not grant\n      publicly.\n\n  - surface: Elsevier Pure CRIS web services\n    baseURL: https://cris.huji.ac.il/ws/api\n    x-operator: tenant\n    model: vendor-api-key\n    detail: >-\n      Pure's API authorization model is Elsevier's, not the university's, and its scope\n      vocabulary belongs in Elsevier's own profile. Recorded here only to mark why no scopes\n      are claimed for the Hebrew University from this surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hebrew-university-of-jerusalem/refs/heads/main/scopes/hebrew-university-of-jerusalem-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Research
- Israel
- Jerusalem
- Course Catalog
- Identity Federation
- Research Repository
- Library
- SAML
- OAI-PMH
- Open Access
- Public Research University
token_urls: []
---
