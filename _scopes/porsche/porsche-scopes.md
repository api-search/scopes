---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the Porsche ID identity provider. Read verbatim from the scopes_supported array of the anonymous discovery document at identity.porsche.com. These are the standard OIDC identity scopes only — Porsche publishes no API-resource scope reference, because the APIs behind Porsche ID are partner-gated and their scope catalog is not public.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Porsche Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Porsche uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Porsche
provider_slug: porsche
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: porsche-scopes
source_filename: porsche-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://identity.porsche.com/.well-known/openid-configuration\nprovider: Porsche\nproviderId: porsche\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the Porsche ID identity provider. Read\n  verbatim from the scopes_supported array of the anonymous discovery document at\n  identity.porsche.com. These are the standard OIDC identity scopes only — Porsche\n  publishes no API-resource scope reference, because the APIs behind Porsche ID are\n  partner-gated and their scope catalog is not public.\nauthorization_server: https://identity.porsche.com/\ndocs: null\ndocs_note: >-\n  No public scopes/permissions reference page found. The Porsche ID Developer Portal\n  (developer.porsche.com) exposes only a landing page, terms, privacy policy and FAQ\n  anonymously; the API reference sits behind portal.developer.porsche.com, which requires\n  a Microsoft Entra ID login.\nscope_count: 14\nscopes:\n  - name: openid\n  \
  \  description: Request an ID token and initiate an OpenID Connect flow.\n    standard: OIDC Core 1.0\n  - name: profile\n    description: Access the end user's default profile claims.\n    standard: OIDC Core 1.0\n  - name: offline_access\n    description: Request a refresh token for long-lived access.\n    standard: OIDC Core 1.0\n  - name: name\n    description: Full name claim.\n  - name: given_name\n    description: Given name claim.\n  - name: family_name\n    description: Family name claim.\n  - name: nickname\n    description: Nickname claim.\n  - name: email\n    description: Email address claim.\n  - name: email_verified\n    description: Whether the email address has been verified.\n  - name: picture\n    description: Profile picture URL claim.\n  - name: created_at\n    description: Account creation timestamp claim.\n  - name: identities\n    description: Linked external identity providers for the account.\n  - name: phone\n    description: Phone number claim.\n  - name: address\n\
  \    description: Postal address claim.\nevidence:\n  - url: https://identity.porsche.com/.well-known/openid-configuration\n    status: 200\n  - url: https://developer.porsche.com/faq\n    status: 200\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/porsche/refs/heads/main/scopes/porsche-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Automobiles
- Cars
- Vehicles
- Automotive
- Connected Car
- Identity
- OpenID Connect
- Design System
- Open Source
- Germany
token_urls: []
---
