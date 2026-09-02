---
api_specs:
- filename: index.html
  format: yaml
  label: Skyvia Public API
  slug: skyvia-public-api
  spec_type: OpenAPI
  url: https://api.skyvia.com/swagger/index.html
authorization_urls: []
description: ''
docs: https://docs.skyvia.com/account-management/api-settings.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Skyvia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Skyvia uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Skyvia
provider_slug: skyvia
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: skyvia-scopes
source_filename: skyvia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.skyvia.com/account-management/api-settings.html\ndocs: https://docs.skyvia.com/account-management/api-settings.html\nscheme: api-token-scopes\noauth2: false\nsummary: >-\n  IMPORTANT: these are NOT OAuth 2.0 scopes. Skyvia runs no OAuth or OIDC. A Skyvia API token is an opaque\n  bearer credential created in Account Settings > API Settings, and at creation time the user selects a set\n  of per-resource permissions the token carries. Those permissions are the scope model recorded here. They\n  are documented in prose on the API Settings page and appear nowhere in the OpenAPI document — the spec\n  declares a single `Access Token` apiKey scheme with an empty scope list on every operation, so an agent\n  reading only the spec cannot tell which token permission any operation needs. The mapping below is\n  reconstructed from the documented permission names against the operations they govern.\nscope_count: 18\nresources:\n\
  - resource: Account\n  scopes:\n  - scope: Account / Read\n    description: Access user and invitation lists.\n    governs:\n    - GET /v1/account/users\n    - GET /v1/account/invitations\n  - scope: Account / Modify\n    description: Manage users and invitations.\n    governs:\n    - DELETE /v1/account/users\n    - POST /v1/account/invitations\n    - POST /v1/account/invitations/{invitationId}/resend\n    - DELETE /v1/account/invitations/{invitationId}\n- resource: Agent\n  scopes:\n  - scope: Agent / Read\n    description: View agent lists and details.\n    governs:\n    - GET /v1/workspaces/{workspaceId}/agents\n    - GET /v1/workspaces/{workspaceId}/agents/{agentId}\n  - scope: Agent / Modify\n    description: Test agent connections.\n    governs:\n    - POST /v1/workspaces/{workspaceId}/agents/{agentId}/test\n- resource: Automation\n  scopes:\n  - scope: Automation / Read\n    description: View automation lists, details, state and execution history.\n    governs:\n    - GET /v1/workspaces/{workspaceId}/automations\n\
  \    - GET /v1/workspaces/{workspaceId}/automations/{automationId}\n    - GET /v1/workspaces/{workspaceId}/automations/{automationId}/executions\n    - GET /v1/workspaces/{workspaceId}/automations/{automationId}/executions/{executionId}\n    - GET /v1/workspaces/{workspaceId}/automations/{automationId}/state\n    - GET /v1/workspaces/{workspaceId}/automations/{automationId}/active\n  - scope: Automation / Execute\n    description: Run automations.\n  - scope: Automation / Enable-Disable\n    description: Control automation status.\n    governs:\n    - POST /v1/workspaces/{workspaceId}/automations/{automationId}/enable\n    - POST /v1/workspaces/{workspaceId}/automations/{automationId}/disable\n- resource: Connection\n  scopes:\n  - scope: Connection / Read\n    description: View connection lists and details.\n    governs:\n    - GET /v1/workspaces/{workspaceId}/connections\n    - GET /v1/workspaces/{workspaceId}/connections/{connectionId}\n  - scope: Connection / Test\n    description:\
  \ Verify connection functionality.\n    governs:\n    - POST /v1/workspaces/{workspaceId}/connections/{connectionId}/test\n- resource: Endpoint\n  scopes:\n  - scope: Endpoint / Read\n    description: Access Connect endpoint information and request logs.\n    governs:\n    - GET /v1/endpoints/types\n    - GET /v1/workspaces/{workspaceId}/endpoints\n    - GET /v1/workspaces/{workspaceId}/endpoints/{endpointId}\n    - GET /v1/workspaces/{workspaceId}/endpoints/{endpointId}/executions\n    - GET /v1/workspaces/{workspaceId}/endpoints/{endpointId}/executions/{recordId}\n  - scope: Endpoint / Enable-Disable\n    description: Control endpoint status.\n    governs:\n    - POST /v1/workspaces/{workspaceId}/endpoints/{endpointId}/enable\n    - POST /v1/workspaces/{workspaceId}/endpoints/{endpointId}/disable\n- resource: Integration\n  scopes:\n  - scope: Integration / Read\n    description: View integrations and execution history.\n    governs:\n    - GET /v1/workspaces/{workspaceId}/integrations\n\
  \    - GET /v1/workspaces/{workspaceId}/integrations/{integrationId}\n    - GET /v1/workspaces/{workspaceId}/integrations/{integrationId}/executions\n    - GET /v1/workspaces/{workspaceId}/integrations/{integrationId}/executions/{executionId}\n    - GET /v1/workspaces/{workspaceId}/integrations/{integrationId}/executions/active\n  - scope: Integration / Execute\n    description: Run integrations and manage execution.\n    governs:\n    - POST /v1/workspaces/{workspaceId}/integrations/{integrationId}/executions\n    - POST /v1/workspaces/{workspaceId}/integrations/{integrationId}/executions/cancel\n    - POST /v1/workspaces/{workspaceId}/integrations/{integrationId}/executions/kill\n  - scope: Integration / Read Schedule\n    description: Access scheduling information.\n    governs:\n    - GET /v1/workspaces/{workspaceId}/integrations/{integrationId}/schedule\n  - scope: Integration / Enable-Disable Schedule\n    description: Control schedule status.\n    governs:\n    - POST /v1/workspaces/{workspaceId}/integrations/{integrationId}/schedule/enable\n\
  \    - POST /v1/workspaces/{workspaceId}/integrations/{integrationId}/schedule/disable\n- resource: Workspace\n  scopes:\n  - scope: Workspace / Read\n    description: View workspace information.\n    governs:\n    - GET /v1/workspaces\n    - GET /v1/workspaces/{workspaceId}\n  - scope: Workspace / Read Users\n    description: Access workspace user lists.\n    governs:\n    - GET /v1/workspaces/{workspaceId}/users\n  - scope: Workspace / Modify Users\n    description: Manage user workspace access.\n    governs:\n    - POST /v1/workspaces/{workspaceId}/users\n    - DELETE /v1/workspaces/{workspaceId}/users/{userId}\nunmapped:\n- scope: Automation / Execute\n  reason: >-\n    Documented as a token permission, but the v1 API publishes no operation that starts an automation —\n    automations are started by their own trigger (manual, schedule, connection polling, or webhook). Recorded\n    as published-but-unbound rather than mapped to a guess. Backup schedule enable/disable and snapshot\n\
  \    creation, conversely, appear in the spec but are not named as a distinct Backup permission on the API\n    Settings page.\ngaps:\n- The scope model is prose-only; no scope strings appear in the OpenAPI, so per-operation authorization is not machine-readable.\n- No scope-to-operation table is published by Skyvia; the mapping above is derived by API Evangelist from resource names and is marked as such.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyvia/refs/heads/main/scopes/skyvia-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Data Integration
- iPaaS
- ETL
- ELT
- Data Replication
- Cloud Backup
- OData
- SQL
- Workflow-Automation
- No-Code
- Connectors
- Data Management
- MCP
- agent-native
- Data Access
token_urls: []
---
