---
api_specs:
- filename: university-of-tokyo-archives-portal-openapi.yml
  format: yaml
  label: UTokyo Academic Assets Archives Portal API
  slug: archives-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/openapi/university-of-tokyo-archives-portal-openapi.yml
- filename: university-of-tokyo-archives-portal-openapi.yml
  format: yaml
  label: UTokyo IIIF Presentation and Image APIs
  slug: iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/openapi/university-of-tokyo-archives-portal-openapi.yml
- filename: university-of-tokyo-oai-pmh-openapi.yml
  format: yaml
  label: UTokyo OAI-PMH Metadata Harvesting
  slug: oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/openapi/university-of-tokyo-oai-pmh-openapi.yml
- filename: university-of-tokyo-repository-records-openapi.yml
  format: yaml
  label: UTokyo Repository Records API
  slug: repository-records
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/openapi/university-of-tokyo-repository-records-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Tokyo Scopes
name_suffix: OAuth Scopes
note: There are no OAuth 2.0 scopes to record. No OAuth authorization server, token endpoint or scope vocabulary exists on any University of Tokyo host — /.well-known/oauth-authorization-server and /.well-known/openid-configuration are absent, and every public surface answers unauthenticated. This file exists to record that absence explicitly rather than leave the slot empty and let a reader infer a gap in the profile. The nearest equivalent to a scope model at this institution is SAML attribute release through GakuNin — an IdP decides which attributes (eduPersonPrincipalName, eduPersonAffiliation, eduPersonScopedAffiliation, and so on) it releases to which Service Provider. That is an authorization boundary, but it is a federation policy negotiated between entities, not a scope a developer can request. The three University of Tokyo entities and their endpoints are recorded in authentication/university-of-tokyo-authentication.yml.
overview: 'University of Tokyo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Tokyo
provider_slug: university-of-tokyo
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-tokyo-scopes
source_filename: university-of-tokyo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource:\n  - https://repository.dl.itc.u-tokyo.ac.jp/oai?verb=Identify\n  - https://repository.dl.itc.u-tokyo.ac.jp/api/records/\n  - https://da.dl.itc.u-tokyo.ac.jp/portal/help/api\n  - https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\noauth2: false\nscopes: []\nnote: >-\n  There are no OAuth 2.0 scopes to record. No OAuth authorization server, token endpoint or\n  scope vocabulary exists on any University of Tokyo host — /.well-known/oauth-authorization-server\n  and /.well-known/openid-configuration are absent, and every public surface answers\n  unauthenticated. This file exists to record that absence explicitly rather than leave the slot\n  empty and let a reader infer a gap in the profile.\n\n  The nearest equivalent to a scope model at this institution is SAML attribute release through\n  GakuNin — an IdP decides which attributes (eduPersonPrincipalName, eduPersonAffiliation,\n  eduPersonScopedAffiliation, and so on) it\
  \ releases to which Service Provider. That is an\n  authorization boundary, but it is a federation policy negotiated between entities, not a scope\n  a developer can request. The three University of Tokyo entities and their endpoints are\n  recorded in authentication/university-of-tokyo-authentication.yml.\nauthorization_model:\n  public_read:\n    surfaces:\n      - OAI-PMH (both endpoints)\n      - IIIF Presentation manifests and Image API\n      - Archives Portal item representations (_format=json|csv|bix)\n      - Repository /api/records/\n    control: >-\n      Open to anyone. The Archives Portal restricts what it exposes at the data layer instead —\n      only material for which reuse permission was obtained is served through the APIs, per the\n      university's own documentation. Per-record access is carried in the JPCOAR accessRights\n      field (\"open access\" on every sampled record).\n  federated:\n    surfaces:\n      - UTOL learning management system\n      - HPC Portal\
  \ (Wisteria / Miyabi)\n      - STEP10 course registration system\n      - Licensed library resources\n    control: SAML 2.0 attribute release via the university's GakuNin-registered Shibboleth IdPs.\n  edge_denied:\n    surfaces:\n      - https://da.dl.itc.u-tokyo.ac.jp/portal/search\n    control: >-\n      Apache-level HTTP 403 to external automated clients regardless of User-Agent. Not an\n      authorization scheme — no credential exists that would lift it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/scopes/university-of-tokyo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Japan
- Public Research University
- Research Data
- Research Repository
- Library
- Digital Archives
- Identity Federation
- IIIF
- OAI-PMH
- Open Access
- Metadata
token_urls: []
---
