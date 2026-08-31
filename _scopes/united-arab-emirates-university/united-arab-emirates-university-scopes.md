---
authorization_urls: []
description: Scopes advertised by the UAEU enterprise identity service (eisprod.uaeu.ac.ae) in its OpenID Connect discovery document. Read verbatim from the live scopes_supported array on 2026-08-30; none of these are inferred. The registry.* scopes are WSO2 Identity Server registry scopes, not a UAEU-authored API scope vocabulary — UAEU publishes no scoped public API.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: United Arab Emirates University Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'United Arab Emirates University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: United Arab Emirates University
provider_slug: united-arab-emirates-university
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: united-arab-emirates-university-scopes
source_filename: united-arab-emirates-university-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\naid: united-arab-emirates-university\nname: United Arab Emirates University — OAuth 2.0 / OpenID Connect Scopes\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://eisprod.uaeu.ac.ae/oauth2/oidcdiscovery/.well-known/openid-configuration\nx-operator: institution\ndescription: >-\n  Scopes advertised by the UAEU enterprise identity service (eisprod.uaeu.ac.ae)\n  in its OpenID Connect discovery document. Read verbatim from the live\n  scopes_supported array on 2026-08-30; none of these are inferred. The\n  registry.* scopes are WSO2 Identity Server registry scopes, not a\n  UAEU-authored API scope vocabulary — UAEU publishes no scoped public API.\nscopes:\n  - name: openid\n    standard: openid-connect\n    description: Required to obtain an ID token from the UAEU identity service.\n  - name: profile\n    standard: openid-connect\n    description: Basic profile claims — name, family_name, given_name, preferred_username, picture, locale, updated_at.\n  - name: email\n\
  \    standard: openid-connect\n    description: email and email_verified claims.\n  - name: phone\n    standard: openid-connect\n    description: phone_number and phone_number_verified claims.\n  - name: address\n    standard: openid-connect\n    description: Structured address claim — street_address, locality, region, postal_code, country.\n  - name: registry.user\n    standard: none\n    description: WSO2 Identity Server registry scope — user-level registry access.\n  - name: registry.author\n    standard: none\n    description: WSO2 Identity Server registry scope — authoring access.\n  - name: registry.link\n    standard: none\n    description: WSO2 Identity Server registry scope — symbolic link operations.\n  - name: registry.mount\n    standard: none\n    description: WSO2 Identity Server registry scope — mount operations.\n  - name: registry.realpath\n    standard: none\n    description: WSO2 Identity Server registry scope — real path resolution.\nclaims_supported_count: 29\ncoverage_note:\
  \ >-\n  This is the complete advertised scope set. UAEU publishes no API-product scope\n  vocabulary because it publishes no API product; these scopes govern access to\n  its internal SSO, not to institutional data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-arab-emirates-university/refs/heads/main/scopes/united-arab-emirates-university-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United Arab Emirates
- Middle East
- Public Research University
- Identity Federation
- Research Repository
- Open Data
- OAI-PMH
- SCIM
- SAML
token_urls: []
---
