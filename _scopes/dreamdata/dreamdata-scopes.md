---
authorization_urls:
- https://authenticate.dreamdata.io/oauth/2.1/authorize
- https://authenticate.dreamdata.io/propelauth/oauth/authorize
description: ''
docs: https://developer.dreamdata.io/mcp/mcp-server/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Dreamdata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dreamdata publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dreamdata API on a user''s behalf.


  Tokens are issued from https://authenticate.dreamdata.io/oauth/2.1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dreamdata
provider_slug: dreamdata
schemes:
- flows:
  - authorizationUrl: https://authenticate.dreamdata.io/oauth/2.1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://authenticate.dreamdata.io/oauth/2.1/token
  name: MCPOAuth21
  source: https://mcp.dreamdata.io/.well-known/oauth-authorization-server
- flows:
  - authorizationUrl: https://authenticate.dreamdata.io/propelauth/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://authenticate.dreamdata.io/propelauth/oauth/token
  name: OpenIDConnect
  source: https://authenticate.dreamdata.io/.well-known/openid-configuration
scope_count: 5
scope_names:
- read
- reports:write
- openid
- email
- profile
scopes:
- description: Read Dreamdata resources (reports, audiences, company journeys). Required consent for the MCP server.
  flows:
  - authorizationCode
  scope: read
- description: Save Dreamdata reports. Optional consent for the MCP server.
  flows:
  - authorizationCode
  scope: reports:write
- description: OpenID Connect sign-in (issue an ID token).
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Access basic profile claims (first_name, last_name, picture_url).
  flows:
  - authorizationCode
  scope: profile
slug: dreamdata-scopes
source_filename: dreamdata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://mcp.dreamdata.io/.well-known/oauth-authorization-server\ndocs: https://developer.dreamdata.io/mcp/mcp-server/\nschemes:\n- name: MCPOAuth21\n  source: https://mcp.dreamdata.io/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://authenticate.dreamdata.io/oauth/2.1/authorize\n    tokenUrl: https://authenticate.dreamdata.io/oauth/2.1/token\n- name: OpenIDConnect\n  source: https://authenticate.dreamdata.io/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authenticate.dreamdata.io/propelauth/oauth/authorize\n    tokenUrl: https://authenticate.dreamdata.io/propelauth/oauth/token\nscopes:\n- scope: read\n  description: Read Dreamdata resources (reports, audiences, company journeys). Required consent for the MCP server.\n  flows: [authorizationCode]\n  sources: [MCPOAuth21]\n- scope: reports:write\n\
  \  description: Save Dreamdata reports. Optional consent for the MCP server.\n  flows: [authorizationCode]\n  sources: [MCPOAuth21]\n- scope: openid\n  description: OpenID Connect sign-in (issue an ID token).\n  flows: [authorizationCode]\n  sources: [OpenIDConnect]\n- scope: email\n  description: Access the user's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [OpenIDConnect]\n- scope: profile\n  description: Access basic profile claims (first_name, last_name, picture_url).\n  flows: [authorizationCode]\n  sources: [OpenIDConnect]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamdata/refs/heads/main/scopes/dreamdata-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- B2B Attribution
- Revenue Attribution
- Marketing Analytics
- Customer Journey
- Event Tracking
- Audience Activation
- Analytics
- MCP
token_urls:
- https://authenticate.dreamdata.io/oauth/2.1/token
- https://authenticate.dreamdata.io/propelauth/oauth/token
---
