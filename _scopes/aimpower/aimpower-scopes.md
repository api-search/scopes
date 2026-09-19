---
authorization_urls: []
description: 'OAuth 2.0 / OpenID Connect scopes advertised by Brainsuite''s authorization server. The set is the stock Amazon Cognito OIDC scope list: identity scopes only. No resource or product scopes (for example an asset:write or report:read family for the Creative Effectiveness API) are advertised at the discovery endpoint, and no scope reference page is published. Any API-specific permission model is issued privately with credentials.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Aimpower Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Brainsuite.ai uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brainsuite.ai
provider_slug: aimpower
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: aimpower-scopes
source_filename: aimpower-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: >-\n  https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB/.well-known/openid-configuration\n  (HTTP 200, fetched 2026-09-14). Scopes are read verbatim from scopes_supported in that\n  document - not derived from a specification, because Brainsuite publishes none.\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by Brainsuite's authorization server. The\n  set is the stock Amazon Cognito OIDC scope list: identity scopes only. No resource or\n  product scopes (for example an asset:write or report:read family for the Creative\n  Effectiveness API) are advertised at the discovery endpoint, and no scope reference page\n  is published. Any API-specific permission model is issued privately with credentials.\nauthorization_server: https://auth.brainsuite.ai\nissuer: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_i8L26ssHB\ndocs: null\ndocs_note: No public scope or permissions reference page\
  \ was found on any Brainsuite host.\nscope_count: 4\nscopes:\n- name: openid\n  description: >-\n    Request an ID token and authenticate the end user via OpenID Connect. Standard OIDC\n    scope, required to receive an id_token.\n  standard: true\n- name: email\n  description: Release the end user's email address and email_verified claim to the client.\n  standard: true\n- name: phone\n  description: Release the end user's phone_number and phone_number_verified claims.\n  standard: true\n- name: profile\n  description: >-\n    Release the end user's default profile claims (name, family_name, given_name, picture,\n    locale and similar).\n  standard: true\nproduct_scopes_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimpower/refs/heads/main/scopes/aimpower-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- Marketing
- Artificial Intelligence
- Creative Effectiveness
- Ad Testing
- Market Research
- Consumer Neuroscience
- Media
- Software-as-a-Service
- Germany
token_urls: []
---
