---
authorization_urls: []
description: The complete scope surface advertised by the OAuth 2.1 authorization server on tunetx.com. Read verbatim from `scopes_supported` in the RFC 8414 metadata document and cross-checked against `scopes_supported` in the RFC 9728 protected-resource document. Both name exactly one scope. Tune Therapeutics publishes no scopes or permissions reference page, so there is nothing to enrich these descriptions from — the meaning below is stated as observed, not as documented.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Tune Therapeutics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tune Therapeutics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tune Therapeutics
provider_slug: tune-therapeutics
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tune-therapeutics-scopes
source_filename: tune-therapeutics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://tunetx.com/.well-known/oauth-authorization-server/\nname: Tune Therapeutics — OAuth scopes\ndescription: >-\n  The complete scope surface advertised by the OAuth 2.1 authorization server on\n  tunetx.com. Read verbatim from `scopes_supported` in the RFC 8414 metadata document and\n  cross-checked against `scopes_supported` in the RFC 9728 protected-resource document.\n  Both name exactly one scope. Tune Therapeutics publishes no scopes or permissions\n  reference page, so there is nothing to enrich these descriptions from — the meaning\n  below is stated as observed, not as documented.\n\ndocs: null\ndocs_note: No scopes or permissions reference page is published on tunetx.com.\n\nauthorization_server: https://tunetx.com\nauthorization_endpoint: https://tunetx.com/oauth/authorize\ntoken_endpoint: https://tunetx.com/oauth/token\nrevocation_endpoint: https://tunetx.com/oauth/revoke\n\nscopes:\n- name: mcp\n  description:\
  \ >-\n    Access to the site's Model Context Protocol server at\n    https://tunetx.com/wp-json/mcp/mcp-oauth-server. The authorization server advertises no\n    finer-grained scopes, so this single scope is the whole consent surface — a client\n    either has MCP access or it does not. What that access actually permits depends on the\n    WordPress abilities registered on the site, which is itself auth-gated (HTTP 401) and\n    was not enumerated.\n  source: >-\n    scopes_supported in both /.well-known/oauth-authorization-server/ and\n    /.well-known/oauth-protected-resource\n  granularity: coarse\n\nobservations:\n- >-\n  One scope for an entire MCP server is a coarse consent boundary. There is no read-vs-write\n  split, no per-ability scope, and no way for a user granting consent to see what the token\n  will be able to do.\n- >-\n  Because token_endpoint_auth_methods_supported is [\"none\"] and dynamic client identification\n  via client_id metadata documents is enabled, any public\
  \ client that completes the PKCE\n  flow with a site user can obtain this scope.\n\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://tunetx.com/.well-known/oauth-authorization-server/\n    status: 200\n    field: scopes_supported\n    value: ['mcp']\n  - url: https://tunetx.com/.well-known/oauth-protected-resource\n    status: 200\n    field: scopes_supported\n    value: ['mcp']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tune-therapeutics/refs/heads/main/scopes/tune-therapeutics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Biotechnology
- Life Sciences
- Therapeutics
- Genomics
- Epigenetics
- Gene Therapy
- Clinical Stage
- Research
token_urls: []
---
