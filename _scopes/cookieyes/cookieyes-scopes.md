---
authorization_urls:
- https://app.cookieyes.com/oauth2/auth
description: ''
docs: https://app.cookieyes.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cookieyes Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cookieyes publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cookieyes API on a user''s behalf.


  Tokens are issued from https://app.cookieyes.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cookieyes
provider_slug: cookieyes
schemes:
- flows:
  - authorizationUrl: https://app.cookieyes.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://app.cookieyes.com/oauth2/token
  name: OAuth2
  source: https://app.cookieyes.com/.well-known/oauth-authorization-server
scope_count: 5
scope_names:
- openid
- offline
- offline_access
- mcp:read
- mcp:write
scopes:
- description: Request an OpenID Connect ID token (authenticate the end user).
  flows:
  - authorizationCode
  scope: openid
- description: Request offline access (issue a refresh token).
  flows:
  - authorizationCode
  scope: offline
- description: OIDC offline_access — retain a refresh token for use without the user present.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read access to the CookieYes hosted MCP server (app.cookieyes.com/mcp).
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access to the CookieYes hosted MCP server (app.cookieyes.com/mcp).
  flows:
  - authorizationCode
  scope: mcp:write
slug: cookieyes-scopes
source_filename: cookieyes-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.cookieyes.com/.well-known/oauth-authorization-server\ndocs: https://app.cookieyes.com/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  source: https://app.cookieyes.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.cookieyes.com/oauth2/auth\n    tokenUrl: https://app.cookieyes.com/oauth2/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token (authenticate the end user).\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.cookieyes.com/.well-known/oauth-authorization-server\n- scope: offline\n  description: Request offline access (issue a refresh token).\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.cookieyes.com/.well-known/oauth-authorization-server\n- scope: offline_access\n  description: OIDC offline_access — retain a refresh token for use without the user present.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - https://app.cookieyes.com/.well-known/oauth-authorization-server\n- scope: mcp:read\n  description: Read access to the CookieYes hosted MCP server (app.cookieyes.com/mcp).\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.cookieyes.com/.well-known/oauth-protected-resource\n- scope: mcp:write\n  description: Write access to the CookieYes hosted MCP server (app.cookieyes.com/mcp).\n  flows:\n  - authorizationCode\n  sources:\n  - https://app.cookieyes.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cookieyes/refs/heads/main/scopes/cookieyes-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Consent Management
- Privacy
- GDPR
- CCPA
- Cookie Consent
- Compliance
- Data Protection
- MCP
token_urls:
- https://app.cookieyes.com/oauth2/token
---
