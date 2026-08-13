---
authorization_urls:
- https://auth.jampp.com/v1/oauth/authorize
description: ''
docs: https://developers.jampp.com/docs/reporting-api/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Jampp Scopes
name_suffix: OAuth Scopes
note: 'Jampp runs OAuth 2.0 but publishes no scope vocabulary. The authorization-server metadata at auth.jampp.com omits scopes_supported entirely, and both protected-resource metadata documents advertise a single scope value of "." — a wildcard placeholder, not a named permission. The developer documentation never mentions a scope parameter: the client-credentials request carries only grant_type, client_id and client_secret, and authorization is bound to the user account that issued the credential pair rather than to a requested scope. Recorded as an honest zero-scope surface; nothing was inferred.'
overview: 'Jampp publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jampp API on a user''s behalf.


  Tokens are issued from https://auth.jampp.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jampp
provider_slug: jampp
schemes:
- flows:
  - flow: clientCredentials
    scopes: {}
    tokenUrl: https://auth.jampp.com/v1/oauth/token
  - authorizationUrl: https://auth.jampp.com/v1/oauth/authorize
    flow: authorizationCode
    note: Advertised in RFC 8414 metadata only; not documented for developers.
    scopes: {}
    tokenUrl: https://auth.jampp.com/v1/oauth/token
  name: OAuth2ClientCredentials
  token_url: https://auth.jampp.com/v1/oauth/token
scope_count: 1
scope_names:
- .
scopes:
- description: The only value advertised in scopes_supported by the RFC 9728 protected-resource metadata for both https://api.jampp.com and https://auth.jampp.com. A placeholder wildcard, not a documented permission; no scope-to-capability mapping is published.
  flows: []
  scope: .
slug: jampp-scopes
source_filename: jampp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://auth.jampp.com/.well-known/oauth-protected-resource\ndocs: https://developers.jampp.com/docs/reporting-api/\nnote: >-\n  Jampp runs OAuth 2.0 but publishes no scope vocabulary. The authorization-server\n  metadata at auth.jampp.com omits scopes_supported entirely, and both protected-resource\n  metadata documents advertise a single scope value of \".\" — a wildcard placeholder, not a\n  named permission. The developer documentation never mentions a scope parameter: the\n  client-credentials request carries only grant_type, client_id and client_secret, and\n  authorization is bound to the user account that issued the credential pair rather than to\n  a requested scope. Recorded as an honest zero-scope surface; nothing was inferred.\nschemes:\n- name: OAuth2ClientCredentials\n  token_url: https://auth.jampp.com/v1/oauth/token\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.jampp.com/v1/oauth/token\n \
  \   scopes: {}\n  - flow: authorizationCode\n    authorizationUrl: https://auth.jampp.com/v1/oauth/authorize\n    tokenUrl: https://auth.jampp.com/v1/oauth/token\n    scopes: {}\n    note: Advertised in RFC 8414 metadata only; not documented for developers.\nscopes:\n- scope: '.'\n  description: >-\n    The only value advertised in scopes_supported by the RFC 9728 protected-resource\n    metadata for both https://api.jampp.com and https://auth.jampp.com. A placeholder\n    wildcard, not a documented permission; no scope-to-capability mapping is published.\n  flows: []\n  sources:\n  - https://api.jampp.com/.well-known/oauth-protected-resource\n  - https://auth.jampp.com/.well-known/oauth-protected-resource\nscope_count: 0\nauthorization_model: >-\n  Data visibility follows the dashboard user that minted the credential — a token can read\n  the reporting data of the advertiser accounts that user can see. Jampp exposes no\n  per-scope narrowing; the documented isolation mechanism is issuing\
  \ one credential pair\n  per integrating service so it can be revoked independently.\nx-evidence:\n  fetched: '2026-08-12'\n  urls:\n  - url: https://auth.jampp.com/.well-known/oauth-authorization-server\n    status: 200\n    scopes_supported: absent\n  - url: https://api.jampp.com/.well-known/oauth-protected-resource\n    status: 200\n    scopes_supported: ['.']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jampp/refs/heads/main/scopes/jampp-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags:
- Company
- Advertising
- Marketing
- Mobile
- Analytics
- Reporting
- GraphQL
- Demand-Side Platform
- App Marketing
- Attribution
token_urls:
- https://auth.jampp.com/v1/oauth/token
---
