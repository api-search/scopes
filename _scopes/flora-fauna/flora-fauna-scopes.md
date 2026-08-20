---
api_specs:
- filename: flora-fauna-flora-api-openapi.yml
  format: yaml
  label: Flora.ai API
  slug: flora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-flora-api-openapi.yml
authorization_urls: []
description: 'FLORA publishes OAuth on two hosts and a scope vocabulary on only one of them, and neither vocabulary governs the REST API. This artifact records the real shape rather than manufacturing a scope list: the REST API is workspace-wide bearer-key auth with no scopes at all, the MCP authorization server omits scopes_supported entirely and delegates authorization to the signed-in user''s existing FLORA role, and the only enumerated scopes anywhere on a FLORA host are the Clerk platform scopes behind application sign-in.'
docs: https://developer.flora.ai/mcp/authentication
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Flora Fauna Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FLORA uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FLORA
provider_slug: flora-fauna
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: flora-fauna-scopes
source_filename: flora-fauna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  Live probes of https://agents.flora.ai/.well-known/oauth-authorization-server\n  (HTTP 200) and https://app.florafauna.ai/.well-known/openid-configuration\n  (HTTP 200), plus https://developer.flora.ai/mcp/authentication and\n  https://developer.flora.ai/platform/authentication. Also derived against\n  openapi/flora-fauna-flora-api-openapi.yml, which declares no oauth2 scheme.\ndocs: https://developer.flora.ai/mcp/authentication\ndescription: >-\n  FLORA publishes OAuth on two hosts and a scope vocabulary on only one of them,\n  and neither vocabulary governs the REST API. This artifact records the real\n  shape rather than manufacturing a scope list: the REST API is workspace-wide\n  bearer-key auth with no scopes at all, the MCP authorization server omits\n  scopes_supported entirely and delegates authorization to the signed-in user's\n  existing FLORA role, and the only enumerated scopes anywhere on a FLORA host\n  are\
  \ the Clerk platform scopes behind application sign-in.\nsurfaces:\n  - surface: REST API\n    base_url: https://app.flora.ai/api/v1\n    auth: http bearer (sk_live_)\n    oauth2: false\n    scope_count: 0\n    note: >-\n      An API key inherits the whole workspace. There is no scope, no read-only\n      key type, and no per-resource restriction — the blast radius of a leaked\n      key is every Technique, Project, Asset and billed run in that workspace.\n  - surface: MCP server\n    base_url: https://agents.flora.ai/mcp\n    auth: OAuth 2.1 + PKCE\n    oauth2: true\n    scope_count: 0\n    scopes_supported_published: false\n    evidence:\n      url: https://agents.flora.ai/.well-known/oauth-authorization-server\n      status: 200\n      finding: >-\n        The RFC 8414 document carries issuer, authorization/token/registration/\n        revocation endpoints, grant types, auth methods and PKCE methods — but no\n        scopes_supported member. A client therefore cannot request least-privilege\n\
  \        access; it takes whatever the user already has.\n    documented_authorization_model:\n      basis: the signed-in FLORA user's role in the connected workspace\n      granted_by_default:\n        - List and read Techniques, Projects, Workspaces, Assets, Models\n        - Create runs (billed in USD to the workspace)\n        - Upload assets\n      conditional:\n        - Create or modify Projects — only if the user's FLORA role allows it\n      never_granted:\n        - Manage billing\n        - Manage workspace members\n      denial_error: 403 forbidden\n  - surface: FLORA application sign-in\n    base_url: https://app.florafauna.ai\n    auth: OpenID Connect (Clerk, issuer https://clerk.flora.ai)\n    oauth2: true\n    scope_count: 6\n    evidence:\n      url: https://app.florafauna.ai/.well-known/openid-configuration\n      status: 200\n    scopes:\n      - {name: openid, description: 'OIDC: request an ID token.'}\n      - {name: profile, description: 'OIDC: basic profile claims\
  \ (name, preferred_username, picture).'}\n      - {name: email, description: 'OIDC: email and email_verified claims.'}\n      - {name: offline_access, description: 'OIDC: issue a refresh token.'}\n      - {name: public_metadata, description: 'Clerk: read the user''s public metadata object.'}\n      - {name: private_metadata, description: 'Clerk: read the user''s private metadata object.'}\n    note: >-\n      These are Clerk's scoped-access vocabulary (the document links\n      https://clerk.com/docs/oauth/scoped-access), not FLORA API permissions.\n      Recorded for completeness; do not read them as API authorization.\nsummary:\n  api_scope_count: 0\n  mcp_scope_count: 0\n  application_oidc_scope_count: 6\n  finding: >-\n    Neither callable FLORA surface publishes a scope vocabulary. The gap that\n    matters most is the MCP one: a code-execution server whose single `execute`\n    tool can spend real money on the user's workspace, granted with no scope\n    negotiation at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/scopes/flora-fauna-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Creative AI
- Generative AI
- Infinite Canvas
- Node-Based Workflows
- Creative Workspace
- Image-Generation
- Video Generation
- Text-to-Image
- Text-to-Video
- AI Agents
- Multimodal AI
- Design Tools
- Creative Professionals
- Advertising
- Film
- Fashion
- Branding
- VFX
- Photography
- Architecture
- Motion Design
- FAUNA
- MCP
- Agent Tools
- Workflow-Automation
token_urls: []
---
