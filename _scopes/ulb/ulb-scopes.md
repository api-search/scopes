---
api_specs:
- filename: ulb-difusion-export-openapi.yml
  format: yaml
  label: DI-fusion Export API
  slug: difusion-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ulb/refs/heads/main/openapi/ulb-difusion-export-openapi.yml
- filename: ulb-difusion-oai-pmh-openapi.yml
  format: yaml
  label: DI-fusion OAI-PMH Harvesting Endpoint
  slug: difusion-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ulb/refs/heads/main/openapi/ulb-difusion-oai-pmh-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ulb Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Université libre de Bruxelles uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Université libre de Bruxelles
provider_slug: ulb
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ulb-scopes
source_filename: ulb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: ULB Authorization Scopes\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-30 of every ULB surface listed in authentication/ulb-authentication.yml,\n  plus the SAML metadata at https://auth.ulb.be/idp/metadata.\nx-operator: institution\nscopes: []\nsummary: >-\n  ULB defines no authorization scopes. Its two public machine-readable surfaces are unauthenticated\n  and therefore unscoped; its SAML identity provider expresses release policy through attribute\n  release and entity categories rather than through scopes, and the metadata carries no\n  RequestedAttribute set of its own.\nsaml_release_signals:\n  - name: REFEDS Research and Scholarship\n    value: http://refeds.org/category/research-and-scholarship\n    meaning: >-\n      ULB's IdP supports the R&S entity category, which commits it to releasing a bounded attribute\n      bundle (persistent identifier, person name, email, affiliation) to R&S-tagged service\n      providers without per-service\
  \ negotiation. This is the closest thing ULB publishes to a scope.\n    source: https://auth.ulb.be/idp/metadata\n    verified: '2026-08-30'\n  - name: shibmd:Scope\n    value: ulb.be\n    meaning: The single security domain the IdP is authoritative for; scoped attribute values are asserted only within `@ulb.be`.\n    source: https://auth.ulb.be/idp/metadata\n    verified: '2026-08-30'\n  - name: SIRTFI\n    value: https://refeds.org/sirtfi\n    meaning: >-\n      Security Incident Response Trust Framework for Federated Identity assurance certification —\n      an operational commitment, not an authorization scope, recorded here because it is the only\n      other machine-readable assurance ULB asserts.\n    source: https://auth.ulb.be/idp/metadata\n    verified: '2026-08-30'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ulb/refs/heads/main/scopes/ulb-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Belgium
- Europe
- Research
- Research Data
- Institutional Repository
- Open Access
- Identity Federation
- OAI-PMH
- Library
token_urls: []
---
