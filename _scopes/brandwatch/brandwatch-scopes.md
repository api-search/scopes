---
api_specs:
- filename: brandwatch-consumer-research-openapi.yml
  format: yaml
  label: Brandwatch Consumer Research API
  slug: consumer-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-consumer-research-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.brandwatch.com/docs/authenticate
flows:
- password
kind: oauth-scopes
layout: scope
method: searched
name: Brandwatch Scopes
name_suffix: OAuth Scopes
note: 'Brandwatch publishes no scope reference page. The three scope values below are the ones the provider''s own documented token response returns (`"scope": "read trust write"`), captured from the worked example on the Authentication page — they are observed, not documented. Brandwatch does not say what each grants, does not let a client request a subset at token-request time, and does not map any scope to any operation. The OpenAPI declares an oauth2 scheme with an empty `scopes` map and a placeholder `https://example.com/oauth2/token` token URL, so the spec contributes nothing here.'
overview: 'Brandwatch publishes 3 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brandwatch API on a user''s behalf.


  Tokens are issued from https://api.brandwatch.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brandwatch
provider_slug: brandwatch
schemes:
- flows:
  - flow: password
    grant_type: api-password
    tokenUrl: https://api.brandwatch.com/oauth/token
  name: oauth2-token-endpoint
  source: https://developers.brandwatch.com/docs/authenticate
scope_count: 3
scope_names:
- read
- trust
- write
scopes:
- description: ''
  flows:
  - password
  scope: read
- description: ''
  flows:
  - password
  scope: trust
- description: ''
  flows:
  - password
  scope: write
slug: brandwatch-scopes
source_filename: brandwatch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/brandwatch-consumer-research-openapi.yml\ndocs: https://developers.brandwatch.com/docs/authenticate\nnote: >-\n  Brandwatch publishes no scope reference page. The three scope values below are\n  the ones the provider's own documented token response returns\n  (`\"scope\": \"read trust write\"`), captured from the worked example on the\n  Authentication page — they are observed, not documented. Brandwatch does not\n  say what each grants, does not let a client request a subset at token-request\n  time, and does not map any scope to any operation. The OpenAPI declares an\n  oauth2 scheme with an empty `scopes` map and a placeholder\n  `https://example.com/oauth2/token` token URL, so the spec contributes nothing\n  here.\nschemes:\n  - name: oauth2-token-endpoint\n    source: https://developers.brandwatch.com/docs/authenticate\n    flows:\n      - flow: password\n        tokenUrl: https://api.brandwatch.com/oauth/token\n\
  \        grant_type: api-password\nscopes:\n  - scope: read\n    description: null\n    flows:\n      - password\n    sources:\n      - https://developers.brandwatch.com/docs/authenticate\n    note: returned in the documented token response; Brandwatch publishes no definition\n  - scope: trust\n    description: null\n    flows:\n      - password\n    sources:\n      - https://developers.brandwatch.com/docs/authenticate\n    note: returned in the documented token response; Brandwatch publishes no definition\n  - scope: write\n    description: null\n    flows:\n      - password\n    sources:\n      - https://developers.brandwatch.com/docs/authenticate\n    note: returned in the documented token response; Brandwatch publishes no definition\nscope_count: 3\nplatform_sso_scopes:\n  applies_to: Brandwatch One human sign-in — NOT the Consumer Research API\n  issuer: https://signin.brandwatch.com/auth/realms/bwone\n  discovery: https://signin.brandwatch.com/auth/realms/bwone/.well-known/openid-configuration\n\
  \  file: well-known/brandwatch-openid-configuration.json\n  method: probed\n  note: >-\n    Recorded for completeness and kept strictly separate from the API scopes\n    above. These are the scopes advertised by Brandwatch's Keycloak realm for\n    browser sign-in to the product suite. An API client cannot request them and\n    they do not appear on an API token. They are listed here because they show\n    Brandwatch already models product and tenancy boundaries as OIDC scopes\n    (ci = Consumer Intelligence, smm = Social Media Management) — the exact\n    structure the API's opaque three-value scope string lacks.\n  scopes:\n    - openid\n    - profile\n    - email\n    - phone\n    - address\n    - roles\n    - basic\n    - acr\n    - offline_access\n    - web-origins\n    - microprofile-jwt\n    - service_account\n    - ci\n    - ci-context\n    - smm\n    - smm-context\n    - bwone-account-id\n    - bwone-organization-id\n  scope_count: 18\nselectable: false\nselectable_note: >-\n\
  \  The token request accepts no `scope` parameter. Scopes are a property of the\n  underlying Consumer Research user account, so an agent cannot obtain a\n  read-only token for a read-only task.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/scopes/brandwatch-scopes.yml
summary_line: 3 scopes · password
tags:
- Analytics
- Social Media
- Social Media Monitoring
- Consumer Intelligence
- Brand Management
- Sentiment Analysis
token_urls:
- https://api.brandwatch.com/oauth/token
---
