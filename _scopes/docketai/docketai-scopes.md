---
authorization_urls:
- https://angelic-precision-36.authkit.app/oauth2/authorize
description: ''
docs: https://help.docket.io/articles/8225942528-connect-docket-demand-mcp
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Docketai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Docket publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Docket API on a user''s behalf.


  Tokens are issued from https://angelic-precision-36.authkit.app/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Docket
provider_slug: docketai
schemes:
- flows:
  - authorizationUrl: https://angelic-precision-36.authkit.app/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://angelic-precision-36.authkit.app/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token
  issuer: https://angelic-precision-36.authkit.app
  name: DocketDemandMCPOAuth
  source: well-known/docketai-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token for the signing-in user.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Basic profile claims for the authorizing Docket user.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Email address claim for the authorizing Docket user.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issue a refresh token so the MCP client can keep the connection alive.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: docketai-scopes
source_filename: docketai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://demand-mcp.app.docketai.com/.well-known/oauth-authorization-server\ndocs: https://help.docket.io/articles/8225942528-connect-docket-demand-mcp\n\n# Read from live RFC 8414 / RFC 9728 metadata. Docket publishes no scopes or\n# permissions reference page; the scopes below are the OIDC/AuthKit baseline the\n# authorization server advertises, not a Docket product-permission vocabulary.\n\nschemes:\n  - name: DocketDemandMCPOAuth\n    source: well-known/docketai-oauth-authorization-server.json\n    issuer: https://angelic-precision-36.authkit.app\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://angelic-precision-36.authkit.app/oauth2/authorize\n        tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://angelic-precision-36.authkit.app/oauth2/device_authorization\n        tokenUrl: https://angelic-precision-36.authkit.app/oauth2/token\n\
  \nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the signing-in user.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/docketai-oauth-authorization-server.json]\n  - scope: profile\n    description: Basic profile claims for the authorizing Docket user.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/docketai-oauth-authorization-server.json]\n  - scope: email\n    description: Email address claim for the authorizing Docket user.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/docketai-oauth-authorization-server.json]\n  - scope: offline_access\n    description: Issue a refresh token so the MCP client can keep the connection alive.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/docketai-oauth-authorization-server.json]\n\nresource_scopes:\n  resource: https://demand-mcp.app.docketai.com/mcp\n  scopes_supported: []\n  note: >-\n    The RFC 9728 protected-resource\
  \ document declares an EMPTY scopes_supported array.\n    Docket therefore performs no scope-based authorization at the MCP resource; access\n    is bounded entirely by the authorizing user's Docket workspace role, and the whole\n    server is read-only. An integrator cannot request or reason about a narrower grant.\n\nx-evidence:\n  - url: https://demand-mcp.app.docketai.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://demand-mcp.app.docketai.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docketai/refs/heads/main/scopes/docketai-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Company
- AI Agents
- Agentic Marketing
- Sales Enablement
- Demand Generation
- Marketing Automation
- Conversational AI
- Lead Qualification
- Go-To-Market
- MCP
- Model Context Protocol
token_urls:
- https://angelic-precision-36.authkit.app/oauth2/token
---
