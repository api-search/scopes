---
api_specs:
- filename: university-of-texas-at-austin-tapis-systems-openapi.yml
  format: yaml
  label: Tapis v3 Research Computing Platform (TACC production tenant)
  slug: tapis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-texas-at-austin/refs/heads/main/openapi/university-of-texas-at-austin-tapis-systems-openapi.yml
authorization_urls: []
description: Scopes advertised by University of Texas at Austin authorization surfaces. Read from the live discovery document, not from documentation.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Texas At Austin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Texas at Austin uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Texas at Austin
provider_slug: university-of-texas-at-austin
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-texas-at-austin-scopes
source_filename: university-of-texas-at-austin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nname: University of Texas at Austin — authorization scopes\ndescription: >-\n  Scopes advertised by University of Texas at Austin authorization surfaces.\n  Read from the live discovery document, not from documentation.\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://enterprise.login.utexas.edu/.well-known/openid-configuration\nsurfaces:\n  - surface: UT Austin Enterprise Identity Provider (OpenID Connect)\n    x-operator: institution\n    issuer: https://enterprise.login.utexas.edu\n    generated: '2026-08-30'\n    method: probed\n    source: https://enterprise.login.utexas.edu/.well-known/openid-configuration\n    scopes:\n      - name: openid\n        standard: true\n        description: OpenID Connect base scope; requests an ID token.\n      - name: profile\n        standard: true\n        description: Standard OIDC profile claims.\n      - name: email\n        standard: true\n        description: Standard OIDC email claims.\n      - name: offline_access\n\
  \        standard: true\n        description: Refresh-token issuance.\n      - name: iidasmail\n        standard: false\n        description: >-\n          Institution-defined. Mail attribute released from the UT Austin\n          identity store. Semantics are not published publicly.\n      - name: memberof\n        standard: false\n        description: Institution-defined group membership claim.\n      - name: groups\n        standard: false\n        description: Institution-defined group claim.\n      - name: utexas_profile\n        standard: false\n        description: Institution-defined extended UT Austin profile claims.\n      - name: utexas_restrict\n        standard: false\n        description: >-\n          Institution-defined. Name implies restricted/FERPA-sensitive\n          attribute release; semantics are not published publicly.\n      - name: utexas_student_extended\n        standard: false\n        description: >-\n          Institution-defined extended student attributes.\
  \ Almost certainly\n          FERPA-governed; release is by institutional agreement, not self-service.\n  - surface: Tapis v3 platform — TACC production tenant\n    x-operator: institution\n    generated: '2026-08-30'\n    method: probed\n    source: https://tacc.tapis.io/v3/systems\n    scopes: []\n    note: >-\n      Tapis v3 does not expose an OAuth scope catalog at the tenant. Access is a\n      tenant-issued JWT plus per-resource permissions (READ / MODIFY) and a\n      sharing model, both defined in the Systems, Files and Apps contracts under\n      openapi/. No scope list is published, so none is recorded here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-texas-at-austin/refs/heads/main/scopes/university-of-texas-at-austin-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Texas
- Research Computing
- Identity Federation
- Institutional Repository
- Research Data
- Library
- Open Data
token_urls: []
---
