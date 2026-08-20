---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Spotwise Inc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Spotwise, Inc. uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spotwise, Inc.
provider_slug: spotwise-inc
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: spotwise-inc-scopes
source_filename: spotwise-inc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://spotwise.ai/.well-known/oauth-authorization-server,\n  https://spotwise.ai/.well-known/oauth-protected-resource,\n  https://app.spotwise.ai/.well-known/oauth-authorization-server,\n  https://app.spotwise.ai/.well-known/oauth-protected-resource\ndocs: null\ndocs_note: >-\n  Spotwise publishes no scopes/permissions reference page. Every scope below was read\n  directly from a live RFC 8414 / RFC 9728 metadata document; descriptions are stated\n  as the standard meaning of the scope name, and the two mcp:content.* descriptions\n  are inferred from the resource_name (\"Spotwise CMS MCP\") of the resource that\n  declares them. No scope has been invented.\n\nauthorization_servers:\n- issuer: https://spotwise.ai/api/auth\n  resource: https://spotwise.ai/api/mcp\n  resource_name: Spotwise CMS MCP\n  scopes:\n  - name: openid\n    description: OpenID Connect authentication; issues an ID token\n    standard: OIDC Core\n\
  \  - name: profile\n    description: basic profile claims (name, given_name, family_name, picture)\n    standard: OIDC Core\n  - name: email\n    description: email and email_verified claims\n    standard: OIDC Core\n  - name: offline_access\n    description: permits issuance of a refresh token for long-lived agent sessions\n    standard: OIDC Core\n  - name: mcp:content.read\n    description: read access to the Spotwise site content collections exposed over the\n      CMS MCP server\n    product_scope: true\n  - name: mcp:content.write\n    description: write access to the Spotwise site content collections exposed over the\n      CMS MCP server\n    product_scope: true\n\n- issuer: https://app.spotwise.ai/api/auth\n  resource: https://app.spotwise.ai/api/mcp\n  resource_name: Spotwise Remote MCP\n  scopes:\n  - name: openid\n    description: OpenID Connect authentication; issues an ID token\n    standard: OIDC Core\n  - name: profile\n    description: basic profile claims\n    standard:\
  \ OIDC Core\n  - name: email\n    description: email and email_verified claims\n    standard: OIDC Core\n  - name: offline_access\n    description: permits issuance of a refresh token\n    standard: OIDC Core\n  note: >-\n    The product MCP server declares NO product-shaped scopes. Authorization to the\n    ad-detection, lead-list, contact-finder and CRM surface is therefore bound to the\n    authenticated user's workspace rather than expressed as delegatable OAuth scopes —\n    an agent cannot request least-privilege access to a subset of the product.\n\nsummary:\n  scope_count: 6\n  product_scopes: 2\n  identity_scopes: 4\n  least_privilege_available_on_product_server: false\n\nevidence:\n- url: https://spotwise.ai/.well-known/oauth-authorization-server\n  status: 200\n- url: https://app.spotwise.ai/.well-known/oauth-protected-resource\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotwise-inc/refs/heads/main/scopes/spotwise-inc-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Broadcast Media
- Advertising
- Media Monitoring
- Sales Intelligence
- Lead Generation
- Artificial Intelligence
- Radio
- MCP
- Agents
- Attribution
token_urls: []
---
