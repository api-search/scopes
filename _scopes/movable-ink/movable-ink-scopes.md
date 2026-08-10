---
authorization_urls: []
description: Scopes advertised by the Movable Ink identity tenant (auth.movableink.com, an Auth0 tenant) in its OpenID Connect discovery document. These are the standard OIDC identity scopes that govern login to the Movable Ink Studio application — they are NOT API authorization scopes. The Customer Data API uses HTTP Basic authentication and has no scope model at all; see authentication/movable-ink-authentication.yml.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Movable Ink Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Movable Ink uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Movable Ink
provider_slug: movable-ink
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: movable-ink-scopes
source_filename: movable-ink-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://auth.movableink.com/.well-known/openid-configuration\nname: Movable Ink OAuth / OpenID Connect Scopes\ndescription: >-\n  Scopes advertised by the Movable Ink identity tenant (auth.movableink.com, an\n  Auth0 tenant) in its OpenID Connect discovery document. These are the standard\n  OIDC identity scopes that govern login to the Movable Ink Studio application —\n  they are NOT API authorization scopes. The Customer Data API uses HTTP Basic\n  authentication and has no scope model at all; see\n  authentication/movable-ink-authentication.yml.\nissuer: https://auth.movableink.com/\nauthorization_endpoint: https://auth.movableink.com/authorize\ntoken_endpoint: https://auth.movableink.com/oauth/token\nscopes:\n  - name: openid\n    description: Request an ID token — signals an OpenID Connect authentication request.\n  - name: profile\n    description: Basic profile claims (name, given_name, family_name, nickname, picture).\n\
  \  - name: offline_access\n    description: Issue a refresh token so the session can be renewed without re-prompting.\n  - name: email\n    description: The user's email address.\n  - name: email_verified\n    description: Whether the user's email address has been verified.\n  - name: name\n    description: The user's full display name.\n  - name: given_name\n    description: The user's given (first) name.\n  - name: family_name\n    description: The user's family (last) name.\n  - name: nickname\n    description: The user's nickname.\n  - name: picture\n    description: URL of the user's profile picture.\n  - name: created_at\n    description: When the user account was created.\n  - name: identities\n    description: Linked identity-provider identities for the user.\n  - name: phone\n    description: The user's phone number.\n  - name: address\n    description: The user's address.\nobserved_in_use:\n  scopes: [openid, profile, email, offline_access]\n  where: >-\n    The 302 from https://app.movableink.com/\
  \ carries\n    scope=openid+profile+email+offline_access on the authorize request.\nnotes:\n  - No resource-server / API scopes (audience-bound permissions) are advertised\n    anonymously. Any per-product authorization inside Studio or Da Vinci is not\n    expressed as a public OAuth scope.\n  - Movable Ink publishes no scopes or permissions reference page on a public URL.\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n    - url: https://auth.movableink.com/.well-known/openid-configuration\n      status: 200\n    - url: https://app.movableink.com/\n      status: 302\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/movable-ink/refs/heads/main/scopes/movable-ink-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Personalization
- Email
- Customer Data
- Mobile SDK
- Artificial Intelligence
- Advertising Technology
- Content
- Events
token_urls: []
---
