---
authorization_urls: []
description: OAuth 2.0 scopes advertised by the Diligent Pharma authorization server (clerk.diligentpharma.com), the Clerk-hosted identity provider behind the Diligent360 application. These are identity/profile scopes for application sign-in, not resource scopes over a published Diligent Pharma API — Diligent Pharma publishes no developer API and no scopes reference page. Recorded verbatim from the discovery document; nothing here is inferred.
docs: https://clerk.com/docs/oauth/scoped-access
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Diligent Pharma Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Diligent Pharma uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Diligent Pharma
provider_slug: diligent-pharma
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: diligent-pharma-scopes
source_filename: diligent-pharma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://clerk.diligentpharma.com/.well-known/oauth-authorization-server\ndescription: >-\n  OAuth 2.0 scopes advertised by the Diligent Pharma authorization server\n  (clerk.diligentpharma.com), the Clerk-hosted identity provider behind the\n  Diligent360 application. These are identity/profile scopes for application sign-in,\n  not resource scopes over a published Diligent Pharma API — Diligent Pharma publishes\n  no developer API and no scopes reference page. Recorded verbatim from the discovery\n  document; nothing here is inferred.\nauthorization_server: https://clerk.diligentpharma.com\ndocs: https://clerk.com/docs/oauth/scoped-access\ndocs_note: >-\n  service_documentation in the discovery document points at Clerk's own generic\n  documentation, not at a Diligent Pharma scopes reference. No provider-authored\n  scope documentation exists.\nscope_type: identity\nresource_scopes_published: false\nscope_count: 6\nscopes:\n\
  \  - name: openid\n    description: OpenID Connect sign-in; requests an ID token for the authenticated user.\n    standard: true\n  - name: profile\n    description: >-\n      Basic profile claims — name, given_name, family_name, preferred_username, picture.\n    standard: true\n  - name: email\n    description: Email address and its verification state (email, email_verified claims).\n    standard: true\n  - name: offline_access\n    description: Issues a refresh token so the client can renew access without re-prompting.\n    standard: true\n  - name: public_metadata\n    description: >-\n      Clerk public metadata attached to the user record — application-defined,\n      readable by the client and the frontend.\n    standard: false\n  - name: private_metadata\n    description: >-\n      Clerk private metadata attached to the user record — application-defined,\n      backend-only data.\n    standard: false\nclaims_supported:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - email\n  -\
  \ email_verified\n  - preferred_username\n  - given_name\n  - family_name\n  - name\n  - picture\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diligent-pharma/refs/heads/main/scopes/diligent-pharma-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Clinical Trials
- Life Sciences
- Pharmaceuticals
- Biotechnology
- Vendor Management
- Risk Management
- Quality Management
- Compliance
- GxP
- Auditing
- Software-as-a-Service
token_urls: []
---
