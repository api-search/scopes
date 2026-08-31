---
authorization_urls: []
description: The only OAuth scope surface Bloomberg publishes anonymously is the one advertised in the bloomberg.com OpenID Connect discovery document. The Data License / Hypermedia API also carries a scopes field inside its issued credential object, but that credential is provisioned under contract and its scope vocabulary is not published on any public page, so it is recorded as unpublished rather than guessed.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bloomberg Applications Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bloomberg Applications uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloomberg Applications
provider_slug: bloomberg-applications
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: bloomberg-applications-scopes
source_filename: bloomberg-applications-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://www.bloomberg.com/.well-known/openid-configuration\nprovider: Bloomberg Applications\nproviderId: bloomberg-applications\ndescription: >-\n  The only OAuth scope surface Bloomberg publishes anonymously is the one advertised in the\n  bloomberg.com OpenID Connect discovery document. The Data License / Hypermedia API also\n  carries a scopes field inside its issued credential object, but that credential is provisioned\n  under contract and its scope vocabulary is not published on any public page, so it is recorded\n  as unpublished rather than guessed.\nauthorization_server:\n  issuer: https://www.bloomberg.com\n  authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize\n  token_endpoint: https://login.bloomberg.com/api/oauth/token\n  jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json\n  grant_types_supported:\n    - authorization_code\n    - refresh_token\n  code_challenge_methods_supported:\n\
  \    - S256\nscopes:\n  - name: openid\n    description: >-\n      Standard OpenID Connect scope. Requests an id_token identifying the bloomberg.com account.\n      Signed RS256; keys at the published jwks_uri.\n    source: openid-configuration scopes_supported\n  - name: user\n    description: >-\n      Access to the authenticated user's bloomberg.com profile. Bloomberg publishes the scope\n      name in discovery but no claim-level reference page; description is limited to what the\n      discovery document states.\n    source: openid-configuration scopes_supported\n  - name: entitlements\n    description: >-\n      Access to the account's Bloomberg product entitlements. This is the scope that matters for\n      API consumers: Bloomberg's authorization model is entitlement-driven end to end, and the\n      same concept appears in BLPAPI as EMRS entitlements and NOT_ENTITLED_FIELD errors.\n    source: openid-configuration scopes_supported\nunpublished:\n  - api: Bloomberg Data API (Data\
  \ License / HAPI)\n    reason: >-\n      Credentials issued for api.bloomberg.com/eap carry a scopes array, but the scope vocabulary\n      is delivered with the credential under a Data License contract. No anonymous page enumerates\n      it and /.well-known/oauth-authorization-server on that host returns 403.\ndocs: null\ndocs_note: >-\n  No public scopes or permissions reference page was found. developer.bloomberg.com, which would\n  carry it, requires sign-in for every route.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-applications/refs/heads/main/scopes/bloomberg-applications-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Enterprise API
- Financial Analytics
- Financial-Services
- Market Data
- Real-Time Data
token_urls: []
---
