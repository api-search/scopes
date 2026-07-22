---
authorization_urls:
- https://qualified-tree-19-staging.authkit.app/oauth2/authorize
description: ''
docs: https://docs.watolabs.com/docs/connect-clients
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Wato Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wato publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wato API on a user''s behalf.


  Tokens are issued from https://qualified-tree-19-staging.authkit.app/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wato
provider_slug: wato
schemes:
- flows:
  - authorizationUrl: https://qualified-tree-19-staging.authkit.app/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://qualified-tree-19-staging.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://qualified-tree-19-staging.authkit.app/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://qualified-tree-19-staging.authkit.app/oauth2/token
  name: watoOAuth
  source: well-known/wato-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication (ID token issuance)
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Access to the user's basic profile claims
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Access to the user's email address claim
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issue a refresh token for long-lived MCP client sessions
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: wato-scopes
source_filename: wato-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://mesh.watolabs.com/.well-known/oauth-authorization-server\ndocs: https://docs.watolabs.com/docs/connect-clients\nnotes: >-\n  Scopes published as scopes_supported in the authorization server's RFC 8414\n  metadata (WorkOS AuthKit). These are identity/OIDC scopes — Wato does not\n  publish fine-grained API scopes; tool- and memory-level access is governed\n  server-side per team, role, and connector approval rather than via OAuth\n  scope strings (see conventions/wato-conventions.yml).\nschemes:\n- name: watoOAuth\n  source: well-known/wato-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://qualified-tree-19-staging.authkit.app/oauth2/authorize\n    tokenUrl: https://qualified-tree-19-staging.authkit.app/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://qualified-tree-19-staging.authkit.app/oauth2/device_authorization\n    tokenUrl: https://qualified-tree-19-staging.authkit.app/oauth2/token\n\
  scopes:\n- scope: openid\n  description: OpenID Connect authentication (ID token issuance)\n  flows: [authorizationCode, deviceCode]\n- scope: profile\n  description: Access to the user's basic profile claims\n  flows: [authorizationCode, deviceCode]\n- scope: email\n  description: Access to the user's email address claim\n  flows: [authorizationCode, deviceCode]\n- scope: offline_access\n  description: Issue a refresh token for long-lived MCP client sessions\n  flows: [authorizationCode, deviceCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wato/refs/heads/main/scopes/wato-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- Agent Governance
- Team Memory
- Connectors
- Agent Skills
- Automation
- Developer Tools
- Y Combinator
token_urls:
- https://qualified-tree-19-staging.authkit.app/oauth2/token
---
