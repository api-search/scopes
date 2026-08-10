---
api_specs:
- filename: chili-piper-availability-api-openapi.yml
  format: yaml
  label: Chili Piper Availability API
  slug: chili-piper-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-availability-api-openapi.yml
- filename: chili-piper-chat-api-openapi.yml
  format: yaml
  label: Chili Piper Chat API
  slug: chili-piper-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-chat-api-openapi.yml
- filename: chili-piper-concierge-api-openapi.yml
  format: yaml
  label: Chili Piper Concierge API
  slug: chili-piper-concierge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-concierge-api-openapi.yml
- filename: chili-piper-distribution-api-openapi.yml
  format: yaml
  label: Chili Piper Distribution API
  slug: chili-piper-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-distribution-api-openapi.yml
- filename: chili-piper-distro-api-openapi.yml
  format: yaml
  label: Chili Piper Distro API
  slug: chili-piper-distro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-distro-api-openapi.yml
- filename: chili-piper-handoff-api-openapi.yml
  format: yaml
  label: Chili Piper Handoff API
  slug: chili-piper-handoff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-handoff-api-openapi.yml
- filename: chili-piper-meeting-type-api-openapi.yml
  format: yaml
  label: Chili Piper Meeting Type API
  slug: chili-piper-meeting-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meeting-type-api-openapi.yml
- filename: chili-piper-meeting-type-reminder-api-openapi.yml
  format: yaml
  label: Chili Piper Meeting Type Reminder API
  slug: chili-piper-meeting-type-reminder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meeting-type-reminder-api-openapi.yml
- filename: chili-piper-meetings-api-openapi.yml
  format: yaml
  label: Chili Piper Meetings API
  slug: chili-piper-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meetings-api-openapi.yml
- filename: chili-piper-rule-api-openapi.yml
  format: yaml
  label: Chili Piper Rule API
  slug: chili-piper-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-rule-api-openapi.yml
- filename: chili-piper-schedulinglinks-api-openapi.yml
  format: yaml
  label: Chili Piper Scheduling Links API
  slug: chili-piper-schedulinglinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-schedulinglinks-api-openapi.yml
- filename: chili-piper-team-api-openapi.yml
  format: yaml
  label: Chili Piper Team API
  slug: chili-piper-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-team-api-openapi.yml
- filename: chili-piper-tenant-api-openapi.yml
  format: yaml
  label: Chili Piper Tenant API
  slug: chili-piper-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-tenant-api-openapi.yml
- filename: chili-piper-user-api-openapi.yml
  format: yaml
  label: Chili Piper User API
  slug: chili-piper-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-user-api-openapi.yml
- filename: chili-piper-workspace-api-openapi.yml
  format: yaml
  label: Chili Piper Workspace API
  slug: chili-piper-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-workspace-api-openapi.yml
authorization_urls: []
description: 'Chili Piper API access tokens are scoped in Command Center at issue time. Scope is a matrix: a permission verb is granted per API section, so a token can be limited to exactly the surface a script or agent needs. The published OpenAPI documents declare only the apiKeyAuth bearer scheme and carry no oauth2 scope maps, so the matrix below is transcribed from Chili Piper documentation rather than derived from a spec.'
docs: https://help.chilipiper.com/hc/en-us/articles/35576029581971-Edge-API-References
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Chili Piper Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Chili Piper uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chili Piper
provider_slug: chili-piper
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: chili-piper-scopes
source_filename: chili-piper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://help.chilipiper.com/hc/en-us/articles/35576029581971-Edge-API-References\ndocs: https://help.chilipiper.com/hc/en-us/articles/35576029581971-Edge-API-References\ndescription: >-\n  Chili Piper API access tokens are scoped in Command Center at issue time. Scope is a matrix: a\n  permission verb is granted per API section, so a token can be limited to exactly the surface a\n  script or agent needs. The published OpenAPI documents declare only the apiKeyAuth bearer scheme\n  and carry no oauth2 scope maps, so the matrix below is transcribed from Chili Piper documentation\n  rather than derived from a spec.\nmodel: permission-matrix\nissuance:\n  ui_path: 'Command Center > Integrations > Credentials > API Access Tokens > Generate Token'\n  admin_only: true\n  note: >-\n    Only users with the Admin role can generate API tokens. Workspace Managers cannot access the\n    credentials page. The token value is shown once and\
  \ cannot be retrieved later.\n  management: 'Tokens list shows Last Access, Created Date and Created By; tokens can be viewed for permissions, removed and deleted. Deleting a token revokes its access immediately.'\npermissions:\n  - {verb: Ping, description: Health/reachability check only.}\n  - {verb: Read, description: Read access to the granted sections.}\n  - {verb: Modify, description: Create and update access to the granted sections.}\n  - {verb: Remove, description: Delete access to the granted sections.}\nsections:\n  - {section: Health, description: Monitor the health of the application.}\n  - {section: Tenant, description: Organization tenant metadata.}\n  - {section: Rule, description: Create/update/delete and list routing rules.}\n  - {section: Workspace, description: Read workspaces, add and remove users.}\n  - {section: Team, description: Read teams, add and remove users.}\n  - {section: Distribution, description: List, update, publish and delete distributions.}\n  - {section:\
  \ Availability, description: Available slots of assignees in round-robin meetings.}\n  - {section: User, description: Read/find users, invite users, update licenses.}\n  - {section: CRM, description: Activity, cancel and no-show by CRM event ID.}\n  - {section: Meetings, description: Query, get, cancel, no-show, activity and CSV export.}\n  - {section: Concierge, description: Routers, routing, scheduling and logs.}\n  - {section: 'Scheduling Links', description: List, initialize and schedule across link types.}\n  - {section: Handoff, description: Initialize a handoff flow and schedule from a handoff session.}\nnamed_scopes_documented:\n  - scope: Concierge.schedule\n    description: >-\n      Required to run a Concierge router from outside the UI via the Edge API.\n    source: https://help.chilipiper.com/hc/en-us/articles/30935152032275-Using-Concierge-via-the-Edge-API\noauth:\n  used_by: MCP server (https://fire.chilipiper.com/api/fire-edge/v1/org/mcp)\n  flow: browser-based authorization,\
  \ Admin on a paid account only\n  dynamic_client_registration: 'Client ID and secret are left blank by the client; no registration step is documented.'\n  protected_resource_metadata: well-known/chili-piper-oauth-protected-resource.json\n  published_scope_list: none\n  note: >-\n    Chili Piper publishes no OAuth scope list for the MCP OAuth path. The documentation states the\n    OAuth grant carries the signing-in Admin's org-wide permissions, and recommends the API-key path\n    when a narrower permission scope than the Admin OAuth grant is needed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/scopes/chili-piper-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Scheduling
- Lead Routing
- Meetings
- Sales
- Marketing
- CRM
- Demand Conversion
- Appointment Booking
- Revenue Operations
- Calendar
- Agents
- MCP
token_urls: []
---
