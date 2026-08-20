---
authorization_urls: []
description: ''
docs: https://help.motionapp.com/en/articles/14315735-motion-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Motion Scopes
name_suffix: OAuth Scopes
note: 'Read straight from Motion''s live RFC 8414 authorization-server metadata (HTTP 200) and its RFC 9728 protected-resource metadata. Motion publishes NO prose scopes/permissions reference page — the scope list below exists only as machine metadata on the authorization server. Descriptions marked `inferred: true` are our plain reading of the scope string and its OIDC/product context, not provider copy; nothing has been invented beyond what the strings themselves say. There is no OpenAPI to derive from, so derive-oauth-scopes.py was not run.'
overview: 'Motion publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Motion API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Motion
provider_slug: motion
schemes: []
scope_count: 11
scope_names:
- openid
- profile
- email
- offline_access
- documents:read
- documents:write
- runneth:documents:read
- runneth:documents:write
- runneth:mcp
- runneth:read
- runneth:write
scopes:
- description: Request an ID token — the OpenID Connect core scope.
  flows: []
  scope: openid
- description: Access the user's profile claims. The issuer advertises name, picture, family_name and given_name among claims_supported.
  flows: []
  scope: profile
- description: Access the user's email and email_verified claims.
  flows: []
  scope: email
- description: Issue a refresh token so the connected AI client can keep the session alive without re-prompting. Backed by the refresh_token grant advertised in grant_types_supported.
  flows: []
  scope: offline_access
- description: Read access to documents in the Motion app.
  flows: []
  scope: documents:read
- description: Write access to documents in the Motion app.
  flows: []
  scope: documents:write
- description: Read access to documents within Runneth by Motion, Motion's AI layer for marketing.
  flows: []
  scope: runneth:documents:read
- description: Write access to documents within Runneth by Motion.
  flows: []
  scope: runneth:documents:write
- description: Scope gating MCP access to the Runneth surface. Notable as the only scope string on the issuer that names MCP explicitly.
  flows: []
  scope: runneth:mcp
- description: General read access to Runneth by Motion.
  flows: []
  scope: runneth:read
- description: General write access to Runneth by Motion.
  flows: []
  scope: runneth:write
slug: motion-scopes
source_filename: motion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://projects.motionapp.com/.well-known/oauth-authorization-server\ndocs: https://help.motionapp.com/en/articles/14315735-motion-mcp\nname: Motion — OAuth scopes\nnote: >-\n  Read straight from Motion's live RFC 8414 authorization-server metadata (HTTP 200) and its RFC 9728\n  protected-resource metadata. Motion publishes NO prose scopes/permissions reference page — the\n  scope list below exists only as machine metadata on the authorization server. Descriptions marked\n  `inferred: true` are our plain reading of the scope string and its OIDC/product context, not\n  provider copy; nothing has been invented beyond what the strings themselves say. There is no\n  OpenAPI to derive from, so derive-oauth-scopes.py was not run.\nauthorization_server: https://projects.motionapp.com/api/auth\nprotected_resource: https://projects.motionapp.com/mcp\nscope_count: 11\nscopes_advertised_by_authorization_server: 11\nscopes_advertised_by_protected_resource:\
  \ 4\ndiscrepancy_note: >-\n  The MCP protected-resource document advertises only the four OIDC/session scopes\n  (openid, profile, email, offline_access). The authorization server advertises seven more —\n  documents:* and runneth:* — which belong to the wider Motion/Runneth app on the same issuer. An\n  MCP client should expect to be granted the four; the rest are the issuer's full surface.\nscopes:\n- scope: openid\n  standard: oidc\n  description: Request an ID token — the OpenID Connect core scope.\n  advertised_on:\n  - authorization-server\n  - protected-resource\n- scope: profile\n  standard: oidc\n  description: >-\n    Access the user's profile claims. The issuer advertises name, picture, family_name and given_name\n    among claims_supported.\n  advertised_on:\n  - authorization-server\n  - protected-resource\n- scope: email\n  standard: oidc\n  description: Access the user's email and email_verified claims.\n  advertised_on:\n  - authorization-server\n  - protected-resource\n\
  - scope: offline_access\n  standard: oidc\n  description: >-\n    Issue a refresh token so the connected AI client can keep the session alive without re-prompting.\n    Backed by the refresh_token grant advertised in grant_types_supported.\n  advertised_on:\n  - authorization-server\n  - protected-resource\n- scope: documents:read\n  description: Read access to documents in the Motion app.\n  inferred: true\n  advertised_on:\n  - authorization-server\n- scope: documents:write\n  description: Write access to documents in the Motion app.\n  inferred: true\n  advertised_on:\n  - authorization-server\n- scope: runneth:documents:read\n  description: Read access to documents within Runneth by Motion, Motion's AI layer for marketing.\n  inferred: true\n  advertised_on:\n  - authorization-server\n- scope: runneth:documents:write\n  description: Write access to documents within Runneth by Motion.\n  inferred: true\n  advertised_on:\n  - authorization-server\n- scope: runneth:mcp\n  description:\
  \ >-\n    Scope gating MCP access to the Runneth surface. Notable as the only scope string on the issuer\n    that names MCP explicitly.\n  inferred: true\n  advertised_on:\n  - authorization-server\n- scope: runneth:read\n  description: General read access to Runneth by Motion.\n  inferred: true\n  advertised_on:\n  - authorization-server\n- scope: runneth:write\n  description: General write access to Runneth by Motion.\n  inferred: true\n  advertised_on:\n  - authorization-server\nobservations:\n- >-\n  No scope in the published list maps to the Motion MCP's 13 creative-analytics tools. The MCP is\n  documented as read-only and authorizes on the user's existing Motion role (Owner/Admin/Collaborator)\n  rather than on a granular creative-analytics scope. A consumer therefore cannot narrow what an AI\n  client may read from their ad data below \"everything that user can see in Motion\".\n- >-\n  The read/write split exists on the documents:* and runneth:* families but not on the creative\n\
  \  analytics surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motion/refs/heads/main/scopes/motion-scopes.yml
summary_line: 11 scopes
tags:
- Company
- Creative Analytics
- Advertising
- Marketing Analytics
- Performance Marketing
- Ad Reporting
- Creative Strategy
- Software-as-a-Service
- MCP
- Agent Surface
token_urls: []
---
