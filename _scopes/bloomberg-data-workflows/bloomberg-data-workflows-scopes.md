---
authorization_urls: []
description: The only OAuth scope surface Bloomberg publishes anonymously is the bloomberg.com identity provider's discovery document. Scopes were read verbatim from `scopes_supported`; no scope descriptions are published, so the descriptions below state only what the scope name and the surrounding discovery metadata establish, and are marked as such. The Data License REST API (api.bloomberg.com/eap) uses per-request signed JWTs rather than OAuth scopes and therefore contributes no scopes; BLPAPI/SAPI uses Terminal entitlements, not scopes.
docs: https://www.bloomberg.com/.well-known/oauth-authorization-server
flows:
- authorization_code
- refresh_token
kind: oauth-scopes
layout: scope
method: probed
name: Bloomberg Data Workflows Scopes
name_suffix: OAuth Scopes
note: No public scopes/permissions reference page exists for any Bloomberg API. This artifact is probed from the live discovery document, not searched from documentation.
overview: 'Bloomberg Data Workflows uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloomberg Data Workflows
provider_slug: bloomberg-data-workflows
schemes:
- authorization_url: https://login.bloomberg.com/api/oauth/authorize
  flows:
  - authorization_code
  - refresh_token
  issuer: https://www.bloomberg.com
  name: bloomberg-com-oidc
  pkce_required_methods:
  - S256
  source: https://www.bloomberg.com/.well-known/openid-configuration
  token_url: https://login.bloomberg.com/api/oauth/token
  type: openIdConnect
scope_count: 0
scope_names: []
scopes: []
slug: bloomberg-data-workflows-scopes
source_filename: bloomberg-data-workflows-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://www.bloomberg.com/.well-known/openid-configuration\ndocs: https://www.bloomberg.com/.well-known/oauth-authorization-server\ndescription: >-\n  The only OAuth scope surface Bloomberg publishes anonymously is the bloomberg.com identity\n  provider's discovery document. Scopes were read verbatim from `scopes_supported`; no scope\n  descriptions are published, so the descriptions below state only what the scope name and the\n  surrounding discovery metadata establish, and are marked as such. The Data License REST API\n  (api.bloomberg.com/eap) uses per-request signed JWTs rather than OAuth scopes and therefore\n  contributes no scopes; BLPAPI/SAPI uses Terminal entitlements, not scopes.\nschemes:\n  - name: bloomberg-com-oidc\n    type: openIdConnect\n    source: https://www.bloomberg.com/.well-known/openid-configuration\n    issuer: https://www.bloomberg.com\n    authorization_url: https://login.bloomberg.com/api/oauth/authorize\n\
  \    token_url: https://login.bloomberg.com/api/oauth/token\n    flows: [authorization_code, refresh_token]\n    pkce_required_methods: [S256]\nscopes:\n  - name: openid\n    scheme: bloomberg-com-oidc\n    description: >-\n      Standard OpenID Connect scope; requests an ID token for the authenticated Bloomberg account.\n    description_source: OIDC Core 1.0 (the provider publishes no scope description)\n  - name: user\n    scheme: bloomberg-com-oidc\n    description: >-\n      Access to the authenticated user's Bloomberg.com profile. Bloomberg publishes no description\n      or claim list for this scope.\n    description_source: inferred-from-name\n  - name: entitlements\n    scheme: bloomberg-com-oidc\n    description: >-\n      Access to the authenticated user's Bloomberg subscription entitlements. Bloomberg publishes\n      no description or claim list for this scope.\n    description_source: inferred-from-name\nscope_count: 3\nnote: >-\n  No public scopes/permissions reference page\
  \ exists for any Bloomberg API. This artifact is\n  probed from the live discovery document, not searched from documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-data-workflows/refs/heads/main/scopes/bloomberg-data-workflows-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Enterprise Data
- Financial Analytics
- Financial-Services
- Investment Management
- Market Data
- Reference Data
- Trading
token_urls: []
---
