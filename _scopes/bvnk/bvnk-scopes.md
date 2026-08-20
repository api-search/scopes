---
api_specs:
- filename: bvnk-address-api-openapi.yml
  format: yaml
  label: BVNK Address API
  slug: bvnk-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-address-api-openapi.yml
- filename: bvnk-asset-pool-api-openapi.yml
  format: yaml
  label: BVNK Asset Pool API
  slug: bvnk-asset-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-asset-pool-api-openapi.yml
- filename: bvnk-channels-api-openapi.yml
  format: yaml
  label: BVNK Channels API
  slug: bvnk-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-channels-api-openapi.yml
- filename: bvnk-currencies-api-openapi.yml
  format: yaml
  label: BVNK Currencies API
  slug: bvnk-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-currencies-api-openapi.yml
- filename: bvnk-export-api-openapi.yml
  format: yaml
  label: BVNK Export API
  slug: bvnk-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-export-api-openapi.yml
- filename: bvnk-fee-api-openapi.yml
  format: yaml
  label: BVNK Fee API
  slug: bvnk-fee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-fee-api-openapi.yml
- filename: bvnk-key-pair-api-openapi.yml
  format: yaml
  label: BVNK Key Pair API
  slug: bvnk-key-pair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-key-pair-api-openapi.yml
- filename: bvnk-merchant-ids-api-openapi.yml
  format: yaml
  label: BVNK Merchant IDs API
  slug: bvnk-merchant-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-merchant-ids-api-openapi.yml
- filename: bvnk-network-api-openapi.yml
  format: yaml
  label: BVNK Network API
  slug: bvnk-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-network-api-openapi.yml
- filename: bvnk-payments-api-openapi.yml
  format: yaml
  label: BVNK Payments API
  slug: bvnk-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-payments-api-openapi.yml
- filename: bvnk-return-api-openapi.yml
  format: yaml
  label: BVNK Return API
  slug: bvnk-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-return-api-openapi.yml
- filename: bvnk-screening-api-openapi.yml
  format: yaml
  label: BVNK Screening API
  slug: bvnk-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-screening-api-openapi.yml
- filename: bvnk-trading-and-conversions-api-openapi.yml
  format: yaml
  label: BVNK Trading and Conversions API
  slug: bvnk-trading-and-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-trading-and-conversions-api-openapi.yml
- filename: bvnk-transaction-api-openapi.yml
  format: yaml
  label: BVNK Transaction API
  slug: bvnk-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-transaction-api-openapi.yml
- filename: bvnk-transaction-request-api-openapi.yml
  format: yaml
  label: BVNK Transaction Request API
  slug: bvnk-transaction-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-transaction-request-api-openapi.yml
- filename: bvnk-wallets-api-openapi.yml
  format: yaml
  label: BVNK Wallets API
  slug: bvnk-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-wallets-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.layer1.com/reference/api-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Bvnk Scopes
name_suffix: OAuth Scopes
note: Scopes are published anonymously by the BVNK Keycloak realm "bvnk" via OIDC discovery on both the production (auth.layer1.com) and sandbox (auth.sandbox.layer1.com) issuers. The Layer1 Digital Asset OpenAPI declares an oauth2 clientCredentials scheme with an empty scopes map, so the per-operation scopes below were recovered from operation security[] requirements in that spec and from the discovery document. One spec entry is an unresolved build placeholder (${exports.read-scope:exports:view}) and is recorded as a defect rather than a scope.
overview: 'BVNK publishes 156 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BVNK API on a user''s behalf.


  Tokens are issued from https://auth.layer1.com/auth/realms/bvnk/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BVNK
provider_slug: bvnk
schemes:
- flows:
  - flow: clientCredentials
    sandboxTokenUrl: https://auth.sandbox.layer1.com/auth/realms/bvnk/protocol/openid-connect/token
    tokenUrl: https://auth.layer1.com/auth/realms/bvnk/protocol/openid-connect/token
  grant_types:
  - authorization_code
  - client_credentials
  - implicit
  - password
  - refresh_token
  - urn:ietf:params:oauth:grant-type:card-sensitive-details-token-exchange
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:uma-ticket
  - urn:openid:params:grant-type:ciba
  name: oauth2
  source: openapi/bvnk-layer1-digital-asset-openapi-original.yml
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
scope_count: 156
scope_names:
- NetworkWhitelist
- account:edit
- account:view
- acr
- address
- addresses:admin
- addresses:edit
- addresses:view
- ai:assistants:edit
- ai:assistants:view
- ai:knowledgebases:edit
- ai:knowledgebases:view
- ai:query
- ai:tools:edit
- ai:tools:view
- approval-settings:edit
- approval-settings:view
- approvals:edit
- asset-pools:admin
- asset-pools:consolidation
- asset-pools:edit
- asset-pools:support
- asset-pools:view
- asset:edit
- balance-adjustments:edit
- basic
- book-entries:edit
- book-entries:view
- books:admin
- books:edit
- books:view
- bvnk-api-gateway-audience
- bvnk-centrifugo-audience
- bvnk-trino-audience
- bvnk:tenantId
- card:admin
- card:edit
- card:view
- channel-payments:view
- channels-admin:edit
- channels-admin:view
- channels:edit
- channels:view
- clients:edit
- clients:view
- configuration:compliance:edit
- configuration:compliance:view
- configuration:digital:edit
- configuration:digital:view
- configuration:feature-flags:edit
- configuration:feature-flags:view
- configuration:trade:edit
- configuration:trade:view
- contacts:edit
- contacts:view
- conversions:edit
- conversions:view
- cross-border-payments:edit
- cross-border-payments:view
- cross-border-templates:view
- email
- exchange-rates:view
- exports:edit
- exports:view
- failing-configurations:edit
- failing-configurations:view
- fee-estimate:edit
- fee:configuration:edit
- fee:configuration:view
- fee:edit
- hook-destinations:edit
- hook-destinations:view
- hook-events:view
- hook-webhooks:edit
- hook:admin
- identity-broker-login
- identity-user:action
- identity-user:edit
- identity-user:view
- integration-admin:signing-keys:edit
- integration-admin:signing-keys:view
- kc_idp_hint
- keypairs:edit
- keypairs:view
- layer1:opa:admin
- layer1:scope:roles
- ledger:admin
- merchant-settings:edit
- merchant-settings:view
- microprofile-jwt
- networks:edit
- networks:view
- offline_access
- openid
- organization
- payment-admin:edit
- payment-admin:view
- payment-instruments:edit
- payment-instruments:view
- payment:edit
- payment:view
- phone
- profile
- quote:edit
- quote:view
- report:view
- risk-warehouse:configuration:edit
- risk-warehouse:configuration:view
- roles
- screenings:edit
- screenings:override
- screenings:remediate
- screenings:view
- secrets:edit
- secrets:view
- service_account
- staking-transactions:edit
- superset:edit
- superset:view
- symbol:edit
- symbol:view
- tenant-user:authz
- tenants-vault:edit
- tenants:edit
- tenants:view
- tokenisation:edit
- tokenisation:view
- trade-admin:edit
- trade-settings:edit
- trade-settings:view
- trade:exports:edit
- trade:exports:view
- trade:quote-service:quotes:edit
- trade:quote-service:quotes:view
- transaction-claims:edit
- transactions:edit
- transactions:view
- treasury:admin
- treasury:edit
- treasury:settlement:edit
- treasury:settlement:view
- treasury:view
- venue-balances:view
- venue-deposit-addresses:edit
- venue-deposit-addresses:view
- venue-transfer:edit
- venue-transfer:view
- wallet:edit
- wallet:view
- web-origins
- webhook:edit
- webhook:view
- workflow-orchestrator:admin
- workflow:edit
- workflow:execute
- workflow:view
scopes:
- description: ''
  flows: []
  scope: NetworkWhitelist
- description: ''
  flows: []
  scope: account:edit
- description: ''
  flows: []
  scope: account:view
- description: ''
  flows: []
  scope: acr
- description: ''
  flows: []
  scope: address
- description: ''
  flows: []
  scope: addresses:admin
- description: ''
  flows: []
  scope: addresses:edit
- description: ''
  flows: []
  scope: addresses:view
- description: ''
  flows: []
  scope: ai:assistants:edit
- description: ''
  flows: []
  scope: ai:assistants:view
- description: ''
  flows: []
  scope: ai:knowledgebases:edit
- description: ''
  flows: []
  scope: ai:knowledgebases:view
- description: ''
  flows: []
  scope: ai:query
- description: ''
  flows: []
  scope: ai:tools:edit
- description: ''
  flows: []
  scope: ai:tools:view
- description: ''
  flows: []
  scope: approval-settings:edit
- description: ''
  flows: []
  scope: approval-settings:view
- description: ''
  flows: []
  scope: approvals:edit
- description: ''
  flows: []
  scope: asset-pools:admin
- description: ''
  flows: []
  scope: asset-pools:consolidation
- description: ''
  flows: []
  scope: asset-pools:edit
- description: ''
  flows: []
  scope: asset-pools:support
- description: ''
  flows: []
  scope: asset-pools:view
- description: ''
  flows: []
  scope: asset:edit
- description: ''
  flows: []
  scope: balance-adjustments:edit
- description: ''
  flows: []
  scope: basic
- description: ''
  flows: []
  scope: book-entries:edit
- description: ''
  flows: []
  scope: book-entries:view
- description: ''
  flows: []
  scope: books:admin
- description: ''
  flows: []
  scope: books:edit
- description: ''
  flows: []
  scope: books:view
- description: ''
  flows: []
  scope: bvnk-api-gateway-audience
- description: ''
  flows: []
  scope: bvnk-centrifugo-audience
- description: ''
  flows: []
  scope: bvnk-trino-audience
- description: ''
  flows: []
  scope: bvnk:tenantId
- description: ''
  flows: []
  scope: card:admin
- description: ''
  flows: []
  scope: card:edit
- description: ''
  flows: []
  scope: card:view
- description: ''
  flows: []
  scope: channel-payments:view
- description: ''
  flows: []
  scope: channels-admin:edit
- description: ''
  flows: []
  scope: channels-admin:view
- description: ''
  flows: []
  scope: channels:edit
- description: ''
  flows: []
  scope: channels:view
- description: ''
  flows: []
  scope: clients:edit
- description: ''
  flows: []
  scope: clients:view
- description: ''
  flows: []
  scope: configuration:compliance:edit
- description: ''
  flows: []
  scope: configuration:compliance:view
- description: ''
  flows: []
  scope: configuration:digital:edit
- description: ''
  flows: []
  scope: configuration:digital:view
- description: ''
  flows: []
  scope: configuration:feature-flags:edit
- description: ''
  flows: []
  scope: configuration:feature-flags:view
- description: ''
  flows: []
  scope: configuration:trade:edit
- description: ''
  flows: []
  scope: configuration:trade:view
- description: ''
  flows: []
  scope: contacts:edit
- description: ''
  flows: []
  scope: contacts:view
- description: ''
  flows: []
  scope: conversions:edit
- description: ''
  flows: []
  scope: conversions:view
- description: ''
  flows: []
  scope: cross-border-payments:edit
- description: ''
  flows: []
  scope: cross-border-payments:view
- description: ''
  flows: []
  scope: cross-border-templates:view
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: exchange-rates:view
- description: ''
  flows: []
  scope: exports:edit
- description: ''
  flows: []
  scope: exports:view
- description: ''
  flows: []
  scope: failing-configurations:edit
- description: ''
  flows: []
  scope: failing-configurations:view
- description: ''
  flows: []
  scope: fee-estimate:edit
- description: ''
  flows: []
  scope: fee:configuration:edit
- description: ''
  flows: []
  scope: fee:configuration:view
- description: ''
  flows: []
  scope: fee:edit
- description: ''
  flows: []
  scope: hook-destinations:edit
- description: ''
  flows: []
  scope: hook-destinations:view
- description: ''
  flows: []
  scope: hook-events:view
- description: ''
  flows: []
  scope: hook-webhooks:edit
- description: ''
  flows: []
  scope: hook:admin
- description: ''
  flows: []
  scope: identity-broker-login
- description: ''
  flows: []
  scope: identity-user:action
- description: ''
  flows: []
  scope: identity-user:edit
- description: ''
  flows: []
  scope: identity-user:view
- description: ''
  flows: []
  scope: integration-admin:signing-keys:edit
- description: ''
  flows: []
  scope: integration-admin:signing-keys:view
- description: ''
  flows: []
  scope: kc_idp_hint
- description: ''
  flows: []
  scope: keypairs:edit
- description: ''
  flows: []
  scope: keypairs:view
- description: ''
  flows: []
  scope: layer1:opa:admin
- description: ''
  flows: []
  scope: layer1:scope:roles
- description: ''
  flows: []
  scope: ledger:admin
- description: ''
  flows: []
  scope: merchant-settings:edit
- description: ''
  flows: []
  scope: merchant-settings:view
- description: ''
  flows: []
  scope: microprofile-jwt
- description: ''
  flows: []
  scope: networks:edit
- description: ''
  flows: []
  scope: networks:view
- description: ''
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: organization
- description: ''
  flows: []
  scope: payment-admin:edit
- description: ''
  flows: []
  scope: payment-admin:view
- description: ''
  flows: []
  scope: payment-instruments:edit
- description: ''
  flows: []
  scope: payment-instruments:view
- description: ''
  flows: []
  scope: payment:edit
- description: ''
  flows: []
  scope: payment:view
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: quote:edit
- description: ''
  flows: []
  scope: quote:view
- description: ''
  flows: []
  scope: report:view
- description: ''
  flows: []
  scope: risk-warehouse:configuration:edit
- description: ''
  flows: []
  scope: risk-warehouse:configuration:view
- description: ''
  flows: []
  scope: roles
- description: ''
  flows: []
  scope: screenings:edit
- description: ''
  flows: []
  scope: screenings:override
- description: ''
  flows: []
  scope: screenings:remediate
- description: ''
  flows: []
  scope: screenings:view
- description: ''
  flows: []
  scope: secrets:edit
- description: ''
  flows: []
  scope: secrets:view
- description: ''
  flows: []
  scope: service_account
- description: ''
  flows: []
  scope: staking-transactions:edit
- description: ''
  flows: []
  scope: superset:edit
- description: ''
  flows: []
  scope: superset:view
- description: ''
  flows: []
  scope: symbol:edit
- description: ''
  flows: []
  scope: symbol:view
- description: ''
  flows: []
  scope: tenant-user:authz
- description: ''
  flows: []
  scope: tenants-vault:edit
- description: ''
  flows: []
  scope: tenants:edit
- description: ''
  flows: []
  scope: tenants:view
- description: ''
  flows: []
  scope: tokenisation:edit
- description: ''
  flows: []
  scope: tokenisation:view
- description: ''
  flows: []
  scope: trade-admin:edit
- description: ''
  flows: []
  scope: trade-settings:edit
- description: ''
  flows: []
  scope: trade-settings:view
- description: ''
  flows: []
  scope: trade:exports:edit
- description: ''
  flows: []
  scope: trade:exports:view
- description: ''
  flows: []
  scope: trade:quote-service:quotes:edit
- description: ''
  flows: []
  scope: trade:quote-service:quotes:view
- description: ''
  flows: []
  scope: transaction-claims:edit
- description: ''
  flows: []
  scope: transactions:edit
- description: ''
  flows: []
  scope: transactions:view
- description: ''
  flows: []
  scope: treasury:admin
- description: ''
  flows: []
  scope: treasury:edit
- description: ''
  flows: []
  scope: treasury:settlement:edit
- description: ''
  flows: []
  scope: treasury:settlement:view
- description: ''
  flows: []
  scope: treasury:view
- description: ''
  flows: []
  scope: venue-balances:view
- description: ''
  flows: []
  scope: venue-deposit-addresses:edit
- description: ''
  flows: []
  scope: venue-deposit-addresses:view
- description: ''
  flows: []
  scope: venue-transfer:edit
- description: ''
  flows: []
  scope: venue-transfer:view
- description: ''
  flows: []
  scope: wallet:edit
- description: ''
  flows: []
  scope: wallet:view
- description: ''
  flows: []
  scope: web-origins
- description: ''
  flows: []
  scope: webhook:edit
- description: ''
  flows: []
  scope: webhook:view
- description: ''
  flows: []
  scope: workflow-orchestrator:admin
- description: ''
  flows: []
  scope: workflow:edit
- description: ''
  flows: []
  scope: workflow:execute
- description: ''
  flows: []
  scope: workflow:view
slug: bvnk-scopes
source_filename: bvnk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://auth.layer1.com/auth/realms/bvnk/.well-known/openid-configuration\ndocs: https://docs.layer1.com/reference/api-authentication\nnote: Scopes are published anonymously by the BVNK Keycloak realm \"bvnk\" via OIDC discovery on both the\n  production (auth.layer1.com) and sandbox (auth.sandbox.layer1.com) issuers. The Layer1 Digital Asset\n  OpenAPI declares an oauth2 clientCredentials scheme with an empty scopes map, so the per-operation scopes\n  below were recovered from operation security[] requirements in that spec and from the discovery document.\n  One spec entry is an unresolved build placeholder (${exports.read-scope:exports:view}) and is recorded\n  as a defect rather than a scope.\nissuers:\n- environment: production\n  issuer: https://auth.layer1.com/auth/realms/bvnk\n  discovery: https://auth.layer1.com/auth/realms/bvnk/.well-known/openid-configuration\n  file: well-known/bvnk-openid-configuration.json\n  http_status:\
  \ 200\n- environment: sandbox\n  issuer: https://auth.sandbox.layer1.com/auth/realms/bvnk\n  discovery: https://auth.sandbox.layer1.com/auth/realms/bvnk/.well-known/openid-configuration\n  file: well-known/bvnk-sandbox-openid-configuration.json\n  http_status: 200\nschemes:\n- name: oauth2\n  source: openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.layer1.com/auth/realms/bvnk/protocol/openid-connect/token\n    sandboxTokenUrl: https://auth.sandbox.layer1.com/auth/realms/bvnk/protocol/openid-connect/token\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:card-sensitive-details-token-exchange\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n\
  \  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\nscope_count: 156\nscopes:\n- scope: NetworkWhitelist\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: account:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: account:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: acr\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: address\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: addresses:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: addresses:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: addresses:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n\
  \  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: ai:assistants:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: ai:assistants:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: ai:knowledgebases:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: ai:knowledgebases:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: ai:query\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: ai:tools:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: ai:tools:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: approval-settings:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: approval-settings:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n\
  - scope: approvals:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: asset-pools:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: asset-pools:consolidation\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: asset-pools:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: asset-pools:support\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: asset-pools:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: asset:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: balance-adjustments:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n\
  - scope: basic\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: book-entries:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: book-entries:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: books:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: books:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: books:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: bvnk-api-gateway-audience\n  kind: audience\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: bvnk-centrifugo-audience\n  kind: audience\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: bvnk-trino-audience\n  kind: audience\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: bvnk:tenantId\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n\
  - scope: card:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: card:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: card:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: channel-payments:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: channels-admin:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: channels-admin:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: channels:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: channels:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: clients:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: clients:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n\
  - scope: configuration:compliance:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: configuration:compliance:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: configuration:digital:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: configuration:digital:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: configuration:feature-flags:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: configuration:feature-flags:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: configuration:trade:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: configuration:trade:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: contacts:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n\
  - scope: contacts:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: conversions:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: conversions:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: cross-border-payments:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: cross-border-payments:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: cross-border-templates:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: email\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: exchange-rates:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: exports:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n\
  \  in_spec: true\n- scope: exports:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: failing-configurations:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: failing-configurations:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: fee-estimate:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: fee:configuration:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: fee:configuration:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: fee:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: hook-destinations:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: hook-destinations:view\n  kind: platform\n\
  \  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: hook-events:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: hook-webhooks:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: hook:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: identity-broker-login\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: identity-user:action\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: identity-user:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: identity-user:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: integration-admin:signing-keys:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: integration-admin:signing-keys:view\n  kind: platform\n  sources:\n\
  \  - well-known/bvnk-openid-configuration.json\n- scope: kc_idp_hint\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: keypairs:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: keypairs:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: layer1:opa:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: layer1:scope:roles\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: ledger:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: merchant-settings:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: merchant-settings:view\n  kind: platform\n  sources:\n  -\
  \ well-known/bvnk-openid-configuration.json\n- scope: microprofile-jwt\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: networks:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: networks:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: offline_access\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: openid\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: organization\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: payment-admin:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: payment-admin:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: payment-instruments:edit\n  kind: platform\n\
  \  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: payment-instruments:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: payment:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: payment:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: phone\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: profile\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: quote:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: quote:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: report:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: risk-warehouse:configuration:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: risk-warehouse:configuration:view\n\
  \  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: roles\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: screenings:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: screenings:override\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: screenings:remediate\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: screenings:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: secrets:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: secrets:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: service_account\n  kind: standard-oidc\n\
  \  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: staking-transactions:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: superset:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: superset:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: symbol:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: symbol:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: tenant-user:authz\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: tenants-vault:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: tenants:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: tenants:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: tokenisation:edit\n\
  \  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: tokenisation:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: trade-admin:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: trade-settings:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: trade-settings:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: trade:exports:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: trade:exports:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: trade:quote-service:quotes:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: trade:quote-service:quotes:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: transaction-claims:edit\n  kind: platform\n\
  \  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: transactions:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: transactions:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n  - openapi/bvnk-layer1-digital-asset-openapi-original.yml\n  in_spec: true\n- scope: treasury:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: treasury:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: treasury:settlement:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: treasury:settlement:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: treasury:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: venue-balances:view\n  kind: platform\n\
  \  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: venue-deposit-addresses:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: venue-deposit-addresses:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: venue-transfer:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: venue-transfer:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: wallet:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: wallet:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: web-origins\n  kind: standard-oidc\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: webhook:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: webhook:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n\
  - scope: workflow-orchestrator:admin\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: workflow:edit\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: workflow:execute\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\n- scope: workflow:view\n  kind: platform\n  sources:\n  - well-known/bvnk-openid-configuration.json\ndefects:\n- scope: ${exports.read-scope:exports:view}\n  issue: unresolved build-time placeholder shipped in the published OpenAPI security requirement\n  source: openapi/bvnk-layer1-digital-asset-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/scopes/bvnk-scopes.yml
summary_line: 156 scopes · clientCredentials
tags:
- Company
- Payments
- Stablecoins
- Cryptocurrency
- Wallets
- Virtual Accounts
- Cross-Border Payments
- Financial-Services
- Cards
- Digital Assets
- Banking
- Compliance
token_urls:
- https://auth.layer1.com/auth/realms/bvnk/protocol/openid-connect/token
---
