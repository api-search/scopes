---
api_specs:
- filename: unico-api-integration.postman_collection.json
  format: json
  label: Unico IDCloud API
  slug: idcloud-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-api-integration.postman_collection.json
- filename: unico-web-sdk-integration.postman_collection.json
  format: json
  label: Unico IDCloud Web & SDK API
  slug: idcloud-web-sdk
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-web-sdk-integration.postman_collection.json
- filename: unico-oauth2.postman_collection.json
  format: json
  label: Unico Identity OAuth2
  slug: identity-oauth2
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/postman/unico-oauth2.postman_collection.json
authorization_urls: []
description: ''
docs: https://developer.unico.io/developers/api-reference/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Unico Scopes
name_suffix: OAuth Scopes
note: 'Unico runs OAuth2 with the RFC 7523 JWT-bearer grant, but it does NOT publish a scope catalogue. The documented assertion carries a single wildcard scope claim, and authorization is expressed through the provisioned APIKEY (which capabilities the tenant''s key enables) rather than through per-endpoint scopes. This is an honest record of that design, not a gap in our search: the Authentication page states the scope value verbatim and no permissions/scopes reference page exists anywhere in the developer.unico.io sitemap (184 URLs walked, 2026-09-02).'
overview: 'Unico uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unico
provider_slug: unico
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: unico-scopes
source_filename: unico-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://developer.unico.io/developers/api-reference/authentication\ndocs: https://developer.unico.io/developers/api-reference/authentication\nnote: >-\n  Unico runs OAuth2 with the RFC 7523 JWT-bearer grant, but it does NOT publish a scope\n  catalogue. The documented assertion carries a single wildcard scope claim, and\n  authorization is expressed through the provisioned APIKEY (which capabilities the tenant's\n  key enables) rather than through per-endpoint scopes. This is an honest record of that\n  design, not a gap in our search: the Authentication page states the scope value verbatim\n  and no permissions/scopes reference page exists anywhere in the developer.unico.io sitemap\n  (184 URLs walked, 2026-09-02).\nscheme: oauth2\ngrant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\ntoken_endpoint: https://identity.acesso.io/oauth2/token\nscope_count: 1\nscopes:\n- name: '*'\n  description: >-\n    Wildcard scope asserted\
  \ in the JWT `scope` claim. Documented verbatim as \"grants all\n    permissions\" for the authenticated service account.\n  source: https://developer.unico.io/developers/api-reference/authentication\nauthorization_model:\n  granularity: tenant + api-key\n  description: >-\n    Effective permissions are bound to the APIKEY provisioned for the project, which selects\n    the active product (Onboarding, Transactional, Cardholder Verification) and the capability\n    recipe (flow) executed. Enabling a new capability requires Unico to reissue the key —\n    the upgrade guide states this explicitly.\n  evidence: https://developer.unico.io/developers/api-reference/api/upgrade-guide\nper_endpoint_scopes_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unico/refs/heads/main/scopes/unico-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Identity Verification
- Biometrics
- Facial Recognition
- Liveness Detection
- KYC
- Fraud Prevention
- Onboarding
- Authentication
- AML
- Age Verification
- Document Verification
- Identity
- Brazil
- Latin America
token_urls: []
---
