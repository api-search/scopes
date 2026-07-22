---
authorization_urls:
- https://cloud.polarsignals.com/login/cli
description: ''
docs: https://www.polarsignals.com/docs/single-sign-on
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Polar Signals Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Polar Signals publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Polar Signals API on a user''s behalf.


  Tokens are issued from https://identity.polarsignals.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Polar Signals
provider_slug: polar-signals
schemes:
- flows:
  - authorizationUrl: https://cloud.polarsignals.com/login/cli
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://identity.polarsignals.com/token
  name: OAuth2
  source: well-known/polar-signals-oauth-authorization-server.json
scope_count: 5
scope_names:
- openid
- email
- profile
- groups
- offline_access
scopes:
- description: Standard OpenID Connect scope; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Access the user's basic profile information.
  flows:
  - authorizationCode
  scope: profile
- description: Access the user's group memberships (used for SSO role mapping).
  flows:
  - authorizationCode
  scope: groups
- description: Issue a refresh token for long-lived offline access.
  flows:
  - authorizationCode
  scope: offline_access
slug: polar-signals-scopes
source_filename: polar-signals-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: well-known/polar-signals-oauth-authorization-server.json\ndocs: https://www.polarsignals.com/docs/single-sign-on\ncontext: >-\n  These are OIDC login scopes advertised by the Polar Signals OAuth 2.0\n  Authorization Server (RFC 8414) at issuer https://identity.polarsignals.com,\n  used for interactive CLI / dashboard sign-in (authorization-code + PKCE).\n  API-level authorization for the gRPC/Connect API is RBAC (roles/permissions),\n  not OAuth scopes; automation uses service-account bearer tokens.\nschemes:\n- name: OAuth2\n  source: well-known/polar-signals-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud.polarsignals.com/login/cli\n    tokenUrl: https://identity.polarsignals.com/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; issue an ID token.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the\
  \ user's email address.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the user's basic profile information.\n  flows: [authorizationCode]\n- scope: groups\n  description: Access the user's group memberships (used for SSO role mapping).\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token for long-lived offline access.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar-signals/refs/heads/main/scopes/polar-signals-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Enterprise
- Observability
- Continuous Profiling
- Performance
- eBPF
- gRPC
- Developer Tools
- MCP
- GPU
token_urls:
- https://identity.polarsignals.com/token
---
