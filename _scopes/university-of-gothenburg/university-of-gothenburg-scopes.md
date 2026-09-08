---
api_specs:
- filename: university-of-gothenburg-korp-api-openapi.yml
  format: yaml
  label: Korp API v8 — Corpus Concordance Search
  slug: korp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-korp-api-openapi.yml
- filename: university-of-gothenburg-metadata-api-openapi.yml
  format: yaml
  label: Språkbanken Text Metadata API v3
  slug: sbx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-metadata-api-openapi.yml
- filename: university-of-gothenburg-mink-api-openapi.yml
  format: yaml
  label: Mink API v3 — Bring Your Own Corpus
  slug: mink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-mink-api-openapi.yml
- filename: university-of-gothenburg-sparv-api-openapi.yml
  format: yaml
  label: Sparv API v3 — Text Annotation Pipeline
  slug: sparv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-sparv-api-openapi.yml
- filename: university-of-gothenburg-karp-api-openapi.yml
  format: yaml
  label: Karp API v7 — Lexical Resource Editing
  slug: karp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-karp-api-openapi.yml
- filename: university-of-gothenburg-karp-search-api-openapi.yml
  format: yaml
  label: Karp Search API v1 — Karps sökgränssnitt
  slug: karp-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-karp-search-api-openapi.yml
- filename: university-of-gothenburg-gupea-oai-pmh-openapi.yml
  format: yaml
  label: GUPEA Repository OAI-PMH 2.0 Interface
  slug: gupea-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-gupea-oai-pmh-openapi.yml
authorization_urls: []
description: Scope inventory. The honest headline is that the University of Gothenburg publishes NO named OAuth scopes anywhere. Four of the six contracts declare a security scheme; none of them enumerates scopes, and the OAuth2 password-bearer flow in Mink declares an empty `scopes` object. What exists instead is a coarse two-state model — anonymous read, or an authenticated principal with full write on their own resources — expressed below as observed access tiers rather than invented scope strings. Nothing here is a scope name the University publishes; do not read these ids as such.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: University Of Gothenburg Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Gothenburg uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Gothenburg
provider_slug: university-of-gothenburg
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-gothenburg-scopes
source_filename: university-of-gothenburg-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# x-method: derived\n# x-source-url: https://ws.spraakbanken.gu.se/docs/\n# Written by API Evangelist for the api-evangelist/university-of-gothenburg repo on\n# 2026-09-01. `x-method` uses the provenance-manifest vocabulary; the artifact's own\n# `method:` key uses the enrichment-contract vocabulary. They are not in conflict.\ngenerated: '2026-09-01'\nmethod: derived\nsource: >-\n  Derived from the `components.securitySchemes` and per-operation `security` blocks of the six\n  Språkbanken Text OpenAPI documents in openapi/_original/, cross-checked against anonymous live\n  probes on 2026-09-01.\ndescription: >-\n  Scope inventory. The honest headline is that the University of Gothenburg publishes NO named\n  OAuth scopes anywhere. Four of the six contracts declare a security scheme; none of them\n  enumerates scopes, and the OAuth2 password-bearer flow in Mink declares an empty `scopes`\n  object. What exists instead is a coarse two-state model — anonymous read, or an authenticated\n\
  \  principal with full write on their own resources — expressed below as observed access tiers\n  rather than invented scope strings. Nothing here is a scope name the University publishes; do\n  not read these ids as such.\nx-no-published-scopes: true\ntiers:\n  - id: anonymous-read\n    surfaces:\n      - https://ws.spraakbanken.gu.se/ws/korp/v8\n      - https://ws.spraakbanken.gu.se/ws/metadata/v3\n      - https://ws.spraakbanken.gu.se/ws/sparv/v3\n      - https://ws.spraakbanken.gu.se/ws/mink/v3\n      - https://spraakbanken4.it.gu.se/karp/v7\n      - https://spraakbanken4.it.gu.se/karps/v1\n      - https://gupea.ub.gu.se/server/api\n      - https://gupea.ub.gu.se/server/oai/request\n    grants: >-\n      Read every public corpus, lexicon, model, analysis and repository item. Verified by\n      anonymous HTTP 200 on all eight surfaces on 2026-09-01.\n    obtained_by: nothing — no registration, no key, no header\n  - id: korp-protected-corpora\n    surfaces: [https://ws.spraakbanken.gu.se/ws/korp/v8]\n\
  \    scheme: basicAuth (HTTP Basic, declared globally in the Korp specification)\n    grants: >-\n      Query the corpora Korp reports as protected in its /info response. The corpus set is\n      licence-restricted material, not a paid tier.\n    obtained_by: >-\n      NOT PUBLISHED. The specification declares the scheme but no issuance, application or\n      contact flow for credentials is documented in it.\n  - id: mink-resource-owner\n    surfaces: [https://ws.spraakbanken.gu.se/ws/mink/v3]\n    scheme: OAuth2PasswordBearer + APIKeyHeader (declared; `scopes` object is empty)\n    grants: >-\n      Create, upload to, configure, run, list, publish and delete YOUR OWN corpora and metadata\n      resources — the 63-path write surface. Access is per-resource ownership, not per-scope.\n    obtained_by: >-\n      A Språkbanken Text account, which is a federated login through SWAMID/eduGAIN. This is the\n      one place the institution's own identity federation is a prerequisite for calling\
  \ its own API.\n  - id: karp-editor\n    surfaces: [https://spraakbanken4.it.gu.se/karp/v7]\n    scheme: HTTPBearer + APIKeyQuery\n    grants: Create, update, delete and diff entries in a lexical resource; read entry history.\n    obtained_by: >-\n      NOT PUBLISHED. Karp editing rights are granted internally to lexicographers; no public\n      application route is documented in the specification.\n  - id: sparv-job-submitter\n    surfaces: [https://ws.spraakbanken.gu.se/ws/sparv/v3]\n    scheme: ApiKeyAuth\n    grants: Upload a corpus, run the annotation pipeline, download results, force cleanup.\n    obtained_by: NOT PUBLISHED in the specification.\n  - id: dspace-write\n    surfaces: [https://gupea.ub.gu.se/server/api]\n    scheme: DSpace JWT via the `authn` link advertised in the HAL root\n    grants: Deposit and edit items in GUPEA.\n    obtained_by: A University of Gothenburg library account. Staff surface, not a public API tier.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/scopes/university-of-gothenburg-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Sweden
- Research
- Research Data
- Research Repository
- Open Data
- Library
- OAI-PMH
- Identity Federation
- Language Technology
- Natural Language Processing
- Corpus Linguistics
token_urls: []
---
