---
authorization_urls: []
description: The Nidra MCP authorization server advertises exactly one scope. Both the RFC 8414 Authorization Server Metadata and the RFC 9728 Protected Resource Metadata list the same single value, and no scope reference page is published anywhere on either host, so this list is complete as published rather than a sample.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Noctrix Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Noctrix Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Noctrix Health
provider_slug: noctrix-health
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: noctrix-health-scopes
source_filename: noctrix-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://nidrarls.com/.well-known/oauth-authorization-server\nname: Noctrix Health OAuth scopes\ndescription: >-\n  The Nidra MCP authorization server advertises exactly one scope. Both the RFC 8414\n  Authorization Server Metadata and the RFC 9728 Protected Resource Metadata list the same\n  single value, and no scope reference page is published anywhere on either host, so this\n  list is complete as published rather than a sample.\nauthorization_server: https://nidrarls.com\nresource: https://nidrarls.com/wp-json/mcp/mcp-oauth-server\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page exists. Searched nidrarls.com (including its\n  llms.txt page inventory and .md twins) and noctrixhealth.com, which is bot-challenged.\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Grants a client access to the Model Context Protocol server. Declared verbatim in\n    scopes_supported; the provider publishes no description,\
  \ and none is invented here.\n  source: /.well-known/oauth-authorization-server\n  applies_to: https://nidrarls.com/wp-json/mcp/mcp-oauth-server\n  granularity: coarse\n  note: >-\n    A single undifferentiated scope. There is no read/write split, so a consent screen\n    cannot tell a user what the grant will let an agent do.\nchecked: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noctrix-health/refs/heads/main/scopes/noctrix-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health
- Medical Devices
- Digital Health
- Sleep
- Neurology
- Neurostimulation
- Wearables
- Model Context Protocol
- Agent Readiness
token_urls: []
---
