---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Aidentified Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aidentified uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aidentified
provider_slug: aidentified
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: aidentified-scopes
source_filename: aidentified-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: >-\n  https://login.aidentified.com/.well-known/oauth-authorization-server (HTTP 200) and\n  https://login.aidentified.com/.well-known/openid-configuration (HTTP 200), both fetched\n  2026-09-14 and saved verbatim under well-known/.\ndocs: null\ndocs_note: >-\n  Aidentified publishes NO scopes or permissions reference page. These scopes were read from the\n  provider's own live OAuth discovery documents, which is the authoritative machine-readable\n  source, but a human integrator has nothing to read.\napplies_to:\n  resource: https://mcp.aidentified.com/mcp\n  authorization_server: https://login.aidentified.com\n  flows:\n    - authorization_code\n  pkce: S256\n\nscopes:\n  - name: openid\n    description: Request an OpenID Connect ID token carrying the subject identifier.\n    source: both\n  - name: profile\n    description: Basic profile claims for the authenticated Aidentified user.\n    source: both\n  - name: email\n \
  \   description: Email address claim for the authenticated Aidentified user.\n    source: both\n  - name: phone\n    description: Phone number claim for the authenticated Aidentified user.\n    source: both\n  - name: offline_access\n    description: Issue a refresh token so an agent can act without re-prompting the user.\n    source: both\n  - name: full_access\n    description: >-\n      Full access. Advertised by the OpenID Connect discovery document only; absent from the RFC 8414\n      authorization-server metadata. No published document defines what it grants.\n    source: openid-configuration\n\nscope_count: 6\n\nfindings:\n  - >-\n    The RFC 9728 protected-resource document for the MCP server declares scopes_supported as an EMPTY\n    array, while the authorization server advertises six. An agent reading the resource metadata — the\n    document the 401 challenge points it at — learns nothing about what to request.\n  - >-\n    Every scope except full_access is a standard OIDC\
  \ identity scope. There is no API-capability scope\n    (no read/write, no per-resource scope), so the token model is all-or-nothing with respect to\n    Aidentified data.\n  - >-\n    full_access appears in only one of the two discovery documents and is undefined in prose anywhere.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidentified/refs/heads/main/scopes/aidentified-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Data Enrichment
- Wealth Management
- Financial Services
- Relationship Intelligence
- Sales Intelligence
- Prospecting
- Contact Data
- Identity Resolution
- MCP
token_urls: []
---
