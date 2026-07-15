---
authorization_urls: []
description: Checkout.com's OAuth 2.0 client-credentials scopes. Server-to-server clients POST access_key_id:access_key_secret (HTTP Basic) with grant_type=client_credentials to the /connect/token endpoint and receive a JWT Bearer access token. Tokens expire after four hours and should be cached and reused. Scopes may be omitted (the default scopes assigned to the access key apply) and any requested scopes must be a subset of those assigned to the key. Upgrades the earlier derived file with the searched token flow and the fx scope observed in the docs' token response example.
docs: https://www.checkout.com/docs/developer-resources/api/manage-api-keys/oauth-2-0-client-credentials
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Checkout Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Checkout.com publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Checkout.com API on a user''s behalf.


  Tokens are issued from https://access.checkout.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Checkout.com
provider_slug: checkout-com
schemes:
- description: OAuth 2.0 client-credentials flow for server-to-server authentication.
  flows:
  - flow: clientCredentials
    sandboxTokenUrl: https://{prefix}.access.sandbox.checkout.com/connect/token
    tokenUrl: https://access.checkout.com/connect/token
  grant_types:
  - client_credentials
  name: OAuth2
  source: openapi/checkout-com-openapi.yml
  token_ttl_hours: 4
  token_type: Bearer (JWT)
  type: oauth2
scope_count: 3
scope_names:
- gateway
- vault
- fx
scopes:
- description: Access to all Gateway resources (payments and payment actions).
  flows:
  - clientCredentials
  scope: gateway
- description: Access to all Vault resources (tokenization and stored instruments).
  flows:
  - clientCredentials
  scope: vault
- description: Access to Forex (FX) rate resources; observed in the token response example ("scope":"fx gateway vault").
  flows:
  - clientCredentials
  scope: fx
slug: checkout-com-scopes
source_filename: checkout-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nsource: https://www.checkout.com/docs/developer-resources/api/manage-api-keys/oauth-2-0-client-credentials\ndocs: https://www.checkout.com/docs/developer-resources/api/manage-api-keys/oauth-2-0-client-credentials\ndescription: >-\n  Checkout.com's OAuth 2.0 client-credentials scopes. Server-to-server clients\n  POST access_key_id:access_key_secret (HTTP Basic) with grant_type=client_credentials\n  to the /connect/token endpoint and receive a JWT Bearer access token. Tokens\n  expire after four hours and should be cached and reused. Scopes may be omitted\n  (the default scopes assigned to the access key apply) and any requested scopes\n  must be a subset of those assigned to the key. Upgrades the earlier derived\n  file with the searched token flow and the fx scope observed in the docs' token\n  response example.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    source: openapi/checkout-com-openapi.yml\n    flows:\n      - flow: clientCredentials\n\
  \        tokenUrl: https://access.checkout.com/connect/token\n        sandboxTokenUrl: https://{prefix}.access.sandbox.checkout.com/connect/token\n    grant_types: [client_credentials]\n    token_type: Bearer (JWT)\n    token_ttl_hours: 4\n    description: OAuth 2.0 client-credentials flow for server-to-server authentication.\nscopes:\n  - scope: gateway\n    description: Access to all Gateway resources (payments and payment actions).\n    flows: [clientCredentials]\n    sources: [openapi/checkout-com-openapi.yml, docs]\n  - scope: vault\n    description: Access to all Vault resources (tokenization and stored instruments).\n    flows: [clientCredentials]\n    sources: [openapi/checkout-com-openapi.yml, docs]\n  - scope: fx\n    description: Access to Forex (FX) rate resources; observed in the token response example (\"scope\":\"fx gateway vault\").\n    flows: [clientCredentials]\n    sources: [docs]\nnotes: >-\n  The docs indicate more granular sub-scopes (e.g. gateway:payment,\n  vault:instruments)\
  \ can be assigned to an access key, but the granular scope\n  table is not rendered in the static docs and is therefore not enumerated here\n  to avoid fabrication. Assign least-privilege scopes when creating an access key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/scopes/checkout-com-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Fintech
- Payments
- Cards
- Acquiring
- Cross-Border
token_urls:
- https://access.checkout.com/connect/token
---
