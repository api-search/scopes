---
api_specs:
- filename: mcmaster-experts-openapi.yml
  format: yaml
  label: McMaster Experts API
  slug: experts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcmaster/refs/heads/main/openapi/mcmaster-experts-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Mcmaster Scopes
name_suffix: OAuth Scopes
note: No OAuth scopes exist on any McMaster-operated surface. This file records that absence with evidence rather than leaving the artifact unwritten, and records the SAML attribute release that stands in place of scopes on the federation surface.
overview: 'McMaster University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: McMaster University
provider_slug: mcmaster
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: mcmaster-scopes
source_filename: mcmaster-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# x-method is the AUTHORSHIP vocabulary build-provenance-manifest.py reads (who wrote the\n# file: we did). `method: probed` below is the university-pipeline PROVENANCE vocabulary\n# (how we came to hold it: live probe). Two axes, two keys, neither guessed.\nx-method: generated\nversion: '0.1'\ngenerated: '2026-09-01'\nmethod: probed\nsource: https://experts.mcmaster.ca/api/search\nnote: >-\n  No OAuth scopes exist on any McMaster-operated surface. This file records that absence with\n  evidence rather than leaving the artifact unwritten, and records the SAML attribute release that\n  stands in place of scopes on the federation surface.\noauth_scopes: []\noauth_scopes_detail: >-\n  The McMaster Experts API is unauthenticated and declares no securitySchemes, so there is nothing\n  to scope. The Azure API Management portal at developer.api.mcmaster.ca issues subscription keys\n  per product after MacID sign-in, but the product list is gated and no scope or product name could\n\
  \  be read anonymously.\nfederation_attribute_release:\n  surface: https://sso.mcmaster.ca/idp/shibboleth\n  x-operator: federation\n  detail: >-\n    A Shibboleth IdP's equivalent of scopes is its attribute release policy, which is negotiated per\n    service provider and is not published in the entity metadata. The metadata does assert\n    shibmd:Scope mcmaster.ca, which bounds every scoped attribute (eduPersonPrincipalName,\n    eduPersonScopedAffiliation) the IdP may assert.\n  evidence:\n    - url: https://sso.mcmaster.ca/idp/shibboleth\n      status: 200\n      locator: Extensions/shibmd:Scope regexp=\"false\" = \"mcmaster.ca\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcmaster/refs/heads/main/scopes/mcmaster-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Canada
- Ontario
- U15 Group of Canadian Research Universities
- Research
- Research Data
- Research Repository
- Identity Federation
- Scholarly Communication
- Open Access
- Library
- Course Catalog
token_urls: []
---
