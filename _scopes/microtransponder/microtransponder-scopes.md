---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Microtransponder Scopes
name_suffix: OAuth Scopes
note: The full published scope surface. RFC 8414 metadata served by www.mobia.com declares exactly one scope. There is no scope reference page — the provider has no developer documentation — so this is the complete, verbatim set and nothing was inferred.
overview: 'MicroTransponder uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MicroTransponder
provider_slug: microtransponder
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: microtransponder-scopes
source_filename: microtransponder-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.mobia.com/.well-known/oauth-authorization-server\nnote: >-\n  The full published scope surface. RFC 8414 metadata served by www.mobia.com declares\n  exactly one scope. There is no scope reference page — the provider has no developer\n  documentation — so this is the complete, verbatim set and nothing was inferred.\nauthorization_server: https://www.mobia.com\nprotected_resource: https://www.mobia.com/wp-json/mcp/mcp-oauth-server\nflows:\n- type: authorization_code\n  authorization_url: https://www.mobia.com/oauth/authorize\n  token_url: https://www.mobia.com/oauth/token\n  pkce: S256\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The single scope declared in both the authorization-server metadata\n    (scopes_supported) and the protected-resource metadata. Grants an OAuth client access\n    to the site's Model Context Protocol endpoint. No finer-grained scopes are published.\n  source: /.well-known/oauth-authorization-server\n\
  docs: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microtransponder/refs/heads/main/scopes/microtransponder-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Medical Devices
- Health Care
- Neurotechnology
- Neuromodulation
- Stroke Rehabilitation
- Implantable Devices
- Life Sciences
- WordPress
- Model Context Protocol
token_urls: []
---
