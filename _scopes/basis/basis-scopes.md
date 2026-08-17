---
api_specs:
- filename: basis-analytics-api-openapi.yml
  format: yaml
  label: Basis Analytics API
  slug: basis-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis/refs/heads/main/openapi/basis-analytics-api-openapi.yml
authorization_urls: []
description: The Basis Platform API delegates authorization to an OpenID Connect provider at https://auth.basis.net (Auth0). The API's own OpenAPI declares a securityScheme named `OAuth2` with no flows object and therefore no scopes, so the scope surface below is taken from the authorization server's published discovery document and from the authorize-URL example in the Basis documentation. These are OIDC identity scopes plus `offline_access`; Basis publishes no resource-level (read/write per-object) scopes for the Analytics API — access is scoped by the credential's owner (agency) and by client-credentials audience, not by scope strings.
docs: https://api.basis.net/swagger.json
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Basis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Basis uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Basis
provider_slug: basis
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: basis-scopes
source_filename: basis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://auth.basis.net/.well-known/openid-configuration (probed 2026-08-13,\n  HTTP 200) and the Authentication section of the Basis Platform API description\n  published at https://api.basis.net/swagger.json.\ndocs: https://api.basis.net/swagger.json\ndescription: >-\n  The Basis Platform API delegates authorization to an OpenID Connect provider at\n  https://auth.basis.net (Auth0). The API's own OpenAPI declares a securityScheme\n  named `OAuth2` with no flows object and therefore no scopes, so the scope\n  surface below is taken from the authorization server's published discovery\n  document and from the authorize-URL example in the Basis documentation. These\n  are OIDC identity scopes plus `offline_access`; Basis publishes no\n  resource-level (read/write per-object) scopes for the Analytics API — access is\n  scoped by the credential's owner (agency) and by client-credentials audience,\n  not by scope strings.\n\
  authorization_server:\n  issuer: https://auth.basis.net/\n  authorization_endpoint: https://auth.basis.net/authorize\n  token_endpoint: https://auth.basis.net/oauth/token\n  jwks_uri: https://auth.basis.net/.well-known/jwks.json\n  revocation_endpoint: https://auth.basis.net/oauth/revoke\n  audience: https://api.basis.net\n  discovery: well-known/basis-openid-configuration.json\ndocumented_request_scopes:\n  source: >-\n    Verbatim from the Basis authorize-URL example — \"scope=openid profile email\n    offline_access\".\n  scopes:\n    - name: openid\n      description: Required to obtain an ID token from the OpenID Connect provider.\n    - name: profile\n      description: Basic profile claims (name, given_name, family_name, nickname, picture).\n    - name: email\n      description: Email address and email_verified claim.\n    - name: offline_access\n      description: >-\n        Required to receive a refresh token. Basis notes that only the\n        authorization-code flow returns\
  \ a refresh token.\nsupported_scopes:\n  source: scopes_supported in the authorization server discovery document\n  scopes:\n    - openid\n    - profile\n    - offline_access\n    - name\n    - given_name\n    - family_name\n    - nickname\n    - email\n    - email_verified\n    - picture\n    - created_at\n    - identities\n    - phone\n    - address\nresource_scopes:\n  published: false\n  note: >-\n    No per-resource or per-operation scopes are published for the Analytics API.\n    Every operation in openapi/basis-analytics-api-openapi.yml declares\n    `security: [{Bearer: [], OAuth2: []}]` with an empty scope array.\nscope_count: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basis/refs/heads/main/scopes/basis-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Programmatic Advertising
- DSP
- Media Buying
- Campaign Management
- Audience Targeting
- AdTech
token_urls: []
---
