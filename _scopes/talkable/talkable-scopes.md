---
api_specs:
- filename: talkable-v2-openapi-original.yml
  format: yaml
  label: Talkable API v2
  slug: talkable-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/openapi/talkable-v2-openapi-original.yml
- filename: talkable-webhooks-openapi-original.yml
  format: yaml
  label: Talkable Webhooks
  slug: talkable-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/openapi/talkable-webhooks-openapi-original.yml
authorization_urls:
- https://www.talkable.com/oauth/authorize
description: ''
docs: https://docs.talkable.com/mcp_server/authentication/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Talkable Scopes
name_suffix: OAuth Scopes
note: 'OAuth scopes apply to the Talkable MCP server (OAuth 2.1), not the REST API v2 (which uses a Bearer API key). Scopes are a ceiling: a credential can still only do what the acting user''s Talkable role permits on each site.'
overview: 'Talkable publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Talkable API on a user''s behalf.


  Tokens are issued from https://www.talkable.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Talkable
provider_slug: talkable
schemes:
- flows:
  - authorizationUrl: https://www.talkable.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://www.talkable.com/oauth/register
    tokenUrl: https://www.talkable.com/oauth/token
  name: oauth2
  source: well-known/talkable-oauth-authorization-server.json
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- browser_control
scopes:
- description: Call MCP tools that read account and site data (list campaigns, look up a referral or person, read metrics).
  flows:
  - authorizationCode
  scope: mcp:read
- description: Call MCP tools that create or update Talkable data (approve a referral, expire a coupon, schedule an export).
  flows:
  - authorizationCode
  scope: mcp:write
- description: Advertised in the authorization-server metadata (scopes_supported); reserved for browser-control agent capabilities.
  flows:
  - authorizationCode
  scope: browser_control
slug: talkable-scopes
source_filename: talkable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: well-known/talkable-oauth-authorization-server.json\ndocs: https://docs.talkable.com/mcp_server/authentication/\nnote: >-\n  OAuth scopes apply to the Talkable MCP server (OAuth 2.1), not the REST API v2\n  (which uses a Bearer API key). Scopes are a ceiling: a credential can still\n  only do what the acting user's Talkable role permits on each site.\nschemes:\n  - name: oauth2\n    source: well-known/talkable-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.talkable.com/oauth/authorize\n        tokenUrl: https://www.talkable.com/oauth/token\n        registrationUrl: https://www.talkable.com/oauth/register\n        pkce: S256\nscopes:\n  - scope: mcp:read\n    description: Call MCP tools that read account and site data (list campaigns, look up a referral or person, read metrics).\n    flows: [authorizationCode]\n  - scope: mcp:write\n    description: Call MCP\
  \ tools that create or update Talkable data (approve a referral, expire a coupon, schedule an export).\n    flows: [authorizationCode]\n  - scope: browser_control\n    description: Advertised in the authorization-server metadata (scopes_supported); reserved for browser-control agent capabilities.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkable/refs/heads/main/scopes/talkable-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Referral Marketing
- Loyalty
- Marketing
- E-commerce
- Advocacy
- Rewards
- Customer Acquisition
- Webhooks
- MCP
token_urls:
- https://www.talkable.com/oauth/token
---
