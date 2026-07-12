---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Key Vault Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Key Vault publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Key Vault API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schemes:
- description: Azure Active Directory OAuth2 authentication. Requires an access token scoped to the Key Vault resource.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/azure-key-vault-data-plane-openapi.yml
scope_count: 1
scope_names:
- https://vault.azure.net/.default
scopes:
- description: Access Azure Key Vault
  flows:
  - implicit
  scope: https://vault.azure.net/.default
slug: microsoft-azure-key-vault-scopes
source_filename: microsoft-azure-key-vault-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-key-vault-data-plane-openapi.yml\nschemes:\n- name: OAuth2Auth\n  source: openapi/azure-key-vault-data-plane-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 authentication. Requires an access token scoped\n    to the Key Vault resource.\nscopes:\n- scope: https://vault.azure.net/.default\n  description: Access Azure Key Vault\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-key-vault-data-plane-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/scopes/microsoft-azure-key-vault-scopes.yml
summary_line: 1 scope · implicit
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
token_urls: []
---
