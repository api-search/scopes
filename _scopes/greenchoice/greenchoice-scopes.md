---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Greenchoice Scopes
name_suffix: OAuth Scopes
note: The scopes below are the complete scopes_supported array Greenchoice's own OpenID Connect discovery document advertises, read live on 2026-09-12. Greenchoice publishes no scope or permission reference page, so the descriptions for the two non-standard scopes record what can honestly be said about them and nothing more. No scope here was invented or inferred.
overview: 'Greenchoice uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Greenchoice
provider_slug: greenchoice
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: greenchoice-scopes
source_filename: greenchoice-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://sso.greenchoice.nl/.well-known/openid-configuration\nnote: >-\n  The scopes below are the complete scopes_supported array Greenchoice's own OpenID Connect\n  discovery document advertises, read live on 2026-09-12. Greenchoice publishes no scope or\n  permission reference page, so the descriptions for the two non-standard scopes record what\n  can honestly be said about them and nothing more. No scope here was invented or inferred.\ndocs: null\ndocs_note: No published scopes/permissions reference exists on any Greenchoice surface.\nissuer: https://sso.greenchoice.nl\nflows:\n  - type: authorization_code\n    authorizationUrl: https://sso.greenchoice.nl/connect/authorize\n    tokenUrl: https://sso.greenchoice.nl/connect/token\n  - type: client_credentials\n    tokenUrl: https://sso.greenchoice.nl/connect/token\n  - type: device_code\n    deviceAuthorizationUrl: https://sso.greenchoice.nl/connect/deviceauthorization\nscope_count:\
  \ 6\nscopes:\n  - name: openid\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Requests an ID token; required for any OIDC authentication request.\n  - name: profile\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: >-\n      Default profile claim set. This deployment advertises name, family_name, given_name,\n      middle_name, nickname, preferred_username, picture, website, gender, birthdate,\n      zoneinfo, locale and updated_at among claims_supported.\n  - name: email\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Releases the email and email_verified claims.\n  - name: offline_access\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Requests a refresh token for long-lived access.\n  - name: id\n    standard: false\n    description: >-\n      Non-standard scope advertised by this issuer. A matching `id` claim appears in\n      claims_supported alongside `klant_id` (customer id). Greenchoice\
  \ publishes no\n      definition; treated as an identifier-releasing scope, unverified.\n  - name: api-genesys-beheer\n    standard: false\n    description: >-\n      Non-standard scope. The name indicates administrative (\"beheer\") access to a Genesys\n      API — Genesys is the contact-centre platform Greenchoice operates. Its presence in a\n      public discovery document is the only evidence that any internal API exists behind this\n      issuer. Greenchoice publishes no definition, no documentation and no route for a third\n      party to be granted it.\nclaims_supported:\n  - sub\n  - auth_method\n  - stp\n  - account_type\n  - medewerker_afkorting\n  - updated_at\n  - locale\n  - zoneinfo\n  - birthdate\n  - gender\n  - website\n  - picture\n  - profile\n  - preferred_username\n  - nickname\n  - middle_name\n  - given_name\n  - family_name\n  - name\n  - emailAlreadyRegistered\n  - permission\n  - id\n  - email\n  - email_verified\n  - klant_id\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenchoice/refs/heads/main/scopes/greenchoice-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Electricity
- Gas
- Renewables
- Sustainability
- Netherlands
token_urls: []
---
