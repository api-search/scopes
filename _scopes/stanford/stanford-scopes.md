---
api_specs:
- filename: stanford-sdr-api-openapi.yml
  format: yaml
  label: SDR API
  slug: sdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-sdr-api-openapi.yml
- filename: stanford-dor-services-api-openapi.yml
  format: yaml
  label: DOR Services API
  slug: dor-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-dor-services-api-openapi.yml
- filename: stanford-preservation-catalog-api-openapi.yml
  format: yaml
  label: Preservation Catalog HTTP API
  slug: preservation-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-preservation-catalog-api-openapi.yml
- filename: stanford-technical-metadata-api-openapi.yml
  format: yaml
  label: Technical Metadata API
  slug: technical-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-technical-metadata-api-openapi.yml
- filename: stanford-suri-api-openapi.yml
  format: yaml
  label: SURI API
  slug: suri-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-suri-api-openapi.yml
authorization_urls: []
description: 'Scope inventory for Stanford''s institution-operated API surfaces. The honest finding is that Stanford declares NO OAuth or fine-grained scopes anywhere in its five first-party contracts: authorization is coarse — a bearer token, a client certificate, or an issued API key grants the whole service. What Stanford does have instead is a privilege model expressed as its own Registry web service, and a Shibboleth attribute release policy at the identity layer.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Stanford Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Stanford University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stanford University
provider_slug: stanford
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: stanford-scopes
source_filename: stanford-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Stanford University — authorization scopes\ndescription: >-\n  Scope inventory for Stanford's institution-operated API surfaces. The honest finding is that\n  Stanford declares NO OAuth or fine-grained scopes anywhere in its five first-party contracts:\n  authorization is coarse — a bearer token, a client certificate, or an issued API key grants\n  the whole service. What Stanford does have instead is a privilege model expressed as its own\n  Registry web service, and a Shibboleth attribute release policy at the identity layer.\ngenerated: '2026-08-19'\nmodified: '2026-08-19'\nmethod: derived\nsource: >-\n  openapi/_original/*.yml security + components.securitySchemes (no oauth2 flows present),\n  https://uit.stanford.edu/developers/apis/privilege, https://idp.stanford.edu/metadata.xml\nx-operator: institution\noauth_scopes:\n  declared: false\n  method: derived\n  note: >-\n    No securityScheme of type oauth2 or openIdConnect appears in any of the five contracts.\n\
  \    bearerAuth is declared with `scheme: bearer` and no scope list, so `security: [{bearerAuth: []}]`\n    is authorization at service granularity.\n  checked:\n    - openapi/_original/stanford-sdr-api-openapi.yml\n    - openapi/_original/stanford-dor-services-api-openapi.yml\n    - openapi/_original/stanford-technical-metadata-api-openapi.yml\n    - openapi/_original/stanford-preservation-catalog-api-openapi.yml\n    - openapi/_original/stanford-suri-api-openapi.yml\nauthorization_model:\n  - id: mais-privilege-service\n    name: MaIS Registry Privilege API\n    method: searched\n    source: https://uit.stanford.edu/developers/apis/privilege\n    note: >-\n      Stanford externalizes authorization as its own API rather than as scopes on other APIs.\n      The Privilege web service answers \"what authority does this person hold\", and the\n      Workgroup web service answers \"who is in this group\" — the two together are Stanford's\n      campus-wide entitlement model. This is an institution-designed\
  \ pattern, not a vendor's.\n    evidence:\n      - url: https://uit.stanford.edu/developers/apis/privilege\n        status: 200\n      - url: https://uit.stanford.edu/developers/apis/workgroup\n        status: 200\n  - id: shibboleth-attribute-release\n    name: Shibboleth attribute release\n    method: probed\n    source: https://idp.stanford.edu/metadata.xml\n    note: >-\n      At the federation layer, authorization is carried by released SAML attributes scoped to\n      stanford.edu (shibmd:Scope). The metadata declares the IdP side; the attribute release\n      policy itself is not published.\n    evidence:\n      - url: https://idp.stanford.edu/metadata.xml\n        status: 200\n  - id: ai-gateway-key\n    name: AI API Gateway key\n    method: searched\n    source: https://uit.stanford.edu/service/ai-api-gateway\n    note: >-\n      Authorization is per-key and per-PTA (billing account), with usage queryable by key. No\n      scope vocabulary is published; a key is all-or-nothing\
  \ against the models in the gateway.\n    evidence:\n      - url: https://uit.stanford.edu/service/ai-api-gateway\n        status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/scopes/stanford-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Research
- United States
- California
- Private Research University
- Association of American Universities
- Research Repository
- Course Catalog
- Identity Federation
- Library
- Digital Repository
- Artificial Intelligence
- IIIF
token_urls: []
---
