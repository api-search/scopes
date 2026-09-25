---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Virtual Incision Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from the RFC 8414 authorization-server metadata the host serves. They govern the MCP endpoint only; the wp/v2 REST surface uses WordPress Application Passwords / cookie+nonce and has no scope model.
overview: 'Virtual Incision uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Virtual Incision
provider_slug: virtual-incision
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: virtual-incision-scopes
source_filename: virtual-incision-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://virtualincision.com/.well-known/oauth-authorization-server\nnote: Scopes are read verbatim from the RFC 8414 authorization-server metadata the host serves. They govern the\n  MCP endpoint only; the wp/v2 REST surface uses WordPress Application Passwords / cookie+nonce and has no scope\n  model.\nflows:\n  authorization_code:\n    authorization_endpoint: https://virtualincision.com/oauth/authorize\n    token_endpoint: https://virtualincision.com/oauth/token\n    revocation_endpoint: https://virtualincision.com/oauth/revoke\n    pkce:\n    - S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n    token_endpoint_auth_methods:\n    - none\n    client_id_metadata_document_supported: true\nscopes:\n- name: mcp\n  description: The single scope advertised in scopes_supported. Grants a client access to the Model Context Protocol\n    endpoint at /wp-json/mcp/mcp-oauth-server. The provider publishes no scope\
  \ reference page, so no finer-grained\n    meaning is asserted here.\n  source: https://virtualincision.com/.well-known/oauth-authorization-server\nscope_count: 1\ndocs: null\ndocs_note: No scopes/permissions reference page is published; the discovery document is the only source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-incision/refs/heads/main/scopes/virtual-incision-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Medical Devices
- Surgical Robotics
- Robotics
- Healthcare
- Health
- Life Sciences
- Medical Technology
- Content
- News
- Careers
- Event
- MCP
token_urls: []
---
