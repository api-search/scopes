---
api_specs:
- filename: carnegie-mellon-university-delphi-epidata-openapi.yml
  format: yaml
  label: Delphi Epidata API
  slug: delphi-epidata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-delphi-epidata-openapi.yml
- filename: carnegie-mellon-university-cert-vulnerability-notes-openapi.yml
  format: yaml
  label: CERT/CC Vulnerability Notes API
  slug: cert-vulnerability-notes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-cert-vulnerability-notes-openapi.yml
- filename: carnegie-mellon-university-library-publishing-openapi.yml
  format: yaml
  label: CMU Library Publishing Service API + OAI-PMH
  slug: library-publishing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-library-publishing-openapi.yml
authorization_urls: []
description: Carnegie Mellon University operates no OAuth 2.0 or OpenID Connect authorization server on a public, institution-owned API surface, so there are no institution-published scopes to record. Both institution-operated public APIs — Delphi Epidata and the CERT/CC Vulnerability Notes API — are anonymous and read-only, with no scoped authorization layer of any kind. This file exists to state that absence explicitly rather than leave it ambiguous; it is a REWARD-ONLY artifact and no scope has been invented to fill it.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Carnegie Mellon University Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Carnegie Mellon University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Carnegie Mellon University
provider_slug: carnegie-mellon-university
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: carnegie-mellon-university-scopes
source_filename: carnegie-mellon-university-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes 2026-08-19 of https://api.delphi.cmu.edu/epidata and https://kb.cert.org/vuls/api,\n  plus the SAML metadata at https://login.cmu.edu/idp/shibboleth.\nprovider: Carnegie Mellon University\nproviderId: carnegie-mellon-university\nsummary:\n  oauth_scopes_published_by_the_institution: 0\n  reason: no_oauth_surface_operated_by_the_institution\ndescription: >-\n  Carnegie Mellon University operates no OAuth 2.0 or OpenID Connect authorization server on a\n  public, institution-owned API surface, so there are no institution-published scopes to record.\n  Both institution-operated public APIs — Delphi Epidata and the CERT/CC Vulnerability Notes API\n  — are anonymous and read-only, with no scoped authorization layer of any kind. This file exists\n  to state that absence explicitly rather than leave it ambiguous; it is a REWARD-ONLY artifact and\n  no scope has been invented to fill it.\nscopes: []\nauthorization_model_in_use_instead:\n\
  - model: SAML 2.0 attribute release\n  operator: institution\n  surface: https://login.cmu.edu/idp/shibboleth\n  detail: >-\n    CMU's authorization boundary for federated services is SAML attribute release through Web\n    Login, governed by the InCommon Research & Scholarship entity category rather than by OAuth\n    scopes. R&S commits the IdP to releasing a defined baseline attribute bundle (eduPersonPrincipalName,\n    mail, displayName / givenName + sn, eduPersonScopedAffiliation) to R&S-tagged service\n    providers. That is the closest thing CMU publishes to a machine-readable permission\n    vocabulary, and it is a federation profile, not a scope list.\n  evidence:\n    url: https://login.cmu.edu/idp/shibboleth\n    status: 200\npreviously_recorded_and_removed:\n- source: figshare OAuth 2.0\n  operator: vendor\n  detail: >-\n    The 2026-06 profile carried a scopes file derived from the figshare v2 OpenAPI. Those scopes\n    are figshare's product, published for every figshare\
  \ customer, and were credited to CMU\n    because the spec sat in CMU's repo. Removed 2026-08-19 under the university pipeline's\n    operator rule.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/scopes/carnegie-mellon-university-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United States
- Private Research University
- Research
- Epidemiology
- Public Health
- Cybersecurity
- Vulnerability Disclosure
- Scholarly Publishing
- Institutional Repository
- Identity Federation
- Open Access
- Open Data
token_urls: []
---
