---
authorization_urls: []
description: Scopes advertised by the TailorMed identity surface at auth.tailormed.com, plus the scopes the shipped TailorMed platform SPA actually requests. TailorMed publishes no OpenAPI and no public scopes reference page, so nothing here is derived from a spec — every scope below was read off a live response or a public JavaScript bundle.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Tailormed Scopes
name_suffix: OAuth Scopes
note: These are platform sign-in scopes. The Application Data API, Claims Data API and HL7/FHIR data-exchange surfaces are documented only behind the login on hub.tailormed.co, so any API-specific scope or permission model they use is not publicly readable.
overview: 'TailorMed uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TailorMed
provider_slug: tailormed
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tailormed-scopes
source_filename: tailormed-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://auth.tailormed.com/.well-known/openid-configuration\nname: TailorMed OAuth 2.0 / OpenID Connect scopes\ndescription: >-\n  Scopes advertised by the TailorMed identity surface at auth.tailormed.com, plus the\n  scopes the shipped TailorMed platform SPA actually requests. TailorMed publishes no\n  OpenAPI and no public scopes reference page, so nothing here is derived from a spec —\n  every scope below was read off a live response or a public JavaScript bundle.\nnote: >-\n  These are platform sign-in scopes. The Application Data API, Claims Data API and\n  HL7/FHIR data-exchange surfaces are documented only behind the login on\n  hub.tailormed.co, so any API-specific scope or permission model they use is not\n  publicly readable.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in; returns an ID token.\n  source: scopes_supported\n- name: profile\n  description: Basic profile claims (name, given_name, family_name,\
  \ preferred_username, locale, ...).\n  source: scopes_supported\n- name: email\n  description: email and email_verified claims.\n  source: scopes_supported\n- name: address\n  description: address claim.\n  source: scopes_supported\n- name: phone\n  description: phone_number claim.\n  source: scopes_supported\n- name: offline_access\n  description: Issues a refresh token.\n  source: scopes_supported\n- name: groups\n  description: Group membership claim used for platform authorization.\n  source: scopes_supported\n- name: 'tableau:views:embed'\n  description: >-\n    Custom scope requested by the TailorMed platform SPA to embed Tableau analytics\n    views inside the application.\n  source: >-\n    REACT_APP_OKTA_SCOPES in the public tenant bundle\n    /ap-search-client/0.37.1-2746777299/static/js/main.f597607c.js\nclaims_supported:\n- iss\n- ver\n- sub\n- aud\n- iat\n- exp\n- jti\n- auth_time\n- amr\n- idp\n- nonce\n- name\n- nickname\n- preferred_username\n- given_name\n- middle_name\n\
  - family_name\n- email\n- email_verified\n- profile\n- zoneinfo\n- locale\n- address\n- phone_number\n- picture\n- website\n- gender\n- birthdate\n- updated_at\n- at_hash\n- c_hash\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailormed/refs/heads/main/scopes/tailormed-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Health IT
- Medication Access
- Medication Affordability
- Financial Navigation
- Patient Assistance
- Pharmacy
- Oncology
- Revenue Cycle
- HL7
- FHIR
- Life Sciences
token_urls: []
---
