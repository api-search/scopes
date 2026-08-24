---
authorization_urls: []
description: ''
docs: https://docs.granica.ai/security-and-compliance/api-token
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Granica Scopes
name_suffix: OAuth Scopes
note: These are NOT OAuth 2.0 scopes. Granica calls them "Access Policies" and "Scope keys" - they are attached to a long-lived bearer API key at creation time and enforced on every request in addition to the caller's RBAC role. They are recorded here because they are the provider's own published, named permission surface and read exactly like scopes. Granica does not run an OAuth authorization server; the only OAuth/OIDC in the product is inbound Console SSO against the customer's own identity provider.
overview: 'Granica uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Granica
provider_slug: granica
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: granica-scopes
source_filename: granica-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://docs.granica.ai/security-and-compliance/api-token\ndocs: https://docs.granica.ai/security-and-compliance/api-token\napi: Granica APIs V1\nnote: >-\n  These are NOT OAuth 2.0 scopes. Granica calls them \"Access Policies\" and \"Scope keys\" - they are attached\n  to a long-lived bearer API key at creation time and enforced on every request in addition to the caller's\n  RBAC role. They are recorded here because they are the provider's own published, named permission surface\n  and read exactly like scopes. Granica does not run an OAuth authorization server; the only OAuth/OIDC in\n  the product is inbound Console SSO against the customer's own identity provider.\nmodel: api-key-access-policy\ndefault_when_none_selected: full access to all API endpoints\ngroups:\n- id: table_discovery_onboarding\n  name: Table Discovery & Onboarding\n  scopes:\n  - key: tables:read\n    description: List tables, view schema, partitions,\
  \ and size metrics.\n  - key: tables:write\n    description: Onboard, update, and remove tables.\n  - key: catalog_connections:read\n    description: List connections, browse catalogs, schemas, and discovered tables.\n  - key: catalog_connections:write\n    description: Create, update, delete connections and trigger syncs.\n  - key: onboarding:read\n    description: Check progress of table onboarding workflows.\n  - key: onboarding:write\n    description: Retry onboarding tasks that have failed.\n- id: crunch_file_optimization\n  name: Crunch - File Optimization\n  scopes:\n  - key: crunch:read\n    description: View job status, execution history, compression metrics.\n  - key: crunch:write\n    description: Run on-demand crunch jobs.\n  - key: crunch_policy:read\n    description: View which primitives are enabled and their configuration.\n  - key: crunch_policy:write\n    description: Enable/disable and configure Compression, Compaction, Sorting, Clustering, and Deduplication.\n  - key:\
  \ schedules:read\n    description: View automated crunch schedules.\n  - key: schedules:write\n    description: Create, update, and delete crunch schedules.\n- id: vacuum\n  name: Vacuum\n  scopes:\n  - key: vacuum:read\n    description: View vacuum job status and cleanup metrics.\n  - key: vacuum:write\n    description: Run on-demand vacuum to expire snapshots and delete orphaned files.\n  - key: vacuum_policy:read\n    description: View retention settings and vacuum policy configuration.\n  - key: vacuum_policy:write\n    description: Update vacuum retention policy.\n- id: partition_expiration\n  name: Partition Expiration\n  scopes:\n  - key: partition_exp_policy:read\n    description: View partition retention rules.\n  - key: partition_exp_policy:write\n    description: Create and update partition expiration policies.\n- id: platform_administration\n  name: Platform Administration\n  scopes:\n  - key: config:read\n    description: Read platform configuration and health status.\n  -\
  \ key: config:write\n    description: Modify platform-level configuration settings.\npresets:\n- name: Read Only\n  description: >-\n    View everything across all groups - tables, crunch jobs, vacuum history, schedules, policies, and config.\n    No write access.\n- name: Full Maintenance\n  description: >-\n    Complete table maintenance - crunch, vacuum, partition expiration, and schedule management. Excludes\n    catalog management and platform admin.\n- name: Vacuum Only\n  description: Snapshot expiration and orphan file cleanup - vacuum read, write, and policy scopes only.\nscope_count: 20\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granica/refs/heads/main/scopes/granica-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Data
- Storage
- Analytics
- Artificial Intelligence
- Machine Learning
- Data Lakehouse
- Cloud Cost Optimization
- Compression
- Data Infrastructure
token_urls: []
---
