---
authorization_urls:
- https://factory.macrofab.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Macrofab Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MacroFab publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MacroFab API on a user''s behalf.


  Tokens are issued from https://factory.macrofab.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MacroFab
provider_slug: macrofab
schemes:
- flows:
  - authorizationUrl: https://factory.macrofab.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://factory.macrofab.com/oauth/token
  name: OAuth2
  source: well-known/macrofab-openid-configuration.json
scope_count: 2
scope_names:
- openid
- email
scopes:
- description: OpenID Connect authentication (issue an ID token)
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated account's email address
  flows:
  - authorizationCode
  scope: email
slug: macrofab-scopes
source_filename: macrofab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://factory.macrofab.com/.well-known/openid-configuration\nnotes: >-\n  Scopes are taken from the scopes_supported field of MacroFab's live OpenID Connect\n  discovery document. The factory platform advertises only the standard OIDC scopes;\n  no product-specific permission scopes are published.\nschemes:\n  - name: OAuth2\n    source: well-known/macrofab-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://factory.macrofab.com/oauth/authorize\n        tokenUrl: https://factory.macrofab.com/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (issue an ID token)\n    flows: [authorizationCode]\n    sources: [well-known/macrofab-openid-configuration.json]\n  - scope: email\n    description: Access to the authenticated account's email address\n    flows: [authorizationCode]\n    sources: [well-known/macrofab-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macrofab/refs/heads/main/scopes/macrofab-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Hardware
- Electronics Manufacturing
- PCB Assembly
- Contract Manufacturing
- Supply Chain
- Manufacturing AI
- ITAR
token_urls:
- https://factory.macrofab.com/oauth/token
---
