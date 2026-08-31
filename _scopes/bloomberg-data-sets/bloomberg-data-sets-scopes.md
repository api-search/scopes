---
authorization_urls:
- https://login.bloomberg.com/api/oauth/authorize
description: Bloomberg publishes no OpenAPI and no public scopes reference page. The three scopes below are the complete scopes_supported array from the OIDC discovery document Bloomberg serves at www.bloomberg.com (identical to the one at login.bloomberg.com). Descriptions are NOT published by Bloomberg and are not invented here - each is marked undocumented.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bloomberg Data Sets Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bloomberg Data Sets publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bloomberg Data Sets API on a user''s behalf.


  Tokens are issued from https://login.bloomberg.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloomberg Data Sets
provider_slug: bloomberg-data-sets
schemes:
- flows:
  - authorizationUrl: https://login.bloomberg.com/api/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://login.bloomberg.com/api/oauth/token
  name: BloombergOIDC
  source: well-known/bloomberg-data-sets-openid-configuration.json
scope_count: 3
scope_names:
- openid
- user
- entitlements
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: user
- description: ''
  flows:
  - authorizationCode
  scope: entitlements
slug: bloomberg-data-sets-scopes
source_filename: bloomberg-data-sets-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://www.bloomberg.com/.well-known/openid-configuration\ndocs: null\ndescription: >-\n  Bloomberg publishes no OpenAPI and no public scopes reference page. The three scopes\n  below are the complete scopes_supported array from the OIDC discovery document\n  Bloomberg serves at www.bloomberg.com (identical to the one at login.bloomberg.com).\n  Descriptions are NOT published by Bloomberg and are not invented here - each is marked\n  undocumented.\nschemes:\n  - name: BloombergOIDC\n    source: well-known/bloomberg-data-sets-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.bloomberg.com/api/oauth/authorize\n        tokenUrl: https://login.bloomberg.com/api/oauth/token\n        code_challenge_methods: [S256]\nscopes:\n  - scope: openid\n    description: null\n    documented: false\n    note: Standard OIDC scope requesting an ID token. Bloomberg publishes no description.\n\
  \    flows: [authorizationCode]\n    sources: [well-known/bloomberg-data-sets-openid-configuration.json]\n  - scope: user\n    description: null\n    documented: false\n    note: Bloomberg publishes no description for this scope.\n    flows: [authorizationCode]\n    sources: [well-known/bloomberg-data-sets-openid-configuration.json]\n  - scope: entitlements\n    description: null\n    documented: false\n    note: >-\n      Bloomberg publishes no description for this scope. Named consistently with\n      Bloomberg's data-entitlement model, but no published definition was found and none\n      is asserted.\n    flows: [authorizationCode]\n    sources: [well-known/bloomberg-data-sets-openid-configuration.json]\nscope_count: 3\ngap: >-\n  The Data License / HAPI JWT surface at api.bloomberg.com/eap is a separate\n  authorization domain from this OIDC issuer and its scope or entitlement vocabulary is\n  not published anonymously. Reading it requires provisioned Enterprise Console\n  credentials.\n\
  maintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-data-sets/refs/heads/main/scopes/bloomberg-data-sets-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Analytics
- Datasets
- Financial-Services
- Market Data
- Reference Data
- Historical Data
- Financial Data
- Data Licensing
token_urls:
- https://login.bloomberg.com/api/oauth/token
---
