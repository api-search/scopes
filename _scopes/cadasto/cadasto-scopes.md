---
api_specs:
- filename: cadasto-ehr-api-openapi.json
  format: json
  label: Cadasto EHR API
  slug: cadasto-ehr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-ehr-api-openapi.json
- filename: cadasto-query-api-openapi.json
  format: json
  label: Cadasto Query API (AQL)
  slug: cadasto-query-api-aql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-query-api-openapi.json
- filename: cadasto-definition-api-openapi.json
  format: json
  label: Cadasto Definition API
  slug: cadasto-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-definition-api-openapi.json
- filename: cadasto-demographic-api-openapi.json
  format: json
  label: Cadasto Demographic API
  slug: cadasto-demographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-demographic-api-openapi.json
- filename: cadasto-admin-api-openapi.json
  format: json
  label: Cadasto Admin API
  slug: cadasto-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-admin-api-openapi.json
- filename: cadasto-system-api-openapi.json
  format: json
  label: Cadasto System API
  slug: cadasto-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-system-api-openapi.json
- filename: cadasto-extra-api-openapi.json
  format: json
  label: Cadasto Additional API
  slug: cadasto-additional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-extra-api-openapi.json
- filename: cadasto-smart-on-openehr-openapi.json
  format: json
  label: Cadasto SMART on openEHR
  slug: cadasto-smart-on-openehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-smart-on-openehr-openapi.json
authorization_urls: []
description: ''
docs: https://docs.cadasto.io/docs/guides/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cadasto Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cadasto uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cadasto
provider_slug: cadasto
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cadasto-scopes
source_filename: cadasto-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://docs.cadasto.io/docs/guides/authentication (token request \"scope\" parameter and the\n  scopes_supported field of the /.well-known/smart-configuration response shown verbatim in the\n  docs) and https://docs.cadasto.io/docs/faq (\"Requested scopes: api.read api.write\" in the\n  credential-request template).\ndocs: https://docs.cadasto.io/docs/guides/authentication\nderived_baseline: >-\n  derive-oauth-scopes.py found ZERO oauth2 securitySchemes in openapi/ — the six openEHR\n  ITS-REST documents Cadasto publishes carry an empty components.securitySchemes, and the\n  Additional API declares only http/bearer. Every scope below therefore comes from the prose\n  documentation, not from a machine-readable contract.\nflow: clientCredentials\ntoken_endpoint: https://{mycompany}.auth.prod.cadasto.io/oauth/token\nscope_delimiter: ' '\nscopes:\n- name: api.read\n  description: >-\n    Read access to the Cadasto API surface.\
  \ Documented as one of the two scopes advertised by\n    scopes_supported and requested at credential issuance.\n- name: api.write\n  description: >-\n    Write access to the Cadasto API surface. Documented as one of the two scopes advertised by\n    scopes_supported and requested at credential issuance.\ngranularity: coarse\nnotes:\n  - >-\n    Only two scopes are published, and they are platform-wide read/write. There is no per-API\n    (EHR vs Demographic vs Admin), per-resource or per-operation scope in the public\n    documentation, so an agent granted api.write on a Cadasto tenant can also reach the Admin\n    API's physically destructive operations unless the tenant restricts them by some other\n    means the docs do not describe.\n  - >-\n    The docs say the live /.well-known/smart-configuration response \"may include additional\n    fields\"; a tenant's actual scopes_supported may be richer than the two documented here.\n    Confirming that requires an issued tenant, so it is\
  \ recorded as unknown rather than guessed.\n  - >-\n    SMART on openEHR is declared fully supported, but no SMART scope grammar\n    (patient/*.read, user/*.write, launch/patient) is published on a public Cadasto page.\ngaps:\n  - No scopes reference page exists; the two scope names appear only as examples inside the\n    authentication guide and the FAQ credential-request template.\n  - No scope-to-operation mapping is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/scopes/cadasto-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare
- Health IT
- openEHR
- Electronic Health Records
- Clinical Data Repository
- Interoperability
- FHIR
- Vendor Neutral Archive
- Clinical Data
- AQL
- MCP
- Agent Skills
- Netherlands
token_urls: []
---
