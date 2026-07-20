---
api_specs:
- filename: brale-openapi-original.yml
  format: yaml
  label: Brale Issuance and Orchestration API
  slug: brale-issuance-and-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brale/refs/heads/main/openapi/brale-openapi-original.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Brale Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Brale publishes 20 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brale API on a user''s behalf.


  Tokens are issued from https://auth.brale.xyz/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brale
provider_slug: brale
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.brale.xyz/oauth2/token
  name: oauth
  source: openapi/brale-openapi-original.yml
scope_count: 20
scope_names:
- accounts:read
- accounts:write
- addresses:read
- addresses:write
- automations:read
- automations:write
- financial-institutions:read
- financial-institutions:write
- mints:write
- orders:read
- redemptions:write
- self_attested_tokens:burn
- self_attested_tokens:mint
- self_attested_tokens:read
- self_attested_tokens:transfer
- tokens:read
- transfers:read
- transfers:write
- webhooks:read
- webhooks:write
scopes:
- description: ''
  flows: []
  scope: accounts:read
- description: ''
  flows: []
  scope: accounts:write
- description: Read address details
  flows:
  - clientCredentials
  scope: addresses:read
- description: ''
  flows: []
  scope: addresses:write
- description: ''
  flows: []
  scope: automations:read
- description: ''
  flows: []
  scope: automations:write
- description: Read financial institution details
  flows:
  - clientCredentials
  scope: financial-institutions:read
- description: ''
  flows: []
  scope: financial-institutions:write
- description: Mint more of a specific token on chain
  flows:
  - clientCredentials
  scope: mints:write
- description: Read order details
  flows:
  - clientCredentials
  scope: orders:read
- description: Redeem/burn a particular token on a specific chain
  flows:
  - clientCredentials
  scope: redemptions:write
- description: Burn attested tokens (tokenization accounts only)
  flows:
  - clientCredentials
  scope: self_attested_tokens:burn
- description: Mint attested tokens (tokenization accounts only)
  flows:
  - clientCredentials
  scope: self_attested_tokens:mint
- description: ''
  flows: []
  scope: self_attested_tokens:read
- description: Transfer attested tokens (tokenization accounts only)
  flows:
  - clientCredentials
  scope: self_attested_tokens:transfer
- description: Read token details
  flows:
  - clientCredentials
  scope: tokens:read
- description: ''
  flows: []
  scope: transfers:read
- description: ''
  flows: []
  scope: transfers:write
- description: Read webhook subscriptions
  flows:
  - clientCredentials
  scope: webhooks:read
- description: Create and manage webhook subscriptions
  flows:
  - clientCredentials
  scope: webhooks:write
slug: brale-scopes
source_filename: brale-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/brale-openapi-original.yml\nschemes:\n- name: oauth\n  source: openapi/brale-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.brale.xyz/oauth2/token\nscopes:\n- scope: accounts:read\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: accounts:write\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: addresses:read\n  description: Read address details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: addresses:write\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: automations:read\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: automations:write\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: financial-institutions:read\n  description: Read financial institution details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: financial-institutions:write\n\
  \  sources:\n  - openapi/brale-openapi-original.yml\n- scope: mints:write\n  description: Mint more of a specific token on chain\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: orders:read\n  description: Read order details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: redemptions:write\n  description: Redeem/burn a particular token on a specific chain\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: self_attested_tokens:burn\n  description: Burn attested tokens (tokenization accounts only)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: self_attested_tokens:mint\n  description: Mint attested tokens (tokenization accounts only)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: self_attested_tokens:read\n  sources:\n  - openapi/brale-openapi-original.yml\n\
  - scope: self_attested_tokens:transfer\n  description: Transfer attested tokens (tokenization accounts only)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: tokens:read\n  description: Read token details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: transfers:read\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: transfers:write\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: webhooks:read\n  description: Read webhook subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n- scope: webhooks:write\n  description: Create and manage webhook subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brale-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brale/refs/heads/main/scopes/brale-scopes.yml
summary_line: 20 scopes · clientCredentials
tags:
- Company
- Stablecoins
- Stablecoin Issuance
- Payments
- Blockchain
- Cryptocurrency
- Fintech
- Financial Services
- Custody
- Tokenization
- On-Ramp
- Off-Ramp
token_urls:
- https://auth.brale.xyz/oauth2/token
---
