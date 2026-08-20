---
authorization_urls: []
description: Cubby's only true OAuth scope surface belongs to its MCP server, and it is a single coarse scope. The REST APIs have no OAuth at all; their authorization axis is a named role stamped on each issued API key, which is recorded here alongside because it is the permission model an integrator actually reasons about.
docs: https://cubbystorage.github.io/docs/api/#roles
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cubby Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cubby uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cubby
provider_slug: cubby
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cubby-scopes
source_filename: cubby-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://api.cubbystorage.com/.well-known/oauth-authorization-server\ndocs: https://cubbystorage.github.io/docs/api/#roles\ndescription: >-\n  Cubby's only true OAuth scope surface belongs to its MCP server, and it is a single\n  coarse scope. The REST APIs have no OAuth at all; their authorization axis is a named\n  role stamped on each issued API key, which is recorded here alongside because it is\n  the permission model an integrator actually reasons about.\noauth:\n  authorization_server: https://api.cubbystorage.com\n  scope_count: 1\n  scopes:\n  - name: mcp\n    description: >-\n      The single scope advertised by both the RFC 8414 authorization server metadata and\n      the RFC 9728 protected resource metadata. Not decomposed by resource or by read/write\n      — a granted MCP token carries the whole server.\n    resource: https://api.cubbystorage.com\n    source: /.well-known/oauth-authorization-server\n  granularity:\
  \ coarse\n  note: >-\n    A single undifferentiated `mcp` scope means consent for an agent is all-or-nothing.\n    Given the underlying REST surface writes leases, charges cards, starts liens and sends\n    tenant messages, this is the most consequential authorization gap on the profile.\nkey_roles:\n  model: role-per-API-key (not OAuth scopes)\n  count: 8\n  values:\n  - name: Manager\n    access: read+write across nearly all resources; read on access codes, discounts, facilities,\n      facility groups, ledgers, organizations, payment methods\n  - name: Search\n  - name: Storefront\n  - name: Report\n  - name: Coverages\n  - name: Access Codes\n  - name: Communication\n  - name: Locks\n  source: https://cubbystorage.github.io/docs/api/#roles\n  note: >-\n    Roles are documented with a per-resource endpoint table in the API reference, added in\n    the May 2026 changelog entry \"Documentation: roles and permissions\".\npii:\n  separate_entitlement: true\n  note: PII visibility is an\
  \ independent flag on the key, orthogonal to the role.\nx-evidence:\n  fetched: '2026-08-11'\n  probes:\n  - url: https://api.cubbystorage.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://api.cubbystorage.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://cubbystorage.github.io/docs/api/\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubby/refs/heads/main/scopes/cubby-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Self Storage
- Property Management
- Facility Management
- Real-Estate
- Payments
- Software-as-a-Service
- Artificial Intelligence
- Revenue Management
- E-Commerce
token_urls: []
---
