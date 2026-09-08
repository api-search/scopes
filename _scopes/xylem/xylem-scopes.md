---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Xylem Scopes
name_suffix: OAuth Scopes
note: scopes_supported read verbatim from the Xylem Cloud (xCloud) Keycloak realm's OpenID Connect discovery document (HTTP 200, 2026-09-04). Xylem publishes no scopes or permissions reference page, so no descriptions beyond the standard OIDC/Keycloak meanings are asserted here — the two api:* entries are Xylem's own and are recorded exactly as advertised, including the trailing-colon entry, which appears to be an unfinished parent scope on the realm rather than a usable value. docs is null because no such page exists to link.
overview: 'Xylem uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xylem
provider_slug: xylem
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: xylem-scopes
source_filename: xylem-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://cloud.xylem.com/xcloud/auth/realms/xcloud/.well-known/openid-configuration\ndocs: null\nnote: >-\n  scopes_supported read verbatim from the Xylem Cloud (xCloud) Keycloak realm's OpenID\n  Connect discovery document (HTTP 200, 2026-09-04). Xylem publishes no scopes or\n  permissions reference page, so no descriptions beyond the standard OIDC/Keycloak\n  meanings are asserted here — the two api:* entries are Xylem's own and are recorded\n  exactly as advertised, including the trailing-colon entry, which appears to be an\n  unfinished parent scope on the realm rather than a usable value.\n  docs is null because no such page exists to link.\nissuer: https://cloud.xylem.com/xcloud/auth/realms/xcloud\nscope_count: 14\nscopes:\n  - name: openid\n    description: Required OIDC scope; requests an ID token.\n    standard: true\n  - name: profile\n    description: Standard OIDC claims — name, given_name, family_name, preferred_username.\n\
  \    standard: true\n  - name: email\n    description: Standard OIDC email and email_verified claims.\n    standard: true\n  - name: address\n    description: Standard OIDC address claim.\n    standard: true\n  - name: phone\n    description: Standard OIDC phone_number claims.\n    standard: true\n  - name: offline_access\n    description: Standard OIDC scope requesting a refresh token usable while the user is offline.\n    standard: true\n  - name: roles\n    description: Keycloak built-in — realm and client role mappings in the token.\n    standard: false\n  - name: web-origins\n    description: Keycloak built-in — allowed CORS web origins.\n    standard: false\n  - name: acr\n    description: Keycloak built-in — authentication context class reference claim.\n    standard: false\n  - name: microprofile-jwt\n    description: Keycloak built-in — Eclipse MicroProfile JWT claim set (upn, groups).\n    standard: false\n  - name: basic\n    description: Keycloak built-in — minimal claim set\
  \ (sub, auth_time).\n    standard: false\n  - name: service_account\n    description: >-\n      Xylem realm scope. Advertised alongside the client_credentials grant; the shape a\n      machine-to-machine integration would request. No published description.\n    standard: false\n    provider_defined: true\n  - name: api:customer\n    description: >-\n      Xylem realm scope naming customer-facing API access. No published description or\n      operation mapping — Xylem ships no API reference this can be bound to.\n    standard: false\n    provider_defined: true\n  - name: 'api:customer:'\n    description: >-\n      Advertised verbatim with a trailing colon. Recorded as found; it reads as an\n      unfinished or parent scope on the realm rather than a requestable value.\n    standard: false\n    provider_defined: true\n    anomaly: true\ngaps:\n  - No scopes or permissions reference page is published anywhere on xylem.com.\n  - >-\n    The two provider-defined api:* scopes carry no description\
  \ and no operation list,\n    so an integrator cannot tell what api:customer actually authorizes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/scopes/xylem-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fortune 1000
- Water
- Water Technology
- Utilities
- Smart Metering
- Industrial IoT
- Water Quality
- Wastewater
- Manufacturing
token_urls: []
---
