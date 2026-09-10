---
authorization_urls: []
description: ''
docs: https://motomarks.io/docs/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Motomarks Scopes
name_suffix: OAuth Scopes
note: Scopes read from the live RFC 8414 authorization-server metadata (HTTP 200, 2026-09-09), which backs the MCP OAuth 2.1 flow. These are identity-shaped scopes only; API capability is governed by the account's plan and key type rather than granular OAuth scopes, and the docs publish no additional scope reference.
overview: 'Motomarks uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Motomarks
provider_slug: motomarks
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: motomarks-scopes
source_filename: motomarks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Motomarks OAuth Scopes\ngenerated: '2026-09-09'\nmethod: probed\nsource: https://motomarks.io/.well-known/oauth-authorization-server\ndocs: https://motomarks.io/docs/mcp\nnote: >-\n  Scopes read from the live RFC 8414 authorization-server metadata (HTTP 200, 2026-09-09), which backs the MCP\n  OAuth 2.1 flow. These are identity-shaped scopes only; API capability is governed by the account's plan and\n  key type rather than granular OAuth scopes, and the docs publish no additional scope reference.\nscopes:\n  - id: openid\n    description: OpenID Connect authentication of the Motomarks account.\n  - id: profile\n    description: Basic profile information for the signed-in user.\n  - id: email\n    description: Email address of the signed-in user.\n  - id: offline_access\n    description: Refresh-token issuance so MCP clients stay connected without re-authorizing.\ngrants_supported:\n  - authorization_code\n  - refresh_token\npkce: S256\ndynamic_client_registration: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motomarks/refs/heads/main/scopes/motomarks-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- automotive
- logo
- image-cdn
- manufacturer
- brand-assets
- images
- CDN
- developer-tools
- agent-native
- MCP
- reference-data
token_urls: []
---
