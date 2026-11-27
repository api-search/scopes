---
api_specs:
- filename: kwnva-design-catalog-api-openapi.yml
  format: yaml
  label: kwnva.design Catalog API
  slug: kwnva-design-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kwnva-design/openapi/kwnva-design-catalog-api-openapi.yml
- filename: kwnva-design-inquiries-api-openapi.yml
  format: yaml
  label: kwnva.design Inquiries API
  slug: kwnva-design-inquiries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kwnva-design/openapi/kwnva-design-inquiries-api-openapi.yml
- filename: kwnva-design-meta-api-openapi.yml
  format: yaml
  label: kwnva.design Meta API
  slug: kwnva-design-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kwnva-design/openapi/kwnva-design-meta-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: kwnva.design Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'kwnva.design publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the kwnva.design API on a user''s behalf.


  Tokens are issued from https://kwnva.design/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: kwnva.design
provider_slug: kwnva-design
schemes:
- description: Optional. Reads work anonymously. Writes may send a bearer from /oauth/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://kwnva.design/oauth/token
  name: optionalBearer
  source: openapi/kwnva-design-openapi.json
scope_count: 3
scope_names:
- catalog:read
- inquiries:write
- sandbox:write
scopes:
- description: Read the project catalog
  flows:
  - clientCredentials
  scope: catalog:read
- description: Submit project inquiries
  flows:
  - clientCredentials
  scope: inquiries:write
- description: Call sandbox writes
  flows:
  - clientCredentials
  scope: sandbox:write
slug: kwnva-design-scopes
source_filename: kwnva-design-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/kwnva-design-openapi.json\nschemes:\n- name: optionalBearer\n  source: openapi/kwnva-design-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://kwnva.design/oauth/token\n  description: Optional. Reads work anonymously. Writes may send a bearer from /oauth/token.\nscopes:\n- scope: catalog:read\n  description: Read the project catalog\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/kwnva-design-openapi.json\n- scope: inquiries:write\n  description: Submit project inquiries\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/kwnva-design-openapi.json\n- scope: sandbox:write\n  description: Call sandbox writes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/kwnva-design-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kwnva-design/scopes/kwnva-design-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Design
- Branding
- 3D Art
- UI/UX
- Studio
token_bound: false
token_urls:
- https://kwnva.design/oauth/token
---
