---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by American Woodmark's identity provider at id.woodmark.com, taken verbatim from the `scopes_supported` array of its live discovery document. American Woodmark publishes no scope reference page, so no description below is quoted from the provider — the standard OIDC scopes carry their OIDC Core 1.0 §5.4 meaning and the provider-specific ones are marked as undocumented rather than guessed at.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: American Woodmark Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'American Woodmark uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: American Woodmark
provider_slug: american-woodmark
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: american-woodmark-scopes
source_filename: american-woodmark-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://id.woodmark.com/.well-known/openid-configuration\nspecification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: American Woodmark\nproviderId: american-woodmark\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by American Woodmark's identity\n  provider at id.woodmark.com, taken verbatim from the `scopes_supported` array\n  of its live discovery document. American Woodmark publishes no scope\n  reference page, so no description below is quoted from the provider — the\n  standard OIDC scopes carry their OIDC Core 1.0 §5.4 meaning and the\n  provider-specific ones are marked as undocumented rather than guessed at.\nauthorization_server: https://id.woodmark.com\nauthorization_url: https://id.woodmark.com/connect/authorize\ntoken_url: https://id.woodmark.com/connect/token\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page is published. The corporate site\n  (www.americanwoodmark.com)\
  \ has no developer section — its sitemap.xml lists\n  140 URLs, none of which is developer, API or integration documentation.\nscope_count: 9\nscopes:\n  - name: openid\n    standard: OIDC Core 1.0\n    description: Requests an ID token; required for any OpenID Connect request.\n    documented_by_provider: false\n  - name: profile\n    standard: OIDC Core 1.0\n    description: >-\n      Default profile claims — name, family_name, given_name, middle_name,\n      nickname, preferred_username, picture, website, gender, birthdate,\n      zoneinfo, locale, updated_at.\n    documented_by_provider: false\n  - name: email\n    standard: OIDC Core 1.0\n    description: The email and email_verified claims.\n    documented_by_provider: false\n  - name: address\n    standard: OIDC Core 1.0\n    description: The address claim.\n    documented_by_provider: false\n  - name: phone\n    standard: OIDC Core 1.0\n    description: The phone_number and phone_number_verified claims.\n    documented_by_provider:\
  \ false\n  - name: offline_access\n    standard: OIDC Core 1.0\n    description: Requests a refresh token for access when the user is not present.\n    documented_by_provider: false\n  - name: roles\n    standard: provider-specific\n    description: >-\n      Releases the `roles` and `role_name` claims (both appear in\n      claims_supported). American Woodmark publishes no description of what\n      roles exist or what they grant.\n    documented_by_provider: false\n  - name: permissions\n    standard: provider-specific\n    description: >-\n      Releases the `permissions` and `permission_name` claims (both appear in\n      claims_supported). The permission vocabulary is not published.\n    documented_by_provider: false\n  - name: TestClient\n    standard: provider-specific\n    description: >-\n      Named scope advertised on the PRODUCTION issuer. Its purpose is not\n      documented. Recorded verbatim because it is in scopes_supported; no\n      meaning is inferred.\n    documented_by_provider:\
  \ false\n    note: A test-shaped scope advertised on a production authorization server.\nclaims_supported:\n  - address\n  - email_verified\n  - email\n  - sub\n  - phone_number_verified\n  - phone_number\n  - zoneinfo\n  - birthdate\n  - gender\n  - website\n  - picture\n  - profile\n  - preferred_username\n  - nickname\n  - middle_name\n  - given_name\n  - family_name\n  - name\n  - locale\n  - updated_at\n  - role_name\n  - summary\n  - permission_name\n  - MinimumVersion\n  - MaximumVersion\n  - permissions\n  - roles\nclaims_note: >-\n  `MinimumVersion` and `MaximumVersion` are non-standard claims, suggesting the\n  IdP pins a client-version floor/ceiling per token. Undocumented.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-woodmark/refs/heads/main/scopes/american-woodmark-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Cabinetry
- Home Products
- Construction
- Building Products
- Manufacturing
- Kitchen and Bath
- Home Improvement
- Identity
- EDI
- Supply Chain
token_urls: []
---
