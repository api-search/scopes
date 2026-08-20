---
api_specs:
- filename: bitski-activity-api-openapi.yml
  format: yaml
  label: Bitski activity API
  slug: bitski-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-activity-api-openapi.yml
- filename: bitski-commerce-api-openapi.yml
  format: yaml
  label: Bitski Commerce API
  slug: bitski-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-commerce-api-openapi.yml
- filename: bitski-droplinks-api-openapi.yml
  format: yaml
  label: Bitski Droplinks API
  slug: bitski-droplinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-droplinks-api-openapi.yml
- filename: bitski-minting-api-openapi.yml
  format: yaml
  label: Bitski Minting API
  slug: bitski-minting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-minting-api-openapi.yml
- filename: bitski-token-gating-api-openapi.yml
  format: yaml
  label: Bitski Token Gating API
  slug: bitski-token-gating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-token-gating-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bitski Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bitski publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bitski API on a user''s behalf.


  Tokens are issued from https://account.bitski.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bitski
provider_slug: bitski
schemes:
- description: Client credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.bitski.com/oauth2/token
  name: oauth2
  source: openapi/bitski-nft-service-openapi-original.json
scope_count: 2
scope_names:
- apps
- commerce
scopes:
- description: manage my applications
  flows:
  - clientCredentials
  scope: apps
- description: ''
  flows: []
  scope: commerce
slug: bitski-scopes
source_filename: bitski-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/bitski-nft-service-openapi-original.json\nschemes:\n- name: oauth2\n  source: openapi/bitski-nft-service-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.bitski.com/oauth2/token\n  description: Client credentials\nscopes:\n- scope: apps\n  description: manage my applications\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bitski-nft-service-openapi-original.json\n- scope: commerce\n  sources:\n  - openapi/bitski-nft-service-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/scopes/bitski-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Web3
- Crypto Wallet
- Wallet as a Service
- NFT
- Blockchain
- Authentication
- Payments
- Developer Tools
- Company
token_urls:
- https://account.bitski.com/oauth2/token
---
