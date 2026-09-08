---
api_specs:
- filename: king-saud-university-open-data-openapi.yml
  format: yaml
  label: KSU Open Data Distribution API
  slug: open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/openapi/king-saud-university-open-data-openapi.yml
- filename: king-saud-university-identity-openapi.yml
  format: yaml
  label: KSU Identity and Access Management (OAuth 2.0 / OpenID Connect / SAML 2.0)
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/openapi/king-saud-university-identity-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: King Saud University Scopes
name_suffix: OAuth Scopes
note: 'These are the university''s declared scopes, not a reconstruction. Three are standard OpenID Connect scopes and three are deployment-specific to KSU''s e-portal. Scope grants are not self-service: the discovery document advertises a registration_endpoint at https://iam.ksu.edu.sa/as/clients.oauth2, but that URL returned HTTP 404 to an anonymous request on 2026-09-01, so a third-party developer cannot obtain a client — and therefore cannot obtain any of these scopes — without going through the university directly.'
overview: 'King Saud University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: King Saud University
provider_slug: king-saud-university
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: king-saud-university-scopes
source_filename: king-saud-university-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: >-\n  The `scopes_supported` array of King Saud University's own OpenID Connect\n  discovery document, fetched anonymously from\n  https://iam.ksu.edu.sa/.well-known/openid-configuration on 2026-09-01 (HTTP 200,\n  application/json) and stored verbatim at\n  authentication/king-saud-university-openid-configuration.json.\nx-operator: institution\napi: king-saud-university:identity\nauthorization_server: https://iam.ksu.edu.sa\nnote: >-\n  These are the university's declared scopes, not a reconstruction. Three are\n  standard OpenID Connect scopes and three are deployment-specific to KSU's\n  e-portal. Scope grants are not self-service: the discovery document advertises a\n  registration_endpoint at https://iam.ksu.edu.sa/as/clients.oauth2, but that URL\n  returned HTTP 404 to an anonymous request on 2026-09-01, so a third-party\n  developer cannot obtain a client — and therefore cannot obtain any of these\n  scopes — without\
  \ going through the university directly.\nscopes:\n  - name: openid\n    standard: OpenID Connect Core 1.0\n    description: Requests an ID token; required for any OpenID Connect flow.\n  - name: profile\n    standard: OpenID Connect Core 1.0\n    description: >-\n      Basic profile claims. Against this deployment's claims_supported that\n      includes name, given_name, family_name, middle_name, nickname,\n      preferred_username, picture, website, gender, birthdate, zoneinfo, locale\n      and updated_at.\n  - name: email\n    standard: OpenID Connect Core 1.0\n    description: The end user's email address and its verification status.\n  - name: eportalclaims\n    standard: deployment-specific\n    description: >-\n      King Saud University e-portal claim set. Not documented publicly; the name\n      appears only in the university's discovery document.\n  - name: eportalWebScope\n    standard: deployment-specific\n    description: >-\n      King Saud University e-portal web scope,\
  \ used by the university's own\n      web-tier clients. Not documented publicly.\n  - name: NoClaim\n    standard: deployment-specific\n    description: >-\n      Issues a token carrying no claims — a PingFederate pattern for\n      authentication-only or client-credentials use where no user attributes\n      should be released.\nclaims_supported:\n  standard:\n    - sub\n    - name\n    - given_name\n    - family_name\n    - middle_name\n    - nickname\n    - preferred_username\n    - profile\n    - picture\n    - website\n    - email\n    - email_verified\n    - gender\n    - birthdate\n    - zoneinfo\n    - locale\n    - updated_at\n    - phone_number\n    - phone_number_verified\n    - address\n  deployment_specific:\n    - StudentName\n    - sAMAccountName\n    - userPrincipalName\n    - givenName\n    - sn\n    - mail\n    - mobile\n    - username\n    - sid\n    - pi.sri\n    - extensionAttribute1\n    - extensionAttribute3\n    - extensionAttribute4\n    - extensionAttribute6\n\
  \    - extensionAttribute7\n  note: >-\n    The deployment-specific list is Active Directory attribute passthrough\n    (sAMAccountName, userPrincipalName, sn, givenName, mail) plus a StudentName\n    claim, which tells you the identity provider is fronting the university's\n    directory and student records rather than a standalone user store.\nopen_data_surface:\n  api: king-saud-university:open-data\n  scopes: []\n  note: >-\n    The Open Data distribution surface at data.ksu.edu.sa requires no\n    authorization at all — no scope, key or token. It is governed by the King Saud\n    University Open Data Licence (https://data.ksu.edu.sa/ar/node/1178) rather\n    than by an authorization server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/king-saud-university/refs/heads/main/scopes/king-saud-university-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Public Research University
- Saudi Arabia
- Middle East
- Riyadh
- Open Data
- Research Data
- Identity Federation
- Single Sign-On
- Research
- Linked Data
token_urls: []
---
