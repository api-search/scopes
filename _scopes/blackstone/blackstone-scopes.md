---
authorization_urls: []
description: Blackstone publishes no developer-facing OAuth scope catalog, because it publishes no developer API. The scopes recorded here are the ones its two identity issuers actually advertise in their anonymous discovery documents. They are identity scopes — who the user is — not business-capability scopes. Nothing here grants access to Blackstone fund, portfolio, or investor data; that access is negotiated in an LP or partner contract and mediated by a login.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Blackstone Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blackstone uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blackstone
provider_slug: blackstone
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: blackstone-scopes
source_filename: blackstone-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: >-\n  https://auth.bx.com/identity-broker/.well-known/openid-configuration and\n  https://login.bx.com/.well-known/oauth-authorization-server (both fetched 2026-08-10, HTTP 200)\nprovider: Blackstone\nproviderId: blackstone\ndescription: >-\n  Blackstone publishes no developer-facing OAuth scope catalog, because it publishes no\n  developer API. The scopes recorded here are the ones its two identity issuers actually\n  advertise in their anonymous discovery documents. They are identity scopes — who the user is —\n  not business-capability scopes. Nothing here grants access to Blackstone fund, portfolio, or\n  investor data; that access is negotiated in an LP or partner contract and mediated by a login.\nscope_count: 11\nbusiness_scopes_published: false\nissuers:\n  - issuer: https://auth.bx.com\n    discovery: https://auth.bx.com/identity-broker/.well-known/openid-configuration\n    applies_to: BXAccess investor portal\n    scopes:\n\
  \      - scope: openid\n        description: Required OIDC scope; requests an ID token asserting the investor's identity.\n      - scope: email\n        description: Releases the authenticated investor's email address claim.\n      - scope: phone\n        description: Releases the authenticated investor's phone-number claim.\n      - scope: profile\n        description: Releases standard OIDC profile claims (name, locale, updated_at, ...).\n    requested_by_the_portal: openid email profile\n    requested_by_source: https://www.bxaccess.com/bxa-next/env.json\n  - issuer: https://login.bx.com\n    discovery: https://login.bx.com/.well-known/openid-configuration\n    applies_to: Firmwide Blackstone SSO (Okta tenant), including docs.blackstone.com visitor auth\n    scopes:\n      - scope: openid\n        description: Required OIDC scope.\n      - scope: email\n        description: Email address claim.\n      - scope: profile\n        description: Standard profile claims.\n      - scope: address\n\
  \        description: Address claim.\n      - scope: phone\n        description: Phone-number claim.\n      - scope: offline_access\n        description: Issues a refresh token so a session can be renewed without re-prompting.\n      - scope: groups\n        description: >-\n          Releases the user's Okta group memberships — the claim that drives entitlement to\n          gated Blackstone surfaces such as docs.blackstone.com.\nnotes:\n  - >-\n    The org-level authorization server at https://login.bx.com/.well-known/oauth-authorization-server\n    additionally advertises Okta's own management-API scope catalog (okta.users.read,\n    okta.apps.manage, okta.logs.read, and ~60 more). Those are Okta platform scopes present on\n    every Okta tenant, NOT a Blackstone API. They are deliberately not enumerated here so the\n    catalog does not read as if Blackstone published sixty business scopes.\n  - >-\n    No scopes/permissions reference page exists on any public Blackstone property;\
  \ the\n    documentation site that might carry one (docs.blackstone.com) is behind Okta visitor auth.\ndocs: null\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackstone/refs/heads/main/scopes/blackstone-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Alternative Assets
- Finance
- Investment Management
- Private Equity
- Real-Estate
- Fortune 500
token_urls: []
---
