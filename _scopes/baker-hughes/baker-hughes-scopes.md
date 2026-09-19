---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Baker Hughes Scopes
name_suffix: OAuth Scopes
note: scopes_supported read verbatim from the Keycloak realm's OIDC discovery document. Baker Hughes publishes no scope reference page, so descriptions are limited to what the OIDC Core spec defines (openid/profile/email) and what the scope NAME says for the two custom ones; nothing about what tenant-scope or abac_scope grants is asserted.
overview: 'Baker Hughes uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Baker Hughes
provider_slug: baker-hughes
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: baker-hughes-scopes
source_filename: baker-hughes-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: https://auth-developer.bakerhughes.com/auth/realms/dedicated/.well-known/openid-configuration\nprovider: Baker Hughes\nproviderId: baker-hughes\nissuer: https://auth-developer.bakerhughes.com/auth/realms/dedicated\ndocs: null\nnote: scopes_supported read verbatim from the Keycloak realm's OIDC discovery document. Baker Hughes publishes no\n  scope reference page, so descriptions are limited to what the OIDC Core spec defines (openid/profile/email) and\n  what the scope NAME says for the two custom ones; nothing about what tenant-scope or abac_scope grants is asserted.\nscopes:\n- name: openid\n  description: OpenID Connect authentication request (OIDC Core 3.1.2.1).\n  standard: true\n- name: profile\n  description: Standard OIDC profile claims (name, family_name, given_name, ...).\n  standard: true\n- name: email\n  description: Standard OIDC email + email_verified claims.\n  standard: true\n- name: tenant-scope\n  description:\
  \ Custom realm scope. Name suggests tenant selection for the multi-tenant Cordant platform; semantics\n    not published.\n  standard: false\n- name: abac_scope\n  description: Custom realm scope. Name suggests attribute-based access control claims; semantics not published.\n  standard: false\nobserved_requests:\n- client_id: app-cdp\n  scope: openid profile email\n  context: developer.bakerhughes.com sign-in\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baker-hughes/refs/heads/main/scopes/baker-hughes-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy Technology
- Industrial IoT
- Oil and Gas
- Asset Performance Management
- Digital Energy
- Fortune 500
token_urls: []
---
