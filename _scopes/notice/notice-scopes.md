---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Notice Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Notice uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Notice
provider_slug: notice
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: notice-scopes
source_filename: notice-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://api.stytch.notice.co/.well-known/oauth-authorization-server\nalso_source:\n  - https://api.stytch.notice.co/.well-known/openid-configuration\n  - https://api.notice.co/.well-known/oauth-protected-resource\nsummary: >-\n  Every scope below was read from a document Notice serves anonymously, not from a docs page - no\n  scope reference is published. Note the divergence between the three documents: the protected\n  resource (the MCP endpoint) advertises three scopes, the RFC 8414 authorization-server metadata\n  five, and the OIDC discovery document six. The union is recorded, with the source of each.\nauthorization_server: https://api.stytch.notice.co\nprotected_resource: https://api.notice.co/mcp\nscopes:\n  - name: openid\n    description: OpenID Connect authentication; issues an ID token.\n    declared_in: [protected-resource, authorization-server, openid-configuration]\n  - name: profile\n    description: Basic profile\
  \ claims for the authenticated Notice member.\n    declared_in: [protected-resource, authorization-server, openid-configuration]\n  - name: email\n    description: Email address claim for the authenticated Notice member.\n    declared_in: [protected-resource, authorization-server, openid-configuration]\n  - name: phone\n    description: Phone number claim.\n    declared_in: [authorization-server, openid-configuration]\n  - name: offline_access\n    description: Refresh-token issuance for long-lived agent/client sessions.\n    declared_in: [authorization-server, openid-configuration]\n  - name: full_access\n    description: >-\n      Declared only by the OIDC discovery document. No published definition of what it grants\n      against Notice data; not described on any Notice page.\n    declared_in: [openid-configuration]\nscope_count: 6\ndocs: null\ndivergence_note: >-\n  scopes_supported differs across the three discovery documents on the same auth plane. A client\n  reading only the protected-resource\
  \ metadata would never learn that offline_access or\n  full_access exist.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notice/refs/heads/main/scopes/notice-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Private Markets
- Market Data
- Financial Data
- Investing
- Pre-IPO
- Secondary Markets
- Valuations
- Fintech
- MCP
token_urls: []
---
