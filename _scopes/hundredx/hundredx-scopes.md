---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hundredx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HundredX uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HundredX
provider_slug: hundredx
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hundredx-scopes
source_filename: hundredx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  https://login.hundredxinc.com/.well-known/openid-configuration,\n  https://hx-bigquery-mcp.hundredx.com/.well-known/oauth-protected-resource,\n  https://jupyter-mcp.hundredx.com/.well-known/oauth-protected-resource (fetched 2026-08-22).\ndocs: null\ndocs_note: >-\n  HundredX publishes no scopes/permissions reference page. Every scope below was read from a\n  live discovery document, and descriptions are the standard meaning of the registered scope —\n  no HundredX-specific description exists to quote.\nsurfaces:\n  - id: hundredx-portal-oidc\n    issuer: https://login.hundredxinc.com/\n    scopes:\n      - name: openid\n        description: OIDC — request an ID token.\n      - name: profile\n        description: OIDC — basic profile claims.\n      - name: offline_access\n        description: OIDC — issue a refresh token.\n      - name: name\n      - name: given_name\n      - name: family_name\n      - name: nickname\n \
  \     - name: email\n      - name: email_verified\n      - name: picture\n      - name: created_at\n      - name: identities\n      - name: phone\n      - name: address\n  - id: hx-bigquery-mcp\n    issuer: https://hx-bigquery-mcp.hundredx.com\n    scopes:\n      - name: openid\n      - name: email\n      - name: profile\n      - name: bigquery.readonly\n        description: Google Cloud BigQuery read-only — the MCP server reads HundredX's warehouse on the caller's behalf.\n      - name: cloud-platform.read-only\n        description: Google Cloud read-only platform access.\n  - id: jupyter-mcp\n    issuer: https://jupyter-mcp.hundredx.com\n    scopes:\n      - name: openid\n      - name: email\n      - name: profile\n      - name: cloud-platform\n        description: Google Cloud platform access (read/write) for notebook execution.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hundredx/refs/heads/main/scopes/hundredx-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- customer-experience
- consumer-insights
- market-research
- alternative-data
- investment-research
- data-licensing
token_urls: []
---
