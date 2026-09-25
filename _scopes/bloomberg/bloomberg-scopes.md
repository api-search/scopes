---
api_specs:
- filename: bloomberg-reference-data-api-openapi.yml
  format: yaml
  label: Bloomberg BLPAPI Core
  slug: bloomberg-blpapi-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg/refs/heads/main/openapi/bloomberg-reference-data-api-openapi.yml
authorization_urls:
- https://login.bloomberg.com/api/oauth/authorize
description: ''
docs: https://www.bloomberg.com/.well-known/openid-configuration
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Bloomberg Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bloomberg publishes 3 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bloomberg API on a user''s behalf.


  Tokens are issued from https://login.bloomberg.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloomberg
provider_slug: bloomberg
schemes:
- flows:
  - authorizationUrl: https://login.bloomberg.com/api/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://login.bloomberg.com/api/oauth/token
  - flow: refreshToken
    tokenUrl: https://login.bloomberg.com/api/oauth/token
  issuer: https://www.bloomberg.com
  name: BloombergOAuth
  source: https://www.bloomberg.com/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- openid
- user
- entitlements
scopes:
- description: OpenID Connect authentication — issues an RS256-signed ID token for the Bloomberg identity.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated Bloomberg user profile.
  flows:
  - authorizationCode
  scope: user
- description: Access to the user's Bloomberg product/data entitlements.
  flows:
  - authorizationCode
  scope: entitlements
slug: bloomberg-scopes
source_filename: bloomberg-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://www.bloomberg.com/.well-known/oauth-authorization-server\ndocs: https://www.bloomberg.com/.well-known/openid-configuration\nnotes: >-\n  Bloomberg's BLPAPI OpenAPI projections declare no oauth2 securitySchemes (BLPAPI uses SDK\n  session/identity authorization). These scopes come from Bloomberg's published OAuth 2.0 /\n  OIDC authorization-server discovery metadata (endpoints on login.bloomberg.com), which fronts\n  Bloomberg web/console login and token issuance for HTTP-delivered services.\nschemes:\n  - name: BloombergOAuth\n    source: https://www.bloomberg.com/.well-known/oauth-authorization-server\n    issuer: https://www.bloomberg.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.bloomberg.com/api/oauth/authorize\n        tokenUrl: https://login.bloomberg.com/api/oauth/token\n        pkce: S256\n      - flow: refreshToken\n        tokenUrl: https://login.bloomberg.com/api/oauth/token\n\
  scopes:\n  - scope: openid\n    description: OpenID Connect authentication — issues an RS256-signed ID token for the Bloomberg identity.\n    flows: [authorizationCode]\n    sources: [https://www.bloomberg.com/.well-known/oauth-authorization-server]\n  - scope: user\n    description: Access to the authenticated Bloomberg user profile.\n    flows: [authorizationCode]\n    sources: [https://www.bloomberg.com/.well-known/oauth-authorization-server]\n  - scope: entitlements\n    description: Access to the user's Bloomberg product/data entitlements.\n    flows: [authorizationCode]\n    sources: [https://www.bloomberg.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg/refs/heads/main/scopes/bloomberg-scopes.yml
summary_line: 3 scopes · authorizationCode/refreshToken
tags:
- Analytics
- Business Intelligence
- Data License
- Enterprise
- Execution Management
- Financial Services
- Market Data
- News
- Quantitative Analysis
- Trading
- Transaction Cost Analysis
token_urls:
- https://login.bloomberg.com/api/oauth/token
---
