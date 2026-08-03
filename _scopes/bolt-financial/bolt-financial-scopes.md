---
api_specs:
- filename: bolt-financial-bolt-api-openapi.yml
  format: yaml
  label: Bolt API
  slug: bolt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-bolt-api-openapi.yml
- filename: bolt-financial-embeddable-checkout-v1-openapi.yml
  format: yaml
  label: Bolt Embeddable Checkout v1 API
  slug: embeddable-checkout-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-embeddable-checkout-v1-openapi.yml
- filename: bolt-financial-embeddable-checkout-v3-openapi.yml
  format: yaml
  label: Bolt Embeddable Checkout v3 API
  slug: embeddable-checkout-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-embeddable-checkout-v3-openapi.yml
- filename: bolt-financial-tokenizer-openapi.yml
  format: yaml
  label: Bolt Tokenizer API
  slug: tokenizer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-tokenizer-openapi.yml
authorization_urls:
- https://api.boltapp.com/v1/oauth/authorize
- /v1/oauth/authorize
description: ''
docs: https://help.boltapp.com/developers/bolt-oauth/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Bolt Financial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bolt Financial publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bolt Financial API on a user''s behalf.


  Tokens are issued from https://api.boltapp.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bolt Financial
provider_slug: bolt-financial
schemes:
- description: 'Bolt utilizes the OAuth flow that developers can use to attain access to Bolt Account data via APIs.

    For all APIs that require authorization, please provide your `access_token` returned from `/v1/oauth/token` via the basic auth bearer header `Authorization: bearer ${TOKEN}`.

    [Read more about the OAuth token endpoint.](/api-bolt/#tag/OAuth)'
  flows:
  - authorizationUrl: https://api.boltapp.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.boltapp.com/v1/oauth/token
  name: OAuth
  source: openapi/bolt-financial-bolt-api-openapi.yml
- description: 'Bolt utilizes the OAuth flow that developers can use to attain access to Bolt Account data via APIs.

    For all APIs that require authorization, please provide your `access_token` returned from `/v1/oauth/token` via the basic auth bearer header `Authorization: bearer ${TOKEN}`.

    [Read more about the OAuth token endpoint.](/api-bolt/#tag/OAuth)'
  flows:
  - authorizationUrl: https://api.boltapp.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.boltapp.com/v1/oauth/token
  name: OAuth
  source: openapi/bolt-financial-embeddable-checkout-v1-openapi.yml
- flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: /v1/oauth/token
  name: oauth
  source: openapi/bolt-financial-embeddable-checkout-v3-openapi.yml
scope_count: 4
scope_names:
- bolt.account.manage
- bolt.account.view
- openid
- email
scopes:
- description: This scope grants permissions to perform read/edit/delete actions on Bolt Account data
  flows:
  - authorizationCode
  scope: bolt.account.manage
- description: This scope grants permissions to perform read only actions on Bolt Account data
  flows:
  - authorizationCode
  scope: bolt.account.view
- description: This scope grants permissions that enable Bolt SSO by granting an id token JWT that stores account data. Not used in v1/account endpoints
  flows:
  - authorizationCode
  scope: openid
- description: Advertised by the Bolt OIDC discovery document; not declared in any published OpenAPI security scheme.
  flows:
  - authorizationCode
  scope: email
slug: bolt-financial-scopes
source_filename: bolt-financial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\ndocs: https://help.boltapp.com/developers/bolt-oauth/\ndiscovery: https://api.boltapp.com/.well-known/openid-configuration\nsource: openapi/bolt-financial-bolt-api-openapi.yml, openapi/bolt-financial-embeddable-checkout-v1-openapi.yml,\n  openapi/bolt-financial-embeddable-checkout-v3-openapi.yml\nschemes:\n- name: OAuth\n  source: openapi/bolt-financial-bolt-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.boltapp.com/v1/oauth/authorize\n    tokenUrl: https://api.boltapp.com/v1/oauth/token\n  description: |-\n    Bolt utilizes the OAuth flow that developers can use to attain access to Bolt Account data via APIs.\n    For all APIs that require authorization, please provide your `access_token` returned from `/v1/oauth/token` via the basic auth bearer header `Authorization: bearer ${TOKEN}`.\n    [Read more about the OAuth token endpoint.](/api-bolt/#tag/OAuth)\n- name: OAuth\n  source: openapi/bolt-financial-embeddable-checkout-v1-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.boltapp.com/v1/oauth/authorize\n    tokenUrl: https://api.boltapp.com/v1/oauth/token\n  description: |-\n    Bolt utilizes the OAuth flow that developers can use to attain access to Bolt Account data via APIs.\n    For all APIs that require authorization, please provide your `access_token` returned from `/v1/oauth/token` via the basic auth bearer header `Authorization: bearer ${TOKEN}`.\n    [Read more about the OAuth token endpoint.](/api-bolt/#tag/OAuth)\n- name: oauth\n  source: openapi/bolt-financial-embeddable-checkout-v3-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\nscopes:\n- scope: bolt.account.manage\n  description: This scope grants permissions to perform read/edit/delete actions on Bolt Account\n    data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bolt-financial-bolt-api-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v1-openapi.yml\n\
  \  - openapi/bolt-financial-embeddable-checkout-v3-openapi.yml\n- scope: bolt.account.view\n  description: This scope grants permissions to perform read only actions on Bolt Account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bolt-financial-bolt-api-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v1-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v3-openapi.yml\n- scope: openid\n  description: This scope grants permissions that enable Bolt SSO by granting an id token JWT\n    that stores account data. Not used in v1/account endpoints\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bolt-financial-bolt-api-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v1-openapi.yml\n  - openapi/bolt-financial-embeddable-checkout-v3-openapi.yml\n\n- scope: email\n  description: Advertised by the Bolt OIDC discovery document; not declared in any published\n    OpenAPI security scheme.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.boltapp.com/.well-known/openid-configuration\n\
  \nx-evidence:\n  fetched: '2026-07-31'\n  openid_configuration:\n    url: https://api.boltapp.com/.well-known/openid-configuration\n    http_status: 200\n    scopes_supported:\n    - openid\n    - email\n    - bolt.account.manage\n    - bolt.account.view\n  note: The OIDC discovery document advertises an `email` scope that the OpenAPI security\n    schemes do not declare; the three spec-declared scopes are listed above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/scopes/bolt-financial-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Payments
- Checkout
- eCommerce
- Fintech
- Subscriptions
- Tokenization
- Fraud
- Identity
- Webhooks
token_urls:
- https://api.boltapp.com/v1/oauth/token
- /v1/oauth/token
---
