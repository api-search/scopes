---
authorization_urls: []
description: The complete published scope surface for GigaIO, read verbatim from the RFC 8414 authorization-server metadata document and corroborated by the RFC 9728 protected-resource document. One scope exists. GigaIO publishes no scopes or permissions reference page; this is the whole of it.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Gigaio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GigaIO uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GigaIO
provider_slug: gigaio
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: gigaio-scopes
source_filename: gigaio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: probed\nsource: https://gigaio.com/.well-known/oauth-authorization-server\ndescription: >-\n  The complete published scope surface for GigaIO, read verbatim from the RFC 8414\n  authorization-server metadata document and corroborated by the RFC 9728\n  protected-resource document. One scope exists. GigaIO publishes no scopes or\n  permissions reference page; this is the whole of it.\nauthorization_server: https://gigaio.com\nprotected_resource: https://gigaio.com/wp-json/mcp/mcp-oauth-server\ndocs: null\ndocs_note: No public scopes/permissions reference page is published.\nscope_count: 1\nscopes:\n  - name: mcp\n    description: >-\n      Access the GigaIO Model Context Protocol server. Declared in\n      scopes_supported of both the authorization-server and protected-resource\n      metadata documents. The provider publishes no finer-grained read/write split.\n    source: https://gigaio.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigaio/refs/heads/main/scopes/gigaio-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Composable Infrastructure
- Edge Computing
- Artificial Intelligence
- High Performance Computing
- Data Center
- Hardware
- GPU
- PCIe
- Infrastructure as Code
token_urls: []
---
