---
api_specs:
- filename: rudderstack-event-streaming-asyncapi.yml
  format: yaml
  label: RudderStack Webhook Source API
  slug: rudderstack-webhook-source-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/asyncapi/rudderstack-event-streaming-asyncapi.yml
- filename: rudderstack-http-api-api-openapi.yml
  format: yaml
  label: RudderStack HTTP API API
  slug: rudderstack-http-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/openapi/rudderstack-http-api-api-openapi.yml
- filename: rudderstack-internal-api-api-openapi.yml
  format: yaml
  label: RudderStack Internal API API
  slug: rudderstack-internal-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/openapi/rudderstack-internal-api-api-openapi.yml
authorization_urls: []
description: RudderStack runs an OAuth 2.0 authorization server for its hosted MCP endpoint, but PUBLISHES NO SCOPES. The RFC 8414 metadata document at https://mcp.rudderstack.com/.well-known/oauth-authorization-server returns HTTP 200 and declares issuer, endpoints, grant types, PKCE methods and token endpoint auth methods — and omits `scopes_supported` entirely. The RFC 9728 protected-resource document likewise omits `scopes_supported`. There is no scope vocabulary for a client to request or for this catalog to record. This is an honest zero, not a gap in the probe. Authorization is instead expressed as workspace ACCESS POLICIES applied to the token holder — organization-level Service Access Tokens carry Admin by default, workspace-level SATs carry a configurable resource-permission policy, and Personal Access Tokens inherit the user's role. Those permissions are managed in the dashboard and are not exposed as OAuth scopes.
docs: https://www.rudderstack.com/docs/access-management/policies-overview/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Rudderstack Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RudderStack uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RudderStack
provider_slug: rudderstack
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rudderstack-scopes
source_filename: rudderstack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.rudderstack.com/.well-known/oauth-authorization-server\ndocs: https://www.rudderstack.com/docs/access-management/policies-overview/\ndescription: >-\n  RudderStack runs an OAuth 2.0 authorization server for its hosted MCP endpoint,\n  but PUBLISHES NO SCOPES. The RFC 8414 metadata document at\n  https://mcp.rudderstack.com/.well-known/oauth-authorization-server returns HTTP\n  200 and declares issuer, endpoints, grant types, PKCE methods and token\n  endpoint auth methods — and omits `scopes_supported` entirely. The RFC 9728\n  protected-resource document likewise omits `scopes_supported`. There is no\n  scope vocabulary for a client to request or for this catalog to record. This is\n  an honest zero, not a gap in the probe.\n  Authorization is instead expressed as workspace ACCESS POLICIES applied to the\n  token holder — organization-level Service Access Tokens carry Admin by default,\n  workspace-level SATs carry\
  \ a configurable resource-permission policy, and\n  Personal Access Tokens inherit the user's role. Those permissions are managed\n  in the dashboard and are not exposed as OAuth scopes.\nauthorization_server: https://mcp.rudderstack.com\nscopes_supported: null\nscope_count: 0\nevidence:\n  - url: https://mcp.rudderstack.com/.well-known/oauth-authorization-server\n    http_status: 200\n    finding: no scopes_supported member\n    file: well-known/rudderstack-mcp-oauth-authorization-server.json\n  - url: https://mcp.rudderstack.com/.well-known/oauth-protected-resource\n    http_status: 200\n    finding: no scopes_supported member\n    file: well-known/rudderstack-mcp-oauth-protected-resource.json\n  - url: https://mcp.rudderstack.com/mcp\n    http_status: 401\n    finding: >-\n      WWW-Authenticate challenge names only resource_metadata and\n      error=\"invalid_token\" — no scope hint.\nscopes: []\npermission_model:\n  style: role-and-policy, not scope\n  levels:\n    - name: Organization\
  \ Service Access Token\n      default: Admin permissions across the organization\n      docs: https://www.rudderstack.com/docs/access-management/service-access-tokens/\n    - name: Workspace Service Access Token\n      default: Configured under the workspace SAT access policy at creation time\n      docs: https://www.rudderstack.com/docs/access-management/policies-overview/\n    - name: Personal Access Token\n      default: Inherits the individual member's role\n      docs: https://www.rudderstack.com/docs/access-management/personal-access-tokens/\n  enterprise_access_management:\n    plans: [Enterprise]\n    note: The pricing page lists \"Enterprise access management — 3 groups\" on Growth and unlimited on Enterprise.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/scopes/rudderstack-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Customer Data Platform
- CDP
- Data Pipeline
- Open Source
- Event Streaming
- Reverse ETL
- Analytics
- Identity Resolution
token_urls: []
---
