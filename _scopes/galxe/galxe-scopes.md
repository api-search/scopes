---
authorization_urls:
- https://app.galxe.com/oauth
description: OAuth 2.0 scopes for "Sign in with Galxe" (Galxe ID). Each scope grants the requesting app read access to one class of the user's connected identity or wallet address. Requested at the authorization endpoint https://app.galxe.com/oauth and exchanged at https://api.galxe.com/oauth/auth/2/token.
docs: https://docs.galxe.com/galxe-id/galxe-id-integration/galxe-id-oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Galxe Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Galxe publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Galxe API on a user''s behalf.


  Tokens are issued from https://api.galxe.com/oauth/auth/2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Galxe
provider_slug: galxe
schemes:
- flows:
  - authorizationUrl: https://app.galxe.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.galxe.com/oauth/auth/2/token
  name: signInWithGalxe
  source: https://docs.galxe.com/galxe-id/galxe-id-integration/galxe-id-oauth
scope_count: 12
scope_names:
- Email
- Twitter
- Discord
- Github
- Telegram
- EVMAddress
- SolanaAddress
- SeiAddress
- AptosAddress
- InjectiveAddress
- FlowAddress
- GalxeID
scopes:
- description: Access the user's verified email address.
  flows:
  - authorizationCode
  scope: Email
- description: Access the user's connected Twitter/X account.
  flows:
  - authorizationCode
  scope: Twitter
- description: Access the user's connected Discord account.
  flows:
  - authorizationCode
  scope: Discord
- description: Access the user's connected GitHub account.
  flows:
  - authorizationCode
  scope: Github
- description: Access the user's connected Telegram account.
  flows:
  - authorizationCode
  scope: Telegram
- description: Access the user's connected EVM (Ethereum-compatible) wallet address.
  flows:
  - authorizationCode
  scope: EVMAddress
- description: Access the user's connected Solana wallet address.
  flows:
  - authorizationCode
  scope: SolanaAddress
- description: Access the user's connected Sei wallet address.
  flows:
  - authorizationCode
  scope: SeiAddress
- description: Access the user's connected Aptos wallet address.
  flows:
  - authorizationCode
  scope: AptosAddress
- description: Access the user's connected Injective wallet address.
  flows:
  - authorizationCode
  scope: InjectiveAddress
- description: Access the user's connected Flow wallet address.
  flows:
  - authorizationCode
  scope: FlowAddress
- description: Access the user's Galxe ID (universal Web3 identifier).
  flows:
  - authorizationCode
  scope: GalxeID
slug: galxe-scopes
source_filename: galxe-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.galxe.com/galxe-id/galxe-id-integration/galxe-id-oauth\ndocs: https://docs.galxe.com/galxe-id/galxe-id-integration/galxe-id-oauth\ndescription: >-\n  OAuth 2.0 scopes for \"Sign in with Galxe\" (Galxe ID). Each scope grants the\n  requesting app read access to one class of the user's connected identity or\n  wallet address. Requested at the authorization endpoint\n  https://app.galxe.com/oauth and exchanged at\n  https://api.galxe.com/oauth/auth/2/token.\nschemes:\n  - name: signInWithGalxe\n    source: https://docs.galxe.com/galxe-id/galxe-id-integration/galxe-id-oauth\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.galxe.com/oauth\n        tokenUrl: https://api.galxe.com/oauth/auth/2/token\nscopes:\n  - scope: Email\n    description: Access the user's verified email address.\n    flows: [authorizationCode]\n  - scope: Twitter\n    description: Access the user's connected Twitter/X\
  \ account.\n    flows: [authorizationCode]\n  - scope: Discord\n    description: Access the user's connected Discord account.\n    flows: [authorizationCode]\n  - scope: Github\n    description: Access the user's connected GitHub account.\n    flows: [authorizationCode]\n  - scope: Telegram\n    description: Access the user's connected Telegram account.\n    flows: [authorizationCode]\n  - scope: EVMAddress\n    description: Access the user's connected EVM (Ethereum-compatible) wallet address.\n    flows: [authorizationCode]\n  - scope: SolanaAddress\n    description: Access the user's connected Solana wallet address.\n    flows: [authorizationCode]\n  - scope: SeiAddress\n    description: Access the user's connected Sei wallet address.\n    flows: [authorizationCode]\n  - scope: AptosAddress\n    description: Access the user's connected Aptos wallet address.\n    flows: [authorizationCode]\n  - scope: InjectiveAddress\n    description: Access the user's connected Injective wallet address.\n\
  \    flows: [authorizationCode]\n  - scope: FlowAddress\n    description: Access the user's connected Flow wallet address.\n    flows: [authorizationCode]\n  - scope: GalxeID\n    description: Access the user's Galxe ID (universal Web3 identifier).\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galxe/refs/heads/main/scopes/galxe-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Company
- Crypto Web3
- Digital Identity
- Credentials
- Quests
- Loyalty
- GraphQL
- OAuth
- Blockchain
token_urls:
- https://api.galxe.com/oauth/auth/2/token
---
