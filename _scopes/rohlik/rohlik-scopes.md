---
authorization_urls:
- https://identity.rohlik.cz/oauth2/authorize
description: ''
docs: https://rohlik.cz/mcp-docs
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Rohlik Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rohlik publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rohlik API on a user''s behalf.


  Tokens are issued from https://identity.rohlik.cz/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rohlik
provider_slug: rohlik
schemes:
- flows:
  - authorizationUrl: https://identity.rohlik.cz/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://identity.rohlik.cz/oauth2/token
  name: RohlikOAuth2
  source: https://identity.rohlik.cz/.well-known/openid-configuration
scope_count: 3
scope_names:
- openid
- email
- roles
scopes:
- description: OpenID Connect authentication; issue an ID token for the signed-in Rohlik account.
  flows:
  - authorizationCode
  scope: openid
- description: Access the account's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the account's assigned roles claim.
  flows:
  - authorizationCode
  scope: roles
slug: rohlik-scopes
source_filename: rohlik-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://mcp.rohlik.cz/.well-known/oauth-protected-resource/mcp\ndocs: https://rohlik.cz/mcp-docs\nschemes:\n  - name: RohlikOAuth2\n    source: https://identity.rohlik.cz/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://identity.rohlik.cz/oauth2/authorize\n        tokenUrl: https://identity.rohlik.cz/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the signed-in Rohlik account.\n    flows: [authorizationCode]\n    sources: [https://mcp.rohlik.cz/.well-known/oauth-protected-resource/mcp]\n  - scope: email\n    description: Access the account's email address claim.\n    flows: [authorizationCode]\n    sources: [https://mcp.rohlik.cz/.well-known/oauth-protected-resource/mcp]\n  - scope: roles\n    description: Access the account's assigned roles claim.\n    flows: [authorizationCode]\n    sources: [https://mcp.rohlik.cz/.well-known/oauth-protected-resource/mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rohlik/refs/heads/main/scopes/rohlik-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Retail
- Grocery
- E-commerce
- Delivery
- Logistics
- MCP
- OAuth
- Europe
token_urls:
- https://identity.rohlik.cz/oauth2/token
---
