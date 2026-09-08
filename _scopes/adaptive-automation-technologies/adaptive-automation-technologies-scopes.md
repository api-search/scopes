---
authorization_urls: []
description: Adaptive publishes a closed, ten-entry scope vocabulary that governs BOTH restricted Client App API keys and the consent screen an interactive MCP client sees. Scopes are selected at key creation and are immutable thereafter — changing them means deleting the key and issuing a new one. A key created before scopes existed carries Full access. These are operation scopes on a REST/MCP surface rather than OAuth 2.0 scopes negotiated per authorization request, but the MCP OAuth flow presents the same vocabulary and intersects it with any bound Client App.
docs: https://documentation.adaptive.live/developer-guide/adaptive-api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Adaptive Automation Technologies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adaptive Automation Technologies uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adaptive Automation Technologies
provider_slug: adaptive-automation-technologies
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: adaptive-automation-technologies-scopes
source_filename: adaptive-automation-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://documentation.adaptive.live/developer-guide/adaptive-api\ndocs: https://documentation.adaptive.live/developer-guide/adaptive-api\ndescription: >-\n  Adaptive publishes a closed, ten-entry scope vocabulary that governs BOTH restricted Client\n  App API keys and the consent screen an interactive MCP client sees. Scopes are selected at\n  key creation and are immutable thereafter — changing them means deleting the key and\n  issuing a new one. A key created before scopes existed carries Full access. These are\n  operation scopes on a REST/MCP surface rather than OAuth 2.0 scopes negotiated per\n  authorization request, but the MCP OAuth flow presents the same vocabulary and intersects\n  it with any bound Client App.\nscope_model:\n  default: Full access — the key can call every Client API endpoint\n  restricted: Restricted to selected operations — any other endpoint returns 403\n  mutable_after_creation: false\n  ceiling:\
  \ >-\n    For MCP tokens the offered list is always capped at the connecting user's own role, so an\n    agent can never exceed the human who authorized it.\n  denial: '403 operation not permitted for this key'\nscopes:\n- name: users:read\n  description: List Users — all users and teams in the organization.\n  operations: [GET /api/v3/client/users/list]\n- name: resources:read\n  description: List Resources — all resources in the organization.\n  operations: [GET /api/v3/client/resources/list]\n- name: endpoints:read\n  description: List Endpoints — all endpoints in the organization.\n  operations: [GET /api/v3/client/endpoints/list]\n- name: authorizations:read\n  description: >-\n    List Authorizations — metadata only; the permission policy body lives in an encrypted\n    field and is not returned.\n  operations: [GET /api/v3/client/authorizations/list]\n- name: scripts:read\n  description: >-\n    List Scripts — non-sensitive metadata only; the script body is never returned because\
  \ a\n    script command can embed inline credentials.\n  operations: [GET /api/v3/client/scripts/list]\n- name: schema:read\n  description: >-\n    Fetch Schema — the table/column schema of a database resource. Supported for MySQL,\n    PostgreSQL and SQL Server resources only.\n  operations: ['GET /api/v3/client/schema/{resourceId}/info']\n- name: team:read\n  description: List Teams, List Users of a Team, List Endpoints of a Team.\n  operations:\n  - GET /api/v3/client/teams/list\n  - 'GET /api/v3/client/team/{teamId}/users/list/'\n  - 'GET /api/v3/client/team/{teamId}/endpoint/list/'\n- name: team:write\n  description: >-\n    Add and remove users and endpoints on a team. Only API-managed teams may be modified.\n  operations:\n  - POST /api/v3/client/team/users/add\n  - POST /api/v3/client/team/users/remove\n  - POST /api/v3/client/team/endpoint/add\n  - POST /api/v3/client/team/endpoint/remove\n- name: activity:read\n  description: >-\n    Fetch Activity Log — streams workspace activity\
  \ as CSV for compliance export and SIEM\n    ingestion.\n  operations: [POST /api/v3/client/activity-log]\n- name: access-request:write\n  description: >-\n    Create and Decide Access Requests — raise an access request and approve or reject it in\n    one call, for externally-secured approval workflows.\n  operations: [POST /api/v3/client/access-request]\ncompound_requirements:\n- operation: GET /api/v3/client/endpoints/with-users\n  requires: [endpoints:read, users:read]\n  rationale: >-\n    Provider-stated: a restricted key holding only one of the two is rejected with 403. This\n    deliberately keeps endpoints:read from implicitly granting the ability to enumerate\n    users.\nscope_count: 10\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-automation-technologies/refs/heads/main/scopes/adaptive-automation-technologies-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Security
- Privileged Access Management
- Identity and Access Management
- Data Security
- Agents
- Model Context Protocol
- Infrastructure
- Databases
- Kubernetes
- Compliance
- Audit
token_urls: []
---
