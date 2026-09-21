---
api_specs:
- filename: patronus-protect-openapi.json
  format: json
  label: Patronus Scan API
  slug: patronus-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patronus-protect/refs/heads/main/openapi/patronus-protect-openapi.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Patronus Protect Scopes
name_suffix: OAuth Scopes
note: Both scopes are declared in scopes_supported of the authorization-server and protected-resource metadata. Descriptions are inferred from the scope names and the Scan API surface; the provider does not publish a reachable scope-reference page, so they are not verbatim.
overview: 'Patronus Protect uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Patronus Protect
provider_slug: patronus-protect
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: patronus-protect-scopes
source_filename: patronus-protect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: >-\n  Live RFC 8414 OAuth authorization-server metadata and RFC 9728 protected-resource metadata at\n  control.patronus.studio/.well-known/ (saved verbatim under well-known/). No separate human scopes\n  reference page was reachable (docs host is Cloudflare JS-challenged).\noauth2:\n  authorization_server: https://control.patronus.studio\n  resource: https://control.patronus.studio/api\n  flow: authorizationCode\n  pkce: S256\nscopes:\n- name: scan:read\n  description: Read access to scan results / receipts on the Patronus control plane (MCP).\n- name: scan:write\n  description: Submit scans (text, URL, MCP-server audits) on the Patronus control plane (MCP).\nnote: >-\n  Both scopes are declared in scopes_supported of the authorization-server and protected-resource\n  metadata. Descriptions are inferred from the scope names and the Scan API surface; the provider\n  does not publish a reachable scope-reference page, so they are\
  \ not verbatim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patronus-protect/refs/heads/main/scopes/patronus-protect-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI Safety
- Prompt Injection
- Security
- LLM
- agent-native
- MCP
- DLP
- PII
- On-Device
- AI Firewall
token_urls: []
---
