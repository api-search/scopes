---
authorization_urls:
- https://mcp.kotzilla.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Kotzilla Scopes
name_suffix: OAuth Scopes
note: Scopes were read live from the provider's own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata, not derived from an OpenAPI (Kotzilla publishes none). Kotzilla does NOT publish a scopes / permissions reference page in its documentation; the metadata documents are the only published scope surface, so descriptions below state the standard meaning of each scope rather than a provider-authored one, and are marked accordingly.
overview: 'Kotzilla publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kotzilla API on a user''s behalf.


  Tokens are issued from https://mcp.kotzilla.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kotzilla
provider_slug: kotzilla
schemes:
- flows:
  - authorizationUrl: https://mcp.kotzilla.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.kotzilla.io/oauth/token
  name: KotzillaMCPOAuth
  resource: https://mcp.kotzilla.io
  source: well-known/kotzilla-oauth-authorization-server.json
scope_count: 3
scope_names:
- openid
- email
- offline_access
scopes:
- description: Standard OpenID Connect scope requesting the subject identifier of the authenticated Kotzilla account. Description is the standard meaning; Kotzilla publishes no scope reference page.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OpenID Connect scope requesting the email address of the authenticated Kotzilla account. Description is the standard meaning; Kotzilla publishes no scope reference page.
  flows:
  - authorizationCode
  scope: email
- description: Standard OAuth/OIDC scope requesting a refresh token so an agent session survives access-token expiry. Description is the standard meaning; Kotzilla publishes no scope reference page.
  flows:
  - authorizationCode
  scope: offline_access
slug: kotzilla-scopes
source_filename: kotzilla-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://mcp.kotzilla.io/.well-known/oauth-authorization-server\nnote: >-\n  Scopes were read live from the provider's own RFC 8414 authorization-server\n  metadata and RFC 9728 protected-resource metadata, not derived from an\n  OpenAPI (Kotzilla publishes none). Kotzilla does NOT publish a scopes /\n  permissions reference page in its documentation; the metadata documents are\n  the only published scope surface, so descriptions below state the standard\n  meaning of each scope rather than a provider-authored one, and are marked\n  accordingly.\n\nschemes:\n  - name: KotzillaMCPOAuth\n    source: well-known/kotzilla-oauth-authorization-server.json\n    resource: https://mcp.kotzilla.io\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.kotzilla.io/oauth/authorize\n        tokenUrl: https://mcp.kotzilla.io/oauth/token\n\nscopes:\n  - scope: openid\n    description: >-\n      Standard OpenID Connect\
  \ scope requesting the subject identifier of the\n      authenticated Kotzilla account. Description is the standard meaning;\n      Kotzilla publishes no scope reference page.\n    description_source: standard\n    flows: [authorizationCode]\n    advertised_by: [authorization-server-metadata, protected-resource-metadata]\n    sources: [well-known/kotzilla-oauth-authorization-server.json]\n  - scope: email\n    description: >-\n      Standard OpenID Connect scope requesting the email address of the\n      authenticated Kotzilla account. Description is the standard meaning;\n      Kotzilla publishes no scope reference page.\n    description_source: standard\n    flows: [authorizationCode]\n    advertised_by: [authorization-server-metadata, protected-resource-metadata]\n    sources: [well-known/kotzilla-oauth-authorization-server.json]\n  - scope: offline_access\n    description: >-\n      Standard OAuth/OIDC scope requesting a refresh token so an agent session\n      survives access-token\
  \ expiry. Description is the standard meaning;\n      Kotzilla publishes no scope reference page.\n    description_source: standard\n    flows: [authorizationCode]\n    advertised_by: [authorization-server-metadata]\n    sources: [well-known/kotzilla-oauth-authorization-server.json]\n\nobservations:\n  - >-\n    The scope set is IDENTITY-ONLY. None of the fifteen MCP tools —\n    including the three that mutate state (create_app,\n    set_app_versions_enabled, koin_apply_fix) — is gated by a distinct scope.\n    Authorization is therefore all-or-nothing at the account level: any token\n    that can read issues can also register apps, toggle data ingestion, and\n    apply Koin fixes to source. There is no least-privilege token available to\n    an agent operator.\n  - >-\n    The protected-resource metadata advertises only [openid, email] while the\n    authorization-server metadata advertises [openid, email, offline_access] —\n    a minor inconsistency between the two documents.\n\nsummary:\n\
  \  scope_count: 3\n  resource_scopes: 0\n  identity_scopes: 3\n  granular_authorization: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotzilla/refs/heads/main/scopes/kotzilla-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Ai Data
- Observability
- Monitoring
- Developer Tools
- Kotlin
- Android
- Mobile
- Dependency Injection
- Performance
- MCP
- Agents
token_urls:
- https://mcp.kotzilla.io/oauth/token
---
