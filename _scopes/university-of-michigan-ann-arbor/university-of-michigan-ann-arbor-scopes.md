---
api_specs:
- filename: university-of-michigan-ann-arbor-repository-api-openapi.yml
  format: yaml
  label: University of Michigan-Ann Arbor Repository API
  slug: university-of-michigan-ann-arbor-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-michigan-ann-arbor/refs/heads/main/openapi/university-of-michigan-ann-arbor-repository-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Michigan Ann Arbor Scopes
name_suffix: OAuth Scopes
note: 'No scope model exists to record, and that is a finding rather than a gap in the research. The one U-M contract this repo describes — the Deep Blue Documents OAI-PMH endpoint — is unauthenticated by protocol design: OAI-PMH 2.0 has no authorization layer, the endpoint answered every verb anonymously, and there is therefore nothing to scope. The enterprise estate that WOULD carry scopes, the ITS API Directory on Apigee X, is unreachable without a U-M uniqname, Duo two-factor and campus-network/VPN presence, so no scope catalog could be read. No scopes have been invented to fill the slot.'
overview: 'University of Michigan-Ann Arbor uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Michigan-Ann Arbor
provider_slug: university-of-michigan-ann-arbor
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-michigan-ann-arbor-scopes
source_filename: university-of-michigan-ann-arbor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nname: University of Michigan-Ann Arbor — Authorization Scopes\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probe of the one institution-operated contract in this repo\n  (backend.production.deepblue-documents.lib.umich.edu OAI-PMH) plus attempted probes of the\n  gated ITS API Directory, 2026-08-19.\noperator: institution\nscopes: []\nnote: >-\n  No scope model exists to record, and that is a finding rather than a gap in the research.\n  The one U-M contract this repo describes — the Deep Blue Documents OAI-PMH endpoint — is\n  unauthenticated by protocol design: OAI-PMH 2.0 has no authorization layer, the endpoint\n  answered every verb anonymously, and there is therefore nothing to scope. The enterprise\n  estate that WOULD carry scopes, the ITS API Directory on Apigee X, is unreachable without a\n  U-M uniqname, Duo two-factor and campus-network/VPN presence, so no scope catalog could be\n  read. No scopes have been invented to fill the slot.\nauthorization_boundaries_observed:\n\
  \  - boundary: OAI-PMH set restriction\n    mechanism: '?set=<setSpec>'\n    description: >-\n      The only access-partitioning mechanism on the open surface. 726 sets are advertised\n      (com_2027.42_* communities, col_2027.42_* collections). This partitions WHAT is\n      harvested, not WHO may harvest — every set is readable anonymously.\n  - boundary: ITS API Directory subscription\n    mechanism: per-API subscription behind U-M SSO\n    description: >-\n      Consumers subscribe per API in the Apigee portal and receive a key/secret pair exchanged\n      at a token endpoint. Whether Apigee product entitlements are surfaced as OAuth scopes\n      could not be determined without an account.\n    readable: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-michigan-ann-arbor/refs/heads/main/scopes/university-of-michigan-ann-arbor-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Michigan
- Big Ten
- Association of American Universities
- Research Data
- Institutional Repository
- Identity Federation
- OAI-PMH
- Library
- Research Computing
token_urls: []
---
