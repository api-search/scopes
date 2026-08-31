---
authorization_urls: []
description: 'Scopes advertised by the Blameless Auth0 identity tenant''s OIDC discovery document, fetched 2026-08-29. IMPORTANT: these are the tenant''s standard OIDC identity scopes, not Blameless API permission scopes. Blameless'' API authorization was rule-based (named rules such as IncidentRead), and that rule catalogue was published only on docs.blameless.com, which no longer resolves — so no API scope list can be recovered. Nothing here is derived from an OpenAPI; Blameless never published one.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Blameless Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blameless uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blameless
provider_slug: blameless
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: blameless-scopes
source_filename: blameless-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://blamelesshq.auth0.com/.well-known/openid-configuration\nspecification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Blameless\nproviderId: blameless\ndescription: >-\n  Scopes advertised by the Blameless Auth0 identity tenant's OIDC discovery document,\n  fetched 2026-08-29. IMPORTANT: these are the tenant's standard OIDC identity scopes, not\n  Blameless API permission scopes. Blameless' API authorization was rule-based\n  (named rules such as IncidentRead), and that rule catalogue was published only on\n  docs.blameless.com, which no longer resolves — so no API scope list can be recovered.\n  Nothing here is derived from an OpenAPI; Blameless never published one.\nissuer: https://blamelesshq.auth0.com/\nauthorization_endpoint: https://blamelesshq.auth0.com/authorize\ntoken_endpoint: https://blamelesshq.auth0.com/oauth/token\ngrant_types_supported:\n  - client_credentials\n  - authorization_code\n\
  \  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\ncode_challenge_methods_supported:\n  - S256\n  - plain\nscopes:\n  - name: openid\n    kind: oidc\n    description: Standard OIDC scope requesting an ID token.\n  - name: profile\n    kind: oidc\n    description: Basic profile claims.\n  - name: offline_access\n    kind: oidc\n    description: Requests a refresh token.\n  - name: email\n    kind: oidc\n  - name: email_verified\n    kind: oidc\n  - name: name\n    kind: oidc\n  - name: given_name\n    kind: oidc\n  - name: family_name\n    kind: oidc\n  - name: nickname\n    kind: oidc\n  - name: picture\n    kind: oidc\n  - name: phone\n    kind: oidc\n  - name: address\n    kind: oidc\n  - name: created_at\n    kind: oidc\n  - name: identities\n    kind: oidc\napi_scopes:\n  count: 0\n  note: >-\n    No Blameless API scope catalogue is recoverable.\
  \ The API used named access-control\n    rules rather than OAuth scopes, and the page documenting them is gone.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blameless/refs/heads/main/scopes/blameless-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AIOps
- SRE
- Incident Management
- Reliability
- Service Level Objectives
- Retrospectives
- On-Call
- DevOps
token_urls: []
---
