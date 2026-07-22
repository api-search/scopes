---
api_specs:
- filename: very-good-security-vault-openapi-original.yml
  format: yaml
  label: VGS Vault HTTP API
  slug: vgs-vault-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/very-good-security/refs/heads/main/openapi/very-good-security-vault-openapi-original.yml
authorization_urls: []
description: ''
docs: https://docs.verygoodsecurity.com/vault/developer-tools/apis/vault-api/authentication-and-authorization
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Very Good Security Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Very Good Security publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Very Good Security API on a user''s behalf.


  Tokens are issued from https://auth.verygoodsecurity.com/auth/realms/vgs/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Very Good Security
provider_slug: very-good-security
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.verygoodsecurity.com/auth/realms/vgs/protocol/openid-connect/token
  name: OAuth2 client credentials (vgs realm)
  source: https://auth.verygoodsecurity.com/auth/realms/vgs/.well-known/openid-configuration
scope_count: 3
scope_names:
- aliases:read
- aliases:write
- aliases:delete
scopes:
- description: read the entire vault data object using the associated alias
  flows:
  - clientCredentials
  scope: aliases:read
- description: create new aliases by value
  flows:
  - clientCredentials
  scope: aliases:write
- description: delete any alias
  flows:
  - clientCredentials
  scope: aliases:delete
slug: very-good-security-scopes
source_filename: very-good-security-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.verygoodsecurity.com/vault/developer-tools/apis/vault-api/authentication-and-authorization\ndocs: https://docs.verygoodsecurity.com/vault/developer-tools/apis/vault-api/authentication-and-authorization\nnotes: >-\n  The harvested Vault HTTP API OpenAPI declares only basic auth, so nothing was\n  derivable from the spec; these scopes come from the Vault API auth docs and the\n  live Keycloak OIDC discovery document (well-known/very-good-security-openid-configuration.json),\n  whose scopes_supported lists 150+ platform scopes. Documented Vault API scopes\n  are below; credentials must also be assigned to specific vaults or requests\n  return 401 even with correct scopes.\nschemes:\n- name: OAuth2 client credentials (vgs realm)\n  source: https://auth.verygoodsecurity.com/auth/realms/vgs/.well-known/openid-configuration\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.verygoodsecurity.com/auth/realms/vgs/protocol/openid-connect/token\n\
  scopes:\n- scope: aliases:read\n  description: read the entire vault data object using the associated alias\n  flows: [clientCredentials]\n- scope: aliases:write\n  description: create new aliases by value\n  flows: [clientCredentials]\n- scope: aliases:delete\n  description: delete any alias\n  flows: [clientCredentials]\nplatform_scope_registry:\n  source: well-known/very-good-security-openid-configuration.json\n  count: 150+\n  examples:\n  - routes:read\n  - routes:write\n  - vaults:read\n  - vaults:write\n  - credentials:read\n  - credentials:write\n  - network-tokens:read\n  - network-tokens:write\n  - cards:read\n  - cards:write\n  - cards:read-pci\n  - 3ds:read\n  - 3ds:write\n  - access-logs:read\n  - audit-logs:read\n  - certificates:read\n  - certificates:write\n  - account-validations:read\n  - account-validations:write\n  - financial-instruments:read\n  - financial-instruments:write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/very-good-security/refs/heads/main/scopes/very-good-security-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Company
- Data Security
- Tokenization
- Payments
- Vault
- PCI Compliance
- Data Privacy
- Card Management
- Network Tokens
- Security
token_urls:
- https://auth.verygoodsecurity.com/auth/realms/vgs/protocol/openid-connect/token
---
