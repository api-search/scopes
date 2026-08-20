---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Mailoptin Scopes
name_suffix: OAuth Scopes
note: Not derived from an OpenAPI — derive-oauth-scopes.py found no oauth2 securitySchemes because MailOptin publishes no OpenAPI. The single scope below is read verbatim from the RFC 8414 authorization-server metadata document mailoptin.io serves, and confirmed against the RFC 9728 protected-resource document. MailOptin publishes no human-readable scopes/permissions reference page, so there is no `docs:` URL to record.
overview: 'MailOptin uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MailOptin
provider_slug: mailoptin
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: mailoptin-scopes
source_filename: mailoptin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://mailoptin.io/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Not derived from an OpenAPI — derive-oauth-scopes.py found no oauth2 securitySchemes\n  because MailOptin publishes no OpenAPI. The single scope below is read verbatim from\n  the RFC 8414 authorization-server metadata document mailoptin.io serves, and confirmed\n  against the RFC 9728 protected-resource document. MailOptin publishes no human-readable\n  scopes/permissions reference page, so there is no `docs:` URL to record.\nauthorization_server: https://mailoptin.io\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Access to the MailOptin site's Model Context Protocol server at\n    https://mailoptin.io/wp-json/mcp/mcp-oauth-server. This is the only scope the\n    authorization server advertises; it is coarse-grained — a single scope covering the\n    whole MCP surface, with no read/write split and no per-ability scoping.\n  source:\
  \ scopes_supported\n  advertised_by:\n  - https://mailoptin.io/.well-known/oauth-authorization-server\n  - https://mailoptin.io/.well-known/oauth-protected-resource\nobservations:\n- >-\n  Granularity is minimal. Consent to `mcp` is consent to every tool the WordPress\n  Abilities API registers, whatever that set turns out to be — the list is auth-gated and\n  could not be enumerated anonymously.\n- >-\n  Public clients only (token_endpoint_auth_methods_supported is [\"none\"]) with PKCE S256\n  required, and client identity established by client_id metadata document rather than\n  dynamic client registration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailoptin/refs/heads/main/scopes/mailoptin-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Email Marketing
- Marketing Automation
- Lead Generation
- WordPress
- Newsletters
- Webhook
- MCP
- Plugins
token_urls: []
---
