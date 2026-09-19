---
api_specs:
- filename: meddra-api-openapi.yml
  format: yaml
  label: MedDRA API
  slug: meddra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-api-openapi.yml
authorization_urls:
- https://mid.meddra.org/connect/authorize
description: ''
docs: https://www.meddra.org/meddra-apis
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Meddra Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares one scope, meddraapi. The provider's own OIDC discovery document advertises three API-bearing scopes on the same issuer; the other two are named there but are not referenced by the harvested MedDRA API contract, so their exact grant is not documented publicly. The full scope list below is verbatim from scopes_supported.
overview: 'Meddra publishes 3 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Meddra API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meddra
provider_slug: meddra
schemes:
- flows:
  - authorizationUrl: https://mid.meddra.org/connect/authorize
    flow: implicit
  name: oauth2
  source: openapi/meddra-api-openapi.yml
scope_count: 3
scope_names:
- meddraapi
- msmeddraapi
- meddrawapi
scopes:
- description: Meddra API - full access
  flows:
  - implicit
  scope: meddraapi
- description: ''
  flows:
  - implicit
  scope: msmeddraapi
- description: ''
  flows:
  - implicit
  scope: meddrawapi
slug: meddra-scopes
source_filename: meddra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://mid.meddra.org/.well-known/openid-configuration\ndocs: https://www.meddra.org/meddra-apis\nnote: The OpenAPI declares one scope, meddraapi. The provider's own OIDC discovery document advertises three API-bearing\n  scopes on the same issuer; the other two are named there but are not referenced by the harvested MedDRA API contract,\n  so their exact grant is not documented publicly. The full scope list below is verbatim from scopes_supported.\nschemes:\n- name: oauth2\n  source: openapi/meddra-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://mid.meddra.org/connect/authorize\nscopes:\n- scope: meddraapi\n  description: Meddra API - full access\n  flows:\n  - implicit\n  sources:\n  - openapi/meddra-api-openapi.yml\n  - https://mid.meddra.org/.well-known/openid-configuration\n  note: The scope the MedDRA API OpenAPI requires on every authenticated operation.\n- scope: msmeddraapi\n  description:\
  \ null\n  flows:\n  - implicit\n  sources:\n  - https://mid.meddra.org/.well-known/openid-configuration\n  note: Advertised by the identity provider; not referenced by the published MedDRA API contract.\n- scope: meddrawapi\n  description: null\n  flows:\n  - implicit\n  sources:\n  - https://mid.meddra.org/.well-known/openid-configuration\n  note: Advertised by the identity provider; appears to serve the Web-Based Browser (WBB). Not referenced by the published\n    MedDRA API contract.\nissuer_scopes_supported:\n- openid\n- profile\n- role\n- Permission\n- username\n- st\n- wr\n- meddra\n- meddracrid\n- meddraint\n- meddraw\n- rc\n- email\n- userid\n- meddrawint\n- meddrawcrid\n- meddraapi\n- msmeddraapi\n- meddrawapi\n- offline_access\napi_scopes_detected:\n- meddraapi\n- msmeddraapi\n- meddrawapi\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/scopes/meddra-scopes.yml
summary_line: 3 scopes · implicit
tags:
- Medical Terminology
- Pharmacovigilance
- Drug Safety
- Adverse Events
- Regulatory
- Clinical Trials
- Healthcare
- Life Sciences
- Standards
- Ontology
token_urls: []
---
