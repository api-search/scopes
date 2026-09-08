---
api_specs:
- filename: vitagroup-hip-ehrbase-openehr.json
  format: json
  label: HIP EHRbase openEHR REST API
  slug: hip-ehrbase-openehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-openehr.json
- filename: vitagroup-hip-ehrbase-admin.json
  format: json
  label: HIP EHRbase Admin API
  slug: hip-ehrbase-admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-admin.json
- filename: vitagroup-hip-ehrbase-item-tags.json
  format: json
  label: HIP EHRbase Item Tag Experimental API
  slug: hip-ehrbase-item-tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-item-tags.json
- filename: vitagroup-hip-ehrbase-enterprise.yml
  format: yaml
  label: HIP EHRbase Enterprise API
  slug: hip-ehrbase-enterprise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-enterprise.yml
- filename: vitagroup-ehrbase-sandbox-live.json
  format: json
  label: EHRbase Sandbox (live springdoc api-docs)
  slug: ehrbase-sandbox-live
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-ehrbase-sandbox-live.json
authorization_urls: []
description: ''
docs: https://docs.ehrbase.org/docs/EHRbase/Explore/Security
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Vitagroup Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py returned zero scopes because none of vitagroup's published OpenAPI documents declare an oauth2 securityScheme — the enterprise spec declares only http/bearer. OAuth 2.0 IS documented, but EHRbase does not model authorization as a scope catalogue. It reads a single role value out of the JWT's realm_access.roles or scope claim and maps it to one of two authorization levels. The role NAMES are operator-configurable, so what is recorded below is the vendor default and the claim path, not a fixed scope vocabulary.
overview: 'vitagroup uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: vitagroup
provider_slug: vitagroup
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: vitagroup-scopes
source_filename: vitagroup-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://docs.ehrbase.org/docs/EHRbase/Explore/Security\ndocs: https://docs.ehrbase.org/docs/EHRbase/Explore/Security\nnote: >-\n  derive-oauth-scopes.py returned zero scopes because none of vitagroup's published\n  OpenAPI documents declare an oauth2 securityScheme — the enterprise spec declares\n  only http/bearer. OAuth 2.0 IS documented, but EHRbase does not model authorization\n  as a scope catalogue. It reads a single role value out of the JWT's realm_access.roles\n  or scope claim and maps it to one of two authorization levels. The role NAMES are\n  operator-configurable, so what is recorded below is the vendor default and the claim\n  path, not a fixed scope vocabulary.\nmodel: role-in-claim\nscope_count: 0\nroles:\n- name: USER\n  claim_paths:\n  - realm_access.roles\n  - scope\n  configurable_via_env: SECURITY_OAUTH2USERROLE\n  configurable_via_property: security.oauth2UserRole\n  default: USER\n  grants: >-\n    The\
  \ openEHR REST API surface — EHR, EHR_STATUS, COMPOSITION, DIRECTORY,\n    CONTRIBUTION, versioned objects, template definitions and AQL query execution.\n  source: https://docs.ehrbase.org/docs/EHRbase/Explore/Security\n- name: ADMIN\n  claim_paths:\n  - realm_access.roles\n  - scope\n  configurable_via_env: SECURITY_OAUTH2ADMINROLE\n  configurable_via_property: security.oauth2AdminRole\n  default: ADMIN\n  grants: >-\n    Everything USER grants, plus the Admin API under /rest/admin/** (hard delete and\n    update of EHRs, compositions, contributions, directories, stored queries and\n    templates; Merge EHR) and, under the default ADMIN_ONLY management access policy,\n    the Spring Actuator management endpoints.\n  source: https://docs.ehrbase.org/docs/EHRbase/Explore/Admin-REST\nauthorization_server:\n  vendor_hosted: false\n  note: >-\n    The issuer is supplied by the operator via\n    SPRING_SECURITY_OAUTH2_RESOURCESERVER_JWT_ISSUERURI. In the HIP platform this is\n    Keycloak,\
  \ with one realm per tenant. vitagroup publishes no\n    /.well-known/openid-configuration of its own — probed and 404 on every vitagroup\n    and ehrbase host (see well-known/vitagroup-well-known.yml).\n  example_issuer_default: http://localhost:8081/auth/realms/ehrbase\ngaps:\n- No per-operation or per-resource scope vocabulary exists; authorization is coarse,\n  two-level (user / admin), so an agent cannot request least privilege beyond\n  \"not admin\".\n- Because role names are deployment-configurable, a client cannot learn the correct\n  role value from any vitagroup-published contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/scopes/vitagroup-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Health IT
- Electronic Health Records
- openEHR
- FHIR
- Clinical Data Repository
- Interoperability
- Germany
- Open Source
token_urls: []
---
