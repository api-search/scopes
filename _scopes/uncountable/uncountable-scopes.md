---
authorization_urls: []
description: ''
docs: https://www.support.uncountable.com/knowledge-base/uncountable-mcp-setup-guide/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Uncountable Scopes
name_suffix: OAuth Scopes
note: 'Scopes are read verbatim from the scopes_supported array of the live OAuth 2.0 / OpenID Connect discovery documents on both the US and EU application hosts (identical on both). Uncountable publishes no scope reference page, so the descriptions below are the plain reading of the scope names plus the one corroborating public signal: the /mcp endpoint''s WWW-Authenticate challenge names EXTERNAL_API_READ and EXTERNAL_API_WRITE as the scopes it requires. No per-endpoint scope mapping is published; that reference sits behind the application sign-in at /docs.'
overview: 'Uncountable uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Uncountable
provider_slug: uncountable
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: uncountable-scopes
source_filename: uncountable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://app.uncountable.com/.well-known/openid-configuration\ndocs: https://www.support.uncountable.com/knowledge-base/uncountable-mcp-setup-guide/\nnote: >-\n  Scopes are read verbatim from the scopes_supported array of the live OAuth 2.0 /\n  OpenID Connect discovery documents on both the US and EU application hosts (identical\n  on both). Uncountable publishes no scope reference page, so the descriptions below are\n  the plain reading of the scope names plus the one corroborating public signal: the\n  /mcp endpoint's WWW-Authenticate challenge names EXTERNAL_API_READ and\n  EXTERNAL_API_WRITE as the scopes it requires. No per-endpoint scope mapping is\n  published; that reference sits behind the application sign-in at /docs.\nauthorization_server: https://app.uncountable.com\nauthorization_endpoint: https://app.uncountable.com/oauth2/authorize\ntoken_endpoint: https://app.uncountable.com/oauth2/token\nflows:\n- authorization_code\n\
  - refresh_token\npkce: S256\nscope_count: 3\nscopes:\n- name: EXTERNAL_API_READ\n  description: Read access to the Uncountable External API and the hosted MCP server.\n  evidence: >-\n    scopes_supported in the discovery document; also named in the WWW-Authenticate\n    Bearer challenge returned by https://app.uncountable.com/mcp (HTTP 401).\n- name: EXTERNAL_API_WRITE\n  description: Write access to the Uncountable External API and the hosted MCP server.\n  evidence: >-\n    scopes_supported in the discovery document; also named in the WWW-Authenticate\n    Bearer challenge returned by https://app.uncountable.com/mcp (HTTP 401).\n- name: CAD\n  description: >-\n    CAD-related access. Uncountable publishes no description of this scope; it is\n    recorded here because it is declared by the authorization server.\n  evidence: scopes_supported in the discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncountable/refs/heads/main/scopes/uncountable-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Laboratory Informatics
- LIMS
- Electronic Lab Notebook
- R&D Data Management
- Product Lifecycle Management
- Quality Management
- Materials Science
- Chemicals
- Artificial Intelligence
- Model Context Protocol
token_urls: []
---
