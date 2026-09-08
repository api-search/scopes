---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Express Scripts Holding Scopes
name_suffix: OAuth Scopes
note: No scopes/permissions reference page is publicly reachable — the developer portal renders client-side and its content backend answers 403 to anonymous requests. Everything below is read from documents the provider serves anonymously. The one Express Scripts-specific scope in the estate is `esrx.default`; every other scope advertised on the default authorization server is a standard OIDC or Okta scope.
overview: 'Express Scripts Holding uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Express Scripts Holding
provider_slug: express-scripts-holding
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: express-scripts-holding-scopes
source_filename: express-scripts-holding-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  scopes_supported from the two fetched OAuth/OIDC discovery documents, plus the\n  scope array the developer portal's own OIDC client requests, read from\n  https://developer.express-scripts.com/assets/index-F-3lEwAf.js\nnote: >-\n  No scopes/permissions reference page is publicly reachable — the developer portal\n  renders client-side and its content backend answers 403 to anonymous requests.\n  Everything below is read from documents the provider serves anonymously. The one\n  Express Scripts-specific scope in the estate is `esrx.default`; every other scope\n  advertised on the default authorization server is a standard OIDC or Okta scope.\ndocs: null\ndocs_note: >-\n  No public scopes reference found. The API-specific scopes behind `esrx.default`\n  are not published and would need an authenticated portal session to enumerate.\nauthorization_servers:\n  - issuer: https://p1-express-scripts.okta.com/oauth2/default\n  \
  \  vanity: https://p.login.developer.express-scripts.com/oauth2/default\n    role: The authorization server the developer portal authenticates against.\n  - issuer: https://p.login.developer.express-scripts.com\n    role: >-\n      Okta org-level authorization server. Advertises client_credentials and the Okta\n      management scope set; not the partner API path.\nscopes:\n  - name: esrx.default\n    source: portal-client\n    first_party: true\n    description: >-\n      The Express Scripts application scope requested by the developer portal client.\n      This is the only vendor-namespaced scope observed in the estate. What it grants\n      is not published; the scope name is recorded, its permissions are not known.\n    evidence: developer portal OIDC client scope array\n  - name: openid\n    source: discovery\n    standard: OpenID Connect Core 1.0\n    description: Requests an ID token. Required for any OIDC flow.\n  - name: profile\n    source: discovery\n    standard: OpenID Connect\
  \ Core 1.0\n    description: Basic profile claims (name, preferred_username, locale, updated_at).\n  - name: email\n    source: discovery\n    standard: OpenID Connect Core 1.0\n    description: email and email_verified claims.\n  - name: address\n    source: discovery\n    standard: OpenID Connect Core 1.0\n    description: The address claim.\n  - name: phone\n    source: discovery\n    standard: OpenID Connect Core 1.0\n    description: phone_number and phone_number_verified claims.\n  - name: offline_access\n    source: discovery\n    standard: OpenID Connect Core 1.0\n    description: Requests a refresh token.\n  - name: groups\n    source: discovery\n    server: org-level\n    description: Group membership claim. Advertised on the org authorization server.\n  - name: device_sso\n    source: discovery\n    server: default\n    description: Okta device single sign-on.\n  - name: interclient_access\n    source: discovery\n    server: default\n    description: Okta cross-client token\
  \ exchange.\ncounts:\n  total: 10\n  first_party: 1\n  standard_oidc: 6\n  vendor_platform: 3\ngaps:\n  - >-\n    No per-API or per-operation scope is published. `esrx.default` is a single coarse\n    application scope; there is no evidence of least-privilege scoping on the partner\n    APIs, and no public document maps a scope to a capability.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/express-scripts-holding/refs/heads/main/scopes/express-scripts-holding-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Health
- Healthcare
- Pharmacy
- Pharmacy Benefit Management
- Prescriptions
- Claims
- Fortune 100
token_urls: []
---
