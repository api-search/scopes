---
api_specs:
- filename: socket-openapi-original.json
  format: json
  label: Socket API
  slug: socket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-openapi-original.json
authorization_urls: []
description: Socket authorizes REST API calls with organization API tokens that carry fine-grained token scopes (not OAuth2, but a documented permission model). Each endpoint declares the scopes it requires; a token missing a scope returns 403. Scopes below are harvested from the per-endpoint "requires the following org token scopes" notes in the Socket API reference.
docs: https://docs.socket.dev/reference/creating-and-managing-api-tokens
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Socket Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Socket publishes 34 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Socket API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Socket
provider_slug: socket
schemes:
- name: orgApiToken
  source: https://docs.socket.dev/docs/api-keys
  transport: Authorization Bearer / Basic
  type: api-token-scopes
scope_count: 34
scope_names:
- packages:list
- full-scans:create
- full-scans:list
- full-scans:delete
- diff-scans:create
- diff-scans:list
- diff-scans:delete
- alerts:list
- alert-resolution:list
- alert-resolution:read
- alert-resolution:delete
- triage:alerts-list
- triage:alerts-update
- repo:list
- repo:create
- repo:update
- repo:delete
- repo-label:list
- repo-label:create
- repo-label:update
- repo-label:delete
- report:read
- fixes:list
- security-policy:read
- security-policy:update
- license-policy:read
- license-policy:update
- historical:alerts-list
- historical:alerts-trend
- historical:dependencies-trend
- historical:snapshots-list
- historical:snapshots-start
- threat-feed:list
- socket-basics:read
scopes:
- description: Batch package/PURL metadata and alert lookups; license policy evaluation.
  flows: []
  scope: packages:list
- description: Create full scans and archive scans; rescan an existing full scan.
  flows: []
  scope: full-scans:create
- description: List, stream, download, and export (CSV/PDF) full scans and metadata.
  flows: []
  scope: full-scans:list
- description: Delete a full scan.
  flows: []
  scope: full-scans:delete
- description: Create diff scans from repo HEAD or from two full scan IDs.
  flows: []
  scope: diff-scans:create
- description: List and read diff scans and their GitHub-flavored-markdown comments.
  flows: []
  scope: diff-scans:list
- description: Delete a diff scan.
  flows: []
  scope: diff-scans:delete
- description: List latest/historical alerts and the full scans associated with an alert.
  flows: []
  scope: alerts:list
- description: List active alert resolutions for an organization.
  flows: []
  scope: alert-resolution:list
- description: Read a single alert resolution by UUID.
  flows: []
  scope: alert-resolution:read
- description: Delete an alert resolution.
  flows: []
  scope: alert-resolution:delete
- description: List alert triage actions for an organization.
  flows: []
  scope: triage:alerts-list
- description: Create, update, and delete alert triage actions.
  flows: []
  scope: triage:alerts-update
- description: List and read repositories.
  flows: []
  scope: repo:list
- description: Create repositories.
  flows: []
  scope: repo:create
- description: Update repository details.
  flows: []
  scope: repo:update
- description: Delete a repository and its scans.
  flows: []
  scope: repo:delete
- description: List and read repository labels and label settings.
  flows: []
  scope: repo-label:list
- description: Create repository labels.
  flows: []
  scope: repo-label:create
- description: Associate/disassociate labels and update label names and settings.
  flows: []
  scope: repo-label:update
- description: Delete a repository label and its associations.
  flows: []
  scope: repo-label:delete
- description: Export SBOMs (CycloneDX, SPDX, OpenVEX) for a scan.
  flows: []
  scope: report:read
- description: Fetch available fixes for vulnerabilities in a repo, scan, or manifest.
  flows: []
  scope: fixes:list
- description: Read an organization's security policy.
  flows: []
  scope: security-policy:read
- description: Update an organization's security policy.
  flows: []
  scope: security-policy:update
- description: Read an organization's license policy.
  flows: []
  scope: license-policy:read
- description: Update an organization's license policy.
  flows: []
  scope: license-policy:update
- description: List historical alerts (Beta).
  flows: []
  scope: historical:alerts-list
- description: Trend analytics of historical alerts (Beta).
  flows: []
  scope: historical:alerts-trend
- description: Trend analytics of historical dependencies (Beta).
  flows: []
  scope: historical:dependencies-trend
- description: List historical data snapshots (Beta).
  flows: []
  scope: historical:snapshots-list
- description: Start an on-demand historical snapshot job (Beta).
  flows: []
  scope: historical:snapshots-start
- description: Read the Socket threat feed (Enterprise plan with Threat Feed add-on).
  flows: []
  scope: threat-feed:list
- description: Read the Socket Basics CI/CD scanning configuration.
  flows: []
  scope: socket-basics:read
slug: socket-scopes
source_filename: socket-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.socket.dev/docs/api-keys\ndocs: https://docs.socket.dev/reference/creating-and-managing-api-tokens\ndescription: >-\n  Socket authorizes REST API calls with organization API tokens that carry fine-grained\n  token scopes (not OAuth2, but a documented permission model). Each endpoint declares the\n  scopes it requires; a token missing a scope returns 403. Scopes below are harvested from the\n  per-endpoint \"requires the following org token scopes\" notes in the Socket API reference.\nschemes:\n- name: orgApiToken\n  type: api-token-scopes\n  source: https://docs.socket.dev/docs/api-keys\n  transport: Authorization Bearer / Basic\nscopes:\n- scope: packages:list\n  description: Batch package/PURL metadata and alert lookups; license policy evaluation.\n- scope: full-scans:create\n  description: Create full scans and archive scans; rescan an existing full scan.\n- scope: full-scans:list\n  description: List, stream,\
  \ download, and export (CSV/PDF) full scans and metadata.\n- scope: full-scans:delete\n  description: Delete a full scan.\n- scope: diff-scans:create\n  description: Create diff scans from repo HEAD or from two full scan IDs.\n- scope: diff-scans:list\n  description: List and read diff scans and their GitHub-flavored-markdown comments.\n- scope: diff-scans:delete\n  description: Delete a diff scan.\n- scope: alerts:list\n  description: List latest/historical alerts and the full scans associated with an alert.\n- scope: alert-resolution:list\n  description: List active alert resolutions for an organization.\n- scope: alert-resolution:read\n  description: Read a single alert resolution by UUID.\n- scope: alert-resolution:delete\n  description: Delete an alert resolution.\n- scope: triage:alerts-list\n  description: List alert triage actions for an organization.\n- scope: triage:alerts-update\n  description: Create, update, and delete alert triage actions.\n- scope: repo:list\n  description:\
  \ List and read repositories.\n- scope: repo:create\n  description: Create repositories.\n- scope: repo:update\n  description: Update repository details.\n- scope: repo:delete\n  description: Delete a repository and its scans.\n- scope: repo-label:list\n  description: List and read repository labels and label settings.\n- scope: repo-label:create\n  description: Create repository labels.\n- scope: repo-label:update\n  description: Associate/disassociate labels and update label names and settings.\n- scope: repo-label:delete\n  description: Delete a repository label and its associations.\n- scope: report:read\n  description: Export SBOMs (CycloneDX, SPDX, OpenVEX) for a scan.\n- scope: fixes:list\n  description: Fetch available fixes for vulnerabilities in a repo, scan, or manifest.\n- scope: security-policy:read\n  description: Read an organization's security policy.\n- scope: security-policy:update\n  description: Update an organization's security policy.\n- scope: license-policy:read\n\
  \  description: Read an organization's license policy.\n- scope: license-policy:update\n  description: Update an organization's license policy.\n- scope: historical:alerts-list\n  description: List historical alerts (Beta).\n- scope: historical:alerts-trend\n  description: Trend analytics of historical alerts (Beta).\n- scope: historical:dependencies-trend\n  description: Trend analytics of historical dependencies (Beta).\n- scope: historical:snapshots-list\n  description: List historical data snapshots (Beta).\n- scope: historical:snapshots-start\n  description: Start an on-demand historical snapshot job (Beta).\n- scope: threat-feed:list\n  description: Read the Socket threat feed (Enterprise plan with Threat Feed add-on).\n- scope: socket-basics:read\n  description: Read the Socket Basics CI/CD scanning configuration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/scopes/socket-scopes.yml
summary_line: 34 scopes
tags:
- Company
- Security
- Software Supply Chain Security
- Dependency Scanning
- Software Composition Analysis
- Vulnerability Management
- Open Source Security
- DevSecOps
- SBOM
- Package Analysis
token_urls: []
---
