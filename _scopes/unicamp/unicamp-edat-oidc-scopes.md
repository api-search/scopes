---
api_specs:
- filename: unicamp-edat-data-api-openapi.yml
  format: yaml
  label: EDAT Data Platform API
  slug: edat-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unicamp/refs/heads/main/openapi/unicamp-edat-data-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Unicamp Edat Oidc Scopes
name_suffix: OAuth Scopes
note: scopes_supported as advertised by Unicamp's EDAT Keycloak realm on 2026-09-01. Institution specific scopes (uecEmailAccount, department_number, minio-authorization) are Unicamp's own realm configuration, not Keycloak defaults. Scope semantics are not documented publicly; the descriptions below are read from the scope names and are marked as such.
overview: 'University of Campinas uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Campinas
provider_slug: unicamp
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: unicamp-edat-oidc-scopes
source_filename: unicamp-edat-oidc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://seguranca.dados.unicamp.br/realms/edat/.well-known/openid-configuration\nnote: >-\n  scopes_supported as advertised by Unicamp's EDAT Keycloak realm on 2026-09-01. Institution\n  specific scopes (uecEmailAccount, department_number, minio-authorization) are Unicamp's own\n  realm configuration, not Keycloak defaults. Scope semantics are not documented publicly; the\n  descriptions below are read from the scope names and are marked as such.\nx-operator: institution\nscopes:\n- name: openid\n  description: Standard OIDC scope; required for an id_token.\n  method: derived\n- name: profile\n  description: Standard OIDC profile claims.\n  method: derived\n- name: phone\n  description: Standard OIDC phone claim.\n  method: derived\n- name: basic\n  description: Keycloak basic scope (sub, auth_time).\n  method: derived\n- name: acr\n  description: Authentication context class reference.\n  method: derived\n- name: groups\n  description:\
  \ Group membership claims.\n  method: derived\n- name: uecEmailAccount\n  description: Unicamp (UEC) institutional email account claim - realm-specific.\n  method: derived\n- name: department_number\n  description: Unicamp organisational unit / department number claim - realm-specific.\n  method: derived\n- name: minio-authorization\n  description: Authorization claims for the EDAT MinIO object store - realm-specific.\n  method: derived\n- name: service_account\n  description: Service-account (client_credentials) scope.\n  method: derived\n- name: Audience\n  description: Audience claim mapper - realm-specific.\n  method: derived\n- name: id\n  description: Identifier claim - realm-specific.\n  method: derived\n- name: type\n  description: Account type claim - realm-specific.\n  method: derived\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicamp/refs/heads/main/scopes/unicamp-edat-oidc-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Public Research University
- Brazil
- Latin America
- Research Data
- Open Data
- Research Repository
- Identity Federation
- OAI-PMH
- Dataverse
- Course Catalog
token_urls: []
---
