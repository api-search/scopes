---
authorization_urls:
- https://app.klue.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Klue Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Klue publishes 23 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Klue API on a user''s behalf.


  Tokens are issued from https://app.klue.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Klue
provider_slug: klue
schemes:
- code_challenge_methods_supported:
  - plain
  - S256
  endpoints:
    authorization: https://app.klue.com/oauth/authorize
    dynamic_client_registration: https://app.klue.com/oauth/register
    introspection: https://app.klue.com/oauth/introspect
    jwks: https://app.klue.com/oauth/discovery/keys
    revocation: https://app.klue.com/oauth/revoke
    token: https://app.klue.com/oauth/token
    userinfo: https://app.klue.com/oauth/userinfo
  flows:
  - authorizationUrl: https://app.klue.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.klue.com/oauth/token
    tokenUrl: https://app.klue.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  implementation_note: The kluein GitHub organization maintains a fork of devise-doorkeeper (https://github.com/kluein/devise-doorkeeper), the Rails Doorkeeper OAuth2 provider integration; the endpoint layout below matches a Doorkeeper deployment.
  issuer: https://app.klue.com
  name: klue-oauth2
  response_types_supported:
  - code
  source: https://app.klue.com/.well-known/openid-configuration
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
scope_count: 23
scope_names:
- openid
- content:read
- content:edit
- win_loss:read
- deal_answers:read
- auto_insights:read
- deal_context:read
- transcript:edit
- crm:edit
- stak_play_mcp:read
- stak_play_mcp:edit
- scim:read
- scim:edit
- slack
- teams
- connect
- usage_reports:read
- service_read
- service_write
- customer_success
- impersonate
- alpha:read
- alpha:edit
scopes:
- description: OpenID Connect authentication; returns an RS256-signed ID token.
  flows: []
  scope: openid
- description: Read access to Klue content (cards, battlecards). API Evangelist reading — Klue publishes no description; the name aligns with the read surface of the Klue Content API and the v1 MCP connector.
  flows: []
  scope: content:read
- description: Write access to Klue content. API Evangelist reading — aligns with the create/update/delete card and battlecard tooling Klue describes as the "admin MCP endpoint" writeback surface.
  flows: []
  scope: content:edit
- description: Read access to win-loss interviews, transcripts and reports. API Evangelist reading — aligns with the win-loss MCP tool family.
  flows: []
  scope: win_loss:read
- description: Read access to deal answers. API Evangelist reading — likely the Smart Answers / Deal Tips surface.
  flows: []
  scope: deal_answers:read
- description: Read access to Auto Insights, Klue's AI-generated insight pipeline. API Evangelist reading; the v2 MCP connector exposes search_agent_insights.
  flows: []
  scope: auto_insights:read
- description: Read access to deal context. API Evangelist reading.
  flows: []
  scope: deal_context:read
- description: Write access to interview transcripts. API Evangelist reading.
  flows: []
  scope: transcript:edit
- description: Write access to the connected CRM surface. API Evangelist reading; Klue integrates with Salesforce, HubSpot and MS Dynamics.
  flows: []
  scope: crm:edit
- description: Read scope for Klue's MCP surface. API Evangelist reading — this is the only scope in the published set whose name contains "mcp", and it is the strongest public evidence that the Klue MCP server authorizes over OAuth rather than only over a bearer API key.
  flows: []
  scope: stak_play_mcp:read
- description: Write/writeback scope for Klue's MCP surface. API Evangelist reading; matches Klue's claim of being the only competitive intelligence MCP server supporting writeback.
  flows: []
  scope: stak_play_mcp:edit
- description: SCIM 2.0 read. API Evangelist reading; the kluein GitHub organization maintains a fork of scimitar, a Rails SCIM v2 endpoint implementation.
  flows: []
  scope: scim:read
- description: SCIM 2.0 write (user/group provisioning). API Evangelist reading.
  flows: []
  scope: scim:edit
- description: Slack integration scope. API Evangelist reading.
  flows: []
  scope: slack
- description: Microsoft Teams integration scope. API Evangelist reading.
  flows: []
  scope: teams
- description: Generic connect/integration scope. API Evangelist reading.
  flows: []
  scope: connect
- description: Read access to usage reporting. API Evangelist reading.
  flows: []
  scope: usage_reports:read
- description: Service-to-service read scope. API Evangelist reading.
  flows: []
  scope: service_read
- description: Service-to-service write scope. API Evangelist reading.
  flows: []
  scope: service_write
- description: Internal customer-success scope. API Evangelist reading.
  flows: []
  scope: customer_success
- description: User-impersonation scope. API Evangelist reading; an internal/support capability, not expected to be grantable to customer integrations.
  flows: []
  scope: impersonate
- description: Read access to alpha/preview features. API Evangelist reading.
  flows: []
  scope: alpha:read
- description: Write access to alpha/preview features. API Evangelist reading.
  flows: []
  scope: alpha:edit
slug: klue-scopes
source_filename: klue-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://app.klue.com/.well-known/openid-configuration\ndocs: null\ndocs_note: >-\n  Klue publishes no public scopes / permissions reference page. The scope list\n  below is read verbatim from Klue's own OpenID Connect discovery document,\n  which app.klue.com serves anonymously at HTTP 200. Descriptions are NOT\n  published by Klue; where a description appears below it is marked as an\n  API Evangelist reading of the scope name and is not a Klue claim.\nscope_count: 23\nschemes:\n- name: klue-oauth2\n  type: oauth2\n  source: https://app.klue.com/.well-known/openid-configuration\n  issuer: https://app.klue.com\n  implementation_note: >-\n    The kluein GitHub organization maintains a fork of devise-doorkeeper\n    (https://github.com/kluein/devise-doorkeeper), the Rails Doorkeeper OAuth2\n    provider integration; the endpoint layout below matches a Doorkeeper\n    deployment.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://app.klue.com/oauth/authorize\n    tokenUrl: https://app.klue.com/oauth/token\n    refreshUrl: https://app.klue.com/oauth/token\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  endpoints:\n    authorization: https://app.klue.com/oauth/authorize\n    token: https://app.klue.com/oauth/token\n    revocation: https://app.klue.com/oauth/revoke\n    introspection: https://app.klue.com/oauth/introspect\n    userinfo: https://app.klue.com/oauth/userinfo\n    jwks: https://app.klue.com/oauth/discovery/keys\n    dynamic_client_registration: https://app.klue.com/oauth/register\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an RS256-signed ID token.\n  standard: OpenID Connect Core 1.0\n  sources: [well-known/klue-openid-configuration.json]\n- scope:\
  \ content:read\n  description: >-\n    Read access to Klue content (cards, battlecards). API Evangelist reading —\n    Klue publishes no description; the name aligns with the read surface of the\n    Klue Content API and the v1 MCP connector.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: content:edit\n  description: >-\n    Write access to Klue content. API Evangelist reading — aligns with the\n    create/update/delete card and battlecard tooling Klue describes as the\n    \"admin MCP endpoint\" writeback surface.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: win_loss:read\n  description: >-\n    Read access to win-loss interviews, transcripts and reports. API Evangelist\n    reading — aligns with the win-loss MCP tool family.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: deal_answers:read\n  description: >-\n    Read access to deal answers. API Evangelist reading — likely the Smart\n    Answers / Deal Tips surface.\n  sources:\
  \ [well-known/klue-openid-configuration.json]\n- scope: auto_insights:read\n  description: >-\n    Read access to Auto Insights, Klue's AI-generated insight pipeline.\n    API Evangelist reading; the v2 MCP connector exposes search_agent_insights.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: deal_context:read\n  description: Read access to deal context. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: transcript:edit\n  description: Write access to interview transcripts. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: crm:edit\n  description: >-\n    Write access to the connected CRM surface. API Evangelist reading; Klue\n    integrates with Salesforce, HubSpot and MS Dynamics.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: stak_play_mcp:read\n  description: >-\n    Read scope for Klue's MCP surface. API Evangelist reading — this is the only\n    scope in the published\
  \ set whose name contains \"mcp\", and it is the strongest\n    public evidence that the Klue MCP server authorizes over OAuth rather than\n    only over a bearer API key.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: stak_play_mcp:edit\n  description: >-\n    Write/writeback scope for Klue's MCP surface. API Evangelist reading; matches\n    Klue's claim of being the only competitive intelligence MCP server supporting\n    writeback.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: scim:read\n  description: >-\n    SCIM 2.0 read. API Evangelist reading; the kluein GitHub organization\n    maintains a fork of scimitar, a Rails SCIM v2 endpoint implementation.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: scim:edit\n  description: SCIM 2.0 write (user/group provisioning). API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: slack\n  description: Slack integration scope. API Evangelist reading.\n\
  \  sources: [well-known/klue-openid-configuration.json]\n- scope: teams\n  description: Microsoft Teams integration scope. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: connect\n  description: Generic connect/integration scope. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: usage_reports:read\n  description: Read access to usage reporting. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: service_read\n  description: Service-to-service read scope. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: service_write\n  description: Service-to-service write scope. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: customer_success\n  description: Internal customer-success scope. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: impersonate\n  description:\
  \ >-\n    User-impersonation scope. API Evangelist reading; an internal/support\n    capability, not expected to be grantable to customer integrations.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: alpha:read\n  description: Read access to alpha/preview features. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\n- scope: alpha:edit\n  description: Write access to alpha/preview features. API Evangelist reading.\n  sources: [well-known/klue-openid-configuration.json]\nx-evidence:\n- url: https://app.klue.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n  fetched: '2026-08-14'\n  file: well-known/klue-openid-configuration.json\n- url: https://app.klue.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json; charset=utf-8\n  fetched: '2026-08-14'\n  file: well-known/klue-oauth-authorization-server.json\n  note: byte-identical to the openid-configuration\
  \ document\nrelated:\n  authentication: authentication/klue-authentication.yml\n  mcp: mcp/klue-mcp.yml\n  well_known: well-known/klue-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klue/refs/heads/main/scopes/klue-scopes.yml
summary_line: 23 scopes · authorizationCode
tags:
- Company
- Software-as-a-Service
- Competitive Intelligence
- Competitive Enablement
- Sales Enablement
- Win-Loss Analysis
- Market Intelligence
- Battlecards
- Agents
- MCP
token_urls:
- https://app.klue.com/oauth/token
---
