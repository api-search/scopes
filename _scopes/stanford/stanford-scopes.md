---
api_specs:
- filename: stanford-about-api-openapi.yml
  format: yaml
  label: Stanford University About API
  slug: stanford-about-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-about-api-openapi.yml
- filename: stanford-authentication-api-openapi.yml
  format: yaml
  label: Stanford University Authentication API
  slug: stanford-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-authentication-api-openapi.yml
- filename: stanford-catalog-api-openapi.yml
  format: yaml
  label: Stanford University Catalog API
  slug: stanford-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-catalog-api-openapi.yml
- filename: stanford-events-api-openapi.yml
  format: yaml
  label: Stanford University Events API
  slug: stanford-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-events-api-openapi.yml
- filename: stanford-files-api-openapi.yml
  format: yaml
  label: Stanford University Files API
  slug: stanford-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-files-api-openapi.yml
- filename: stanford-identifiers-api-openapi.yml
  format: yaml
  label: Stanford University Identifiers API
  slug: stanford-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-identifiers-api-openapi.yml
- filename: stanford-integrations-api-openapi.yml
  format: yaml
  label: Stanford University Integrations API
  slug: stanford-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-integrations-api-openapi.yml
- filename: stanford-jobs-api-openapi.yml
  format: yaml
  label: Stanford University Jobs API
  slug: stanford-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-jobs-api-openapi.yml
- filename: stanford-legacy-api-openapi.yml
  format: yaml
  label: Stanford University Legacy API
  slug: stanford-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-legacy-api-openapi.yml
- filename: stanford-metadata-api-openapi.yml
  format: yaml
  label: Stanford University Metadata API
  slug: stanford-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-metadata-api-openapi.yml
- filename: stanford-objects-api-openapi.yml
  format: yaml
  label: Stanford University Objects API
  slug: stanford-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-objects-api-openapi.yml
- filename: stanford-release-tags-api-openapi.yml
  format: yaml
  label: Stanford University Release Tags API
  slug: stanford-release-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-release-tags-api-openapi.yml
- filename: stanford-tags-api-openapi.yml
  format: yaml
  label: Stanford University Tags API
  slug: stanford-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-tags-api-openapi.yml
- filename: stanford-versions-api-openapi.yml
  format: yaml
  label: Stanford University Versions API
  slug: stanford-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-versions-api-openapi.yml
- filename: stanford-workflows-api-openapi.yml
  format: yaml
  label: Stanford University Workflows API
  slug: stanford-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-workflows-api-openapi.yml
- filename: stanford-workspaces-api-openapi.yml
  format: yaml
  label: Stanford University Workspaces API
  slug: stanford-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-workspaces-api-openapi.yml
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
