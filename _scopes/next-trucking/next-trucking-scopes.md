---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Next Trucking Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NEXT Trucking uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NEXT Trucking
provider_slug: next-trucking
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: next-trucking-scopes
source_filename: next-trucking-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  scopes_supported in https://prod-nexttrucking.us.auth0.com/.well-known/openid-configuration\n  (HTTP 200, saved verbatim to well-known/next-trucking-openid-configuration.json).\ndocs: null\nsummary: >-\n  The only scope set NEXT Trucking exposes anonymously is the stock OpenID Connect profile advertised\n  by its Auth0 tenant. These are identity scopes, NOT application permissions: nothing here grants\n  access to loads, quotes, trips, documents or any ATLAS resource. No API permission reference is\n  published, and the resource scopes the ATLAS gateway actually enforces are not discoverable without\n  credentials.\nprovider: auth0\nissuer: https://prod-nexttrucking.us.auth0.com/\nflows:\n  authorization_code:\n    authorizationUrl: https://prod-nexttrucking.us.auth0.com/authorize\n    tokenUrl: https://prod-nexttrucking.us.auth0.com/oauth/token\n    pkce: S256\n  client_credentials:\n    tokenUrl: https://prod-nexttrucking.us.auth0.com/oauth/token\n\
  \    note: Advertised, but no audience or third-party client registration is published.\nscope_count: 14\nscopes:\n  - name: openid\n    description: Request an ID token (OpenID Connect).\n    kind: identity\n  - name: profile\n    description: Basic profile claims for the authenticated user.\n    kind: identity\n  - name: offline_access\n    description: Issue a refresh token.\n    kind: identity\n  - name: name\n    description: The user's full name claim.\n    kind: identity\n  - name: given_name\n    description: The user's given name claim.\n    kind: identity\n  - name: family_name\n    description: The user's family name claim.\n    kind: identity\n  - name: nickname\n    description: The user's nickname claim.\n    kind: identity\n  - name: email\n    description: The user's email address claim.\n    kind: identity\n  - name: email_verified\n    description: Whether the user's email address has been verified.\n    kind: identity\n  - name: picture\n    description: The user's profile\
  \ picture claim.\n    kind: identity\n  - name: created_at\n    description: Account creation timestamp claim.\n    kind: identity\n  - name: identities\n    description: Linked identity providers for the account.\n    kind: identity\n  - name: phone\n    description: The user's phone number claim.\n    kind: identity\n  - name: address\n    description: The user's address claim.\n    kind: identity\nresource_scopes:\n  published: false\n  note: >-\n    No NEXT-Trucking-specific API scopes (loads, containers, appointments, documents, payables) are\n    published anywhere. The ATLAS gateway returns 401 to every anonymous request, so its authorization\n    model cannot be introspected without credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-trucking/refs/heads/main/scopes/next-trucking-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Logistics
- Freight
- Trucking
- Drayage
- Supply Chain
- Transportation
- Marketplace
- Transportation Management
- Shipping
token_urls: []
---
