---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Innovusion Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no OpenAPI oauth2 securityScheme for this provider (there is no OpenAPI at all). The scope list below is not derived — it is read verbatim from the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata that seyond.com serves anonymously. Seyond publishes no scopes or permissions reference page; a docs URL is recorded as null rather than guessed.
overview: 'Seyond uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Seyond
provider_slug: innovusion
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: innovusion-scopes
source_filename: innovusion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://seyond.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  derive-oauth-scopes.py found no OpenAPI oauth2 securityScheme for this provider (there is no OpenAPI at\n  all). The scope list below is not derived — it is read verbatim from the RFC 8414 authorization-server\n  metadata and the RFC 9728 protected-resource metadata that seyond.com serves anonymously. Seyond\n  publishes no scopes or permissions reference page; a docs URL is recorded as null rather than guessed.\nauthorization_server: https://seyond.com\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The only scope advertised by seyond.com's authorization server, and the only scope named in the\n    protected-resource metadata for https://seyond.com/wp-json/mcp/mcp-oauth-server. No finer-grained\n    scopes are published; per-tool authorization, if any, is not anonymously discoverable.\n  source: both scopes_supported arrays (authorization-server\
  \ and protected-resource metadata)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovusion/refs/heads/main/scopes/innovusion-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- LiDAR
- Sensors
- Autonomous Driving
- Intelligent Transportation
- Robotics
- Perception
- Smart Cities
- Automotive
- Hardware
token_urls: []
---
