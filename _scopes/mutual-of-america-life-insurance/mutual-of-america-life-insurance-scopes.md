---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Mutual Of America Life Insurance Scopes
name_suffix: OAuth Scopes
note: 'Read verbatim from `scopes_supported` in the two discovery documents saved under well-known/. IMPORTANT READING NOTE: the OpenID Connect document advertises the standard OIDC scope set and nothing bespoke — Mutual of America has defined no product scopes of its own, because it ships no public API. The RFC 8414 document additionally advertises the full `okta.*` management scope set; those are the identity vendor''s platform-administration scopes present on every Okta org authorization server, NOT scopes Mutual of America authored or exposes to third parties. They are recorded here for completeness and marked `vendor_platform: true` so they are never mistaken for a Mutual of America API surface.'
overview: 'Mutual of America Life Insurance Company uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mutual of America Life Insurance Company
provider_slug: mutual-of-america-life-insurance
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: mutual-of-america-life-insurance-scopes
source_filename: mutual-of-america-life-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://login.mutualofamerica.com/.well-known/openid-configuration\nissuer: https://login.mutualofamerica.com\nnote: >-\n  Read verbatim from `scopes_supported` in the two discovery documents saved under well-known/.\n  IMPORTANT READING NOTE: the OpenID Connect document advertises the standard OIDC scope set\n  and nothing bespoke — Mutual of America has defined no product scopes of its own, because it\n  ships no public API. The RFC 8414 document additionally advertises the full `okta.*`\n  management scope set; those are the identity vendor's platform-administration scopes present\n  on every Okta org authorization server, NOT scopes Mutual of America authored or exposes to\n  third parties. They are recorded here for completeness and marked `vendor_platform: true` so\n  they are never mistaken for a Mutual of America API surface.\nscope_count: 7\nscopes:\n  - name: openid\n    description: Required for OpenID Connect; requests\
  \ an ID token.\n  - name: email\n    description: Email address and email_verified claims.\n  - name: profile\n    description: Default profile claims (name, family_name, given_name, locale, zoneinfo…).\n  - name: address\n    description: End-user postal address claim.\n  - name: phone\n    description: phone_number and phone_number_verified claims.\n  - name: offline_access\n    description: Requests a refresh token for long-lived sessions.\n  - name: groups\n    description: Group membership claim, used to drive portal entitlements.\nvendor_platform_scopes:\n  vendor_platform: true\n  source: https://login.mutualofamerica.com/.well-known/oauth-authorization-server\n  count: 82\n  note: >-\n    Okta org-management scopes (okta.users.*, okta.groups.*, okta.apps.*, okta.policies.*,\n    okta.logs.read, okta.apiTokens.*, …) advertised by the Okta org authorization server.\n    Reachable only by administrators of the tenant. Not a Mutual of America API product.\ndocs: null\ndocs_note: >-\n\
  \  No scopes/permissions reference page is published. Mutual of America has no developer portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutual-of-america-life-insurance/refs/heads/main/scopes/mutual-of-america-life-insurance-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Life Insurance
- Retirement
- Financial Services
- Pensions
- Annuities
- Wealth Management
- Identity
token_urls: []
---
