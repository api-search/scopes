---
authorization_urls:
- https://example.com/oauth/authorize
description: ''
docs: https://prestodb.io/docs/current/security/oauth2.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Presto Foundation Scopes
name_suffix: OAuth Scopes
note: Presto does not publish its own OAuth scopes; OAuth 2.0 is an optional coordinator authenticator using OIDC where scopes (e.g. openid, email, profile) are configured per deployment via http-server.authentication.oauth2.scopes for the external identity provider (https://prestodb.io/docs/current/security/oauth2.html).
overview: 'Presto Foundation uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Presto Foundation
provider_slug: presto-foundation
schemes:
- description: OAuth 2.0 authenticator (when enabled on the coordinator).
  flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/oauth/token
  name: oauth2
  source: openapi/presto-foundation-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: presto-foundation-scopes
source_filename: presto-foundation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/presto-foundation-openapi.yml\ndocs: https://prestodb.io/docs/current/security/oauth2.html\nnote: Presto does not publish its own OAuth scopes; OAuth 2.0 is an optional coordinator\n  authenticator using OIDC where scopes (e.g. openid, email, profile) are configured\n  per deployment via http-server.authentication.oauth2.scopes for the external identity\n  provider (https://prestodb.io/docs/current/security/oauth2.html).\nschemes:\n- name: oauth2\n  source: openapi/presto-foundation-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n  description: OAuth 2.0 authenticator (when enabled on the coordinator).\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/scopes/presto-foundation-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Big Data
- Distributed SQL
- Linux Foundation
- Open Source
- Query Engine
- SQL
token_urls:
- https://example.com/oauth/token
---
