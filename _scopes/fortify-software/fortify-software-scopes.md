---
api_specs:
- filename: fortify-software-fod-openapi.json
  format: json
  label: Fortify on Demand REST API (v3)
  slug: fortify-on-demand-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortify-software/refs/heads/main/openapi/fortify-software-fod-openapi.json
authorization_urls: []
description: ''
docs: https://www.microfocus.com/documentation/fortify-on-demand/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Fortify Software Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fortify Software publishes 13 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fortify Software API on a user''s behalf.


  Tokens are issued from https://api.ams.fortify.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fortify Software
provider_slug: fortify-software
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.ams.fortify.com/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/fortify-software-fod-openapi.json
scope_count: 13
scope_names:
- api-tenant
- view-apps
- manage-apps
- view-issues
- manage-issues
- start-scans
- view-reports
- manage-reports
- view-users
- manage-users
- manage-user
- view-tenant-data
- manage-notifications
scopes:
- description: Broad tenant-level API access scope.
  flows: []
  scope: api-tenant
- description: Read access to applications and releases.
  flows: []
  scope: view-apps
- description: Read-write access to applications and releases.
  flows: []
  scope: manage-apps
- description: Read access to vulnerabilities / issues.
  flows: []
  scope: view-issues
- description: Read-write access to vulnerabilities / issues (audit, suppress, comment).
  flows: []
  scope: manage-issues
- description: Permission to start static, dynamic, mobile and open-source scans.
  flows: []
  scope: start-scans
- description: Read access to reports and data exports.
  flows: []
  scope: view-reports
- description: Read-write access to create and manage reports and data exports.
  flows: []
  scope: manage-reports
- description: Read access to users and user groups.
  flows: []
  scope: view-users
- description: Read-write access to users and user groups.
  flows: []
  scope: manage-users
- description: Manage an individual user account.
  flows: []
  scope: manage-user
- description: Read access to tenant-level data (entitlements, summaries, heatmaps).
  flows: []
  scope: view-tenant-data
- description: Read-write access to notifications.
  flows: []
  scope: manage-notifications
slug: fortify-software-scopes
source_filename: fortify-software-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fortify-software-fod-openapi.json\ndocs: https://www.microfocus.com/documentation/fortify-on-demand/\nnotes: >-\n  Scopes extracted verbatim from the \"Allowed Scopes:\" clause in every operation\n  description of the Fortify on Demand v3 Swagger document, cross-referenced with\n  the FoD API access documentation. FoD uses OAuth 2.0 client-credentials; the\n  requested `scope` gates operation access. `api-tenant` is the broad tenant scope;\n  the view-*/manage-* pairs are read vs. read-write per domain.\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/fortify-software-fod-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ams.fortify.com/oauth/token\nscopes:\n- scope: api-tenant\n  description: Broad tenant-level API access scope.\n- scope: view-apps\n  description: Read access to applications and releases.\n- scope: manage-apps\n  description: Read-write access to applications\
  \ and releases.\n- scope: view-issues\n  description: Read access to vulnerabilities / issues.\n- scope: manage-issues\n  description: Read-write access to vulnerabilities / issues (audit, suppress, comment).\n- scope: start-scans\n  description: Permission to start static, dynamic, mobile and open-source scans.\n- scope: view-reports\n  description: Read access to reports and data exports.\n- scope: manage-reports\n  description: Read-write access to create and manage reports and data exports.\n- scope: view-users\n  description: Read access to users and user groups.\n- scope: manage-users\n  description: Read-write access to users and user groups.\n- scope: manage-user\n  description: Manage an individual user account.\n- scope: view-tenant-data\n  description: Read access to tenant-level data (entitlements, summaries, heatmaps).\n- scope: manage-notifications\n  description: Read-write access to notifications.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortify-software/refs/heads/main/scopes/fortify-software-scopes.yml
summary_line: 13 scopes · clientCredentials
tags:
- Company
- Security
- Application Security
- AppSec
- SAST
- DAST
- Vulnerability Management
- DevSecOps
- Software Composition Analysis
- API Security
token_urls:
- https://api.ams.fortify.com/oauth/token
---
