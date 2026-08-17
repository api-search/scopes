---
authorization_urls:
- https://mcp.eu.adverity.com/authorize
description: ''
docs: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Adverity Scopes
name_suffix: OAuth Scopes
note: 'The nine strings in verbatim_scope_strings were read directly out of the published Adverity documentation pages. The remaining entries are the documented UI permission families (Workspace Write, Monitor, User) whose literal scope strings do not appear in the docs; they are flagged spec_string_observed: false rather than being asserted as verbatim. Nothing here is invented.'
overview: 'Adverity uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://mcp.eu.adverity.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adverity
provider_slug: adverity
schemes:
- name: ManagementApiKeyPermissions
  note: Set per key at creation time in Administration > Management API keys. Keys are assigned to one workspace and grant access to that workspace and its child workspaces. Maximum 5 keys per workspace; creation requires Administrator permissions in the root workspace.
  source: docs
  type: apiKey
- flows:
  - authorizationUrl: https://mcp.eu.adverity.com/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    note: scopes_supported is [] in the protected-resource metadata; no OAuth scopes are advertised.
    pkce: S256
    registrationUrl: https://mcp.eu.adverity.com/register
    scopes: {}
    tokenUrl: https://mcp.eu.adverity.com/token
  name: AdverityMcpOAuth
  source: https://mcp.eu.adverity.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 0
scope_names: []
scopes: []
slug: adverity-scopes
source_filename: adverity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\ndocs: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\nsummary: >-\n  Adverity has two distinct scope surfaces. (1) Management API keys generated in the\n  Adverity Administration UI carry per-resource PERMISSIONS set to No access, Read-only, or\n  Write; the v1 and v2 endpoint surfaces enforce them as explicit scope strings of the form\n  <resource>:read / <resource>:write. (2) The remote MCP server runs a real OAuth 2.0\n  authorization server (RFC 8414 + RFC 7591 dynamic client registration, PKCE S256) whose\n  published metadata declares an EMPTY scopes_supported array — the OAuth layer carries no\n  scopes of its own, and effective authority comes from the MAPI key the user supplies at\n  the Adverity sign-in step. There is no OAuth2 on the Management API itself.\nschemes:\n- name: ManagementApiKeyPermissions\n\
  \  type: apiKey\n  source: docs\n  note: >-\n    Set per key at creation time in Administration > Management API keys. Keys are assigned\n    to one workspace and grant access to that workspace and its child workspaces. Maximum\n    5 keys per workspace; creation requires Administrator permissions in the root\n    workspace.\n- name: AdverityMcpOAuth\n  type: oauth2\n  source: https://mcp.eu.adverity.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.eu.adverity.com/authorize\n    tokenUrl: https://mcp.eu.adverity.com/token\n    registrationUrl: https://mcp.eu.adverity.com/register\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    scopes: {}\n    note: scopes_supported is [] in the protected-resource metadata; no OAuth scopes are advertised.\nscopes:\n- name: workspace:read\n  resource: Workspace\n  level: read\n  description: >-\n    Permissions equivalent to the Viewer user group across the key's\
  \ workspace and its\n    children.\n  evidence: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\n- name: workspace:write\n  resource: Workspace\n  level: write\n  description: >-\n    Permissions equivalent to the Datastream Manager user group; also allows creating and\n    updating workspaces through the Management API. Deleting a workspace is NOT covered —\n    the owning user must have Administrator permissions in the root workspace.\n  evidence: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\n  spec_string_observed: false\n  note: Documented as the Workspace \"Write\" permission; the literal string is inferred from the workspace:read pattern and is not quoted verbatim in the docs.\n- name: authorization:read\n  resource: Authorization\n  level: read\n  description: >-\n    Read which accounts an authorization is permitted to collect from, and discover\n    available accounts, profiles, and campaigns.\n  evidence:\
  \ https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\n- name: authorization:write\n  resource: Authorization\n  level: write\n  description: Update the set of accounts an authorization is permitted to collect from.\n  evidence: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\n  spec_string_observed: false\n- name: datastream:read\n  resource: Datastream\n  level: read\n  description: List datastreams and retrieve their configuration, including the connector field hierarchy.\n  evidence: https://docs.adverity.com/guides/management-api/managing-datastreams-smart-schedule.html\n- name: datastream:write\n  resource: Datastream\n  level: write\n  description: Update datastream configuration, including smart schedule and pulling-mode settings on the v1/v2 surfaces.\n  evidence: https://docs.adverity.com/guides/management-api/managing-datastreams-smart-schedule.html\n- name: destination:read\n  resource: Destination\n  level:\
  \ read\n  description: Read destination (Target) configuration and datastream-to-destination bindings.\n  evidence: https://docs.adverity.com/guides/management-api/listing-datastream-destination-bindings.html\n- name: destination:write\n  resource: Destination\n  level: write\n  description: >-\n    Create, update, and delete destinations, and requeue extracts. Assignable only at the\n    root workspace level.\n  evidence: https://docs.adverity.com/guides/management-api/requeueing-extracts.html\n- name: transformations:read\n  resource: Transformation\n  level: read\n  description: List and retrieve transformations (Transformers).\n  evidence: https://docs.adverity.com/guides/management-api/creating-editing-transformations.html\n- name: transformations:write\n  resource: Transformation\n  level: write\n  description: Create, edit, and delete transformations.\n  evidence: https://docs.adverity.com/guides/management-api/creating-editing-transformations.html\n- name: usage:read\n  resource:\
  \ Usage\n  level: read\n  description: Retrieve row-usage and billing metrics through the Management API.\n  evidence: https://docs.adverity.com/guides/management-api/viewing-usage-metrics.html\n- name: monitor:read\n  resource: Monitor\n  level: read\n  description: Discover custom monitors available for assignment through the Management API.\n  evidence: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\n  spec_string_observed: false\n  note: Documented as the Monitor \"Read-only\" permission; literal scope string not quoted in the docs.\n- name: monitor:write\n  resource: Monitor\n  level: write\n  description: Assign or unassign custom monitors through the Management API.\n  evidence: https://docs.adverity.com/guides/management-api/bulk-assigning-custom-monitors.html\n  spec_string_observed: false\n- name: user:write\n  resource: User\n  level: write\n  description: >-\n    Access user-management endpoints (root workspace level only, and only for keys\n\
  \    generated in the Adverity user interface), and create, update, and delete notification\n    subscriptions. Notification-subscription writes also work with a key minted from user\n    credentials; subscriptions created that way are owned by the issuing user.\n  evidence: https://docs.adverity.com/guides/management-api/authorizing-to-management-api.html\n  spec_string_observed: false\nscope_count: 14\nverbatim_scope_strings:\n- authorization:read\n- datastream:read\n- datastream:write\n- destination:read\n- destination:write\n- transformations:read\n- transformations:write\n- usage:read\n- workspace:read\nnote: >-\n  The nine strings in verbatim_scope_strings were read directly out of the published\n  Adverity documentation pages. The remaining entries are the documented UI permission\n  families (Workspace Write, Monitor, User) whose literal scope strings do not appear in\n  the docs; they are flagged spec_string_observed: false rather than being asserted as\n  verbatim. Nothing here\
  \ is invented.\nrelated:\n- authentication/adverity-authentication.yml\n- mcp/adverity-mcp.yml\n- well-known/adverity-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adverity/refs/heads/main/scopes/adverity-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Data Analytics
- Marketing Analytics
- Data Integration
- ETL
- Business Intelligence
- Marketing Intelligence
- MCP
token_urls:
- https://mcp.eu.adverity.com/token
---
