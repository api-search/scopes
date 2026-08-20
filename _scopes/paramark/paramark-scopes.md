---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Paramark Scopes
name_suffix: OAuth Scopes
note: Read verbatim from the scopes_supported array of Paramark's own OpenID Connect discovery document and confirmed identical in its OAuth 2.0 Authorization Server Metadata document. These are the four standard OIDC scopes; Paramark advertises no product- or resource-scoped permissions at the authorization server, and publishes no scopes/permissions reference page. Nothing here is inferred — no API-level scope vocabulary was found, and none is invented.
overview: 'Paramark uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paramark
provider_slug: paramark
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: paramark-scopes
source_filename: paramark-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://signin.paramark.com/.well-known/openid-configuration\nnote: >-\n  Read verbatim from the scopes_supported array of Paramark's own OpenID Connect discovery\n  document and confirmed identical in its OAuth 2.0 Authorization Server Metadata document.\n  These are the four standard OIDC scopes; Paramark advertises no product- or resource-scoped\n  permissions at the authorization server, and publishes no scopes/permissions reference page.\n  Nothing here is inferred — no API-level scope vocabulary was found, and none is invented.\nissuer: https://signin.paramark.com\nauthorization_endpoint: https://signin.paramark.com/oauth2/authorize\ntoken_endpoint: https://signin.paramark.com/oauth2/token\nflows:\n- authorization_code\n- client_credentials\n- refresh_token\n- urn:ietf:params:oauth:grant-type:device_code\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OIDC scope; requests an ID token identifying the authenticated\n\
  \    end user.\n  standard: true\n- name: profile\n  description: Standard OIDC scope; requests the end user's default profile claims.\n  standard: true\n- name: email\n  description: Standard OIDC scope; requests the end user's email address and its\n    verification status.\n  standard: true\n- name: offline_access\n  description: Standard OIDC scope; requests a refresh token so the client can obtain\n    new access tokens without the end user present.\n  standard: true\nproduct_scopes_published: false\ndocs: null\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://signin.paramark.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paramark/refs/heads/main/scopes/paramark-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Application
- Marketing
- Analytics
- Measurements
- Marketing Mix Modeling
- Incrementality
- Advertising
- Artificial Intelligence
token_urls: []
---
