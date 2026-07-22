---
authorization_urls:
- https://login.stilla.ai/oauth2/authorize
description: ''
docs: https://login.stilla.ai/.well-known/openid-configuration
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Stilla Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Stilla publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Stilla API on a user''s behalf.


  Tokens are issued from https://login.stilla.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stilla
provider_slug: stilla
schemes:
- flows:
  - authorizationUrl: https://login.stilla.ai/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.stilla.ai/oauth2/token
  - deviceAuthorizationUrl: https://login.stilla.ai/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://login.stilla.ai/oauth2/token
  issuer: https://login.stilla.ai
  name: OAuth2
  source: https://api.stilla.ai/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Access the user's email address.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: stilla-scopes
source_filename: stilla-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.stilla.ai/.well-known/oauth-authorization-server\ndocs: https://login.stilla.ai/.well-known/openid-configuration\nschemes:\n  - name: OAuth2\n    source: https://api.stilla.ai/.well-known/oauth-authorization-server\n    issuer: https://login.stilla.ai\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.stilla.ai/oauth2/authorize\n        tokenUrl: https://login.stilla.ai/oauth2/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://login.stilla.ai/oauth2/device_authorization\n        tokenUrl: https://login.stilla.ai/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token.\n    flows: [authorizationCode, deviceCode]\n  - scope: profile\n    description: Access the user's basic profile claims.\n    flows: [authorizationCode, deviceCode]\n  - scope: email\n    description: Access the user's email address.\n    flows:\
  \ [authorizationCode, deviceCode]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived access.\n    flows: [authorizationCode, deviceCode]\nnotes: >-\n  Scopes are the standard OIDC set advertised by the WorkOS AuthKit authorization server\n  (login.stilla.ai). The MCP protected-resource metadata declares an empty\n  scopes_supported list, i.e. MCP access is authorized at the resource level rather than\n  via granular API scopes. No product-specific permission scopes are published at the\n  authorization-server level.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stilla/refs/heads/main/scopes/stilla-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic
- Productivity
- Collaboration
- MCP
- Automation
- Developer Tools
- Enterprise
token_urls:
- https://login.stilla.ai/oauth2/token
---
