---
authorization_urls:
- https://harbinger-health.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Harbinger Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Harbinger Health publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Harbinger Health API on a user''s behalf.


  Tokens are issued from https://harbinger-health.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Harbinger Health
provider_slug: harbinger-health
schemes:
- flows:
  - authorizationUrl: https://harbinger-health.com/oauth/authorize
    client_id_metadata_document_supported: true
    flow: authorizationCode
    pkce:
    - S256
    refresh_token: true
    revocationUrl: https://harbinger-health.com/oauth/revoke
    tokenUrl: https://harbinger-health.com/oauth/token
    token_endpoint_auth_methods_supported:
    - none
  issuer: https://harbinger-health.com
  name: mcp-oauth
  source: https://harbinger-health.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: The only scope the authorization server advertises. Declared in scopes_supported on both the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata, where it guards https://harbinger-health.com/wp-json/mcp/mcp-oauth-server. No further description, granularity or read/write split is published by the provider.
  flows:
  - authorizationCode
  scope: mcp
slug: harbinger-health-scopes
source_filename: harbinger-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://harbinger-health.com/.well-known/oauth-authorization-server\nalso_from: https://harbinger-health.com/.well-known/oauth-protected-resource\ndocs: null\nsummary: >-\n  Harbinger Health runs a real OAuth 2.1 authorization server on its own origin, published as RFC\n  8414 metadata, guarding the Model Context Protocol server registered on the site. It declares\n  exactly one scope. The scope list below is copied verbatim from the live metadata documents —\n  the provider publishes no scopes or permissions reference page, so nothing here is expanded,\n  grouped or inferred beyond the single published value.\nschemes:\n  - name: mcp-oauth\n    type: oauth2\n    source: https://harbinger-health.com/.well-known/oauth-authorization-server\n    issuer: https://harbinger-health.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://harbinger-health.com/oauth/authorize\n        tokenUrl: https://harbinger-health.com/oauth/token\n\
  \        revocationUrl: https://harbinger-health.com/oauth/revoke\n        pkce: [S256]\n        refresh_token: true\n        token_endpoint_auth_methods_supported: [none]\n        client_id_metadata_document_supported: true\nscopes:\n  - scope: mcp\n    description: >-\n      The only scope the authorization server advertises. Declared in scopes_supported on both the\n      RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata, where it\n      guards https://harbinger-health.com/wp-json/mcp/mcp-oauth-server. No further description,\n      granularity or read/write split is published by the provider.\n    flows: [authorizationCode]\n    protects: https://harbinger-health.com/wp-json/mcp/mcp-oauth-server\n    sources:\n      - https://harbinger-health.com/.well-known/oauth-authorization-server\n      - https://harbinger-health.com/.well-known/oauth-protected-resource\ngaps:\n  - No OpenID Connect discovery document is served (/.well-known/openid-configuration\
  \ is 404), so\n    this is a bare OAuth 2.1 deployment with no identity layer advertised.\n  - Only one coarse scope exists; there is no read/write or per-resource separation, so a token\n    that can list tools can also, in principle, invoke any write-capable ability the server exposes.\n  - No dynamic client registration endpoint is advertised; registration is by client-ID metadata\n    document instead.\n  - The provider publishes no scopes reference page, no OAuth documentation and no developer portal.\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n    - {url: 'https://harbinger-health.com/.well-known/oauth-authorization-server', http_status: 200, content_type: application/json}\n    - {url: 'https://harbinger-health.com/.well-known/oauth-protected-resource', http_status: 200, content_type: application/json}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbinger-health/refs/heads/main/scopes/harbinger-health-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Health
- Healthcare
- Biotechnology
- Cancer Detection
- Diagnostics
- Genomics
- Artificial Intelligence
- Machine Learning
- Life Sciences
- Clinical Laboratory
- Precision Medicine
- United States
- Company
token_urls:
- https://harbinger-health.com/oauth/token
---
