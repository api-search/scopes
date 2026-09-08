---
authorization_urls: []
description: 'The complete scopes_supported list advertised by 4.screen''s Keycloak realm. Two of these are first-party business scopes that map directly onto 4.screen''s two-sided marketplace — the demand side (advertisers and businesses buying in-car placements) and the supply side (automakers and mobility service providers serving them). The rest are Keycloak/OIDC standard scopes. NOTE: which scope each API operation requires is NOT published — there is no public API reference — so the descriptions of the two first-party scopes below are marked inferred and must not be read as documented behaviour.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: 4Screen Scopes
name_suffix: OAuth Scopes
note: ''
overview: '4.screen uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 4.screen
provider_slug: 4screen
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: 4screen-scopes
source_filename: 4screen-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://api.4screen.com/auth/realms/fourscreen/.well-known/openid-configuration\ndocs: null\nname: 4.screen OAuth 2.0 scopes\ndescription: >-\n  The complete scopes_supported list advertised by 4.screen's Keycloak realm.\n  Two of these are first-party business scopes that map directly onto 4.screen's\n  two-sided marketplace — the demand side (advertisers and businesses buying\n  in-car placements) and the supply side (automakers and mobility service\n  providers serving them). The rest are Keycloak/OIDC standard scopes.\n  NOTE: which scope each API operation requires is NOT published — there is no\n  public API reference — so the descriptions of the two first-party scopes below\n  are marked inferred and must not be read as documented behaviour.\n\nissuer: https://api.4screen.com/auth/realms/fourscreen\nauthorization_endpoint: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/auth\ntoken_endpoint: https://api.4screen.com/auth/realms/fourscreen/protocol/openid-connect/token\n\
  scope_count: 14\nfirst_party_scope_count: 3\n\nscopes:\n  - name: demand-client-scope\n    category: first-party\n    documented: false\n    description: >-\n      INFERRED, not documented. 4.screen's own naming for the demand side of its\n      marketplace — the businesses, brands and agencies that buy Branded Pins,\n      Sponsored Search, Recommendations and Detail Screen placements. This is the\n      scope the 4.screen customer portal client would carry.\n  - name: supply-operations-client-scope\n    category: first-party\n    documented: false\n    description: >-\n      INFERRED, not documented. 4.screen's own naming for the supply side — the\n      automaker/OEM and mobility-service-provider integrations that render\n      4.screen content inside an infotainment system, plus the operational\n      tooling around them.\n  - name: service_account\n    category: first-party\n    documented: false\n    description: >-\n      Keycloak service-account scope, used by client_credentials\
  \ machine clients.\n      Present in the realm's scopes_supported list.\n\n  - name: openid\n    category: oidc-standard\n    documented: true\n    description: Required to request an ID token (OpenID Connect Core 1.0).\n  - name: profile\n    category: oidc-standard\n    documented: true\n    description: name, given_name, family_name, preferred_username claims.\n  - name: email\n    category: oidc-standard\n    documented: true\n    description: email claim.\n  - name: phone\n    category: oidc-standard\n    documented: true\n    description: phone_number claims.\n  - name: address\n    category: oidc-standard\n    documented: true\n    description: address claim.\n  - name: offline_access\n    category: oidc-standard\n    documented: true\n    description: Issues a refresh token usable while the user is offline.\n  - name: acr\n    category: keycloak-default\n    documented: true\n    description: Authentication Context Class Reference claim (acr_values 0 and 1 advertised).\n  - name:\
  \ basic\n    category: keycloak-default\n    documented: true\n    description: Keycloak default client scope carrying sub and auth_time.\n  - name: roles\n    category: keycloak-default\n    documented: true\n    description: Realm and client role mappings in the token.\n  - name: web-origins\n    category: keycloak-default\n    documented: true\n    description: CORS allowed-origins mapper.\n  - name: microprofile-jwt\n    category: keycloak-default\n    documented: true\n    description: Eclipse MicroProfile JWT claims (upn, groups).\n\ngaps:\n  - >-\n    No scopes/permissions reference page exists on any public 4.screen surface.\n    docs: is null for that reason, not because the search was skipped —\n    docs.4screen.com and developer.4screen.com do not resolve in DNS, and\n    4screen.com has no developer section in its sitemap.\n  - >-\n    Operation-to-scope mapping is unavailable because api.4screen.com returns\n    401 on every springdoc/OpenAPI path and on /graphql.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4screen/refs/heads/main/scopes/4screen-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- AdTech
- Automotive
- Mobility
- Connected Vehicle
- In-Car Commerce
- Location
- Navigation
- Marketing
- Germany
token_urls: []
---
