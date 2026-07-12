---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bitwarden Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bitwarden publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bitwarden API on a user''s behalf.


  Tokens are issued from https://identity.bitwarden.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bitwarden
provider_slug: bitwarden
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://identity.bitwarden.com/connect/token
  name: OAuth2 Client Credentials
  source: openapi/bitwarden-public-swagger.json
scope_count: 1
scope_names:
- api.organization
scopes:
- description: Organization APIs
  flows:
  - clientCredentials
  scope: api.organization
slug: bitwarden-scopes
source_filename: bitwarden-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitwarden-public-swagger.json\nschemes:\n- name: OAuth2 Client Credentials\n  source: openapi/bitwarden-public-swagger.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.bitwarden.com/connect/token\nscopes:\n- scope: api.organization\n  description: Organization APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bitwarden-public-swagger.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitwarden/refs/heads/main/scopes/bitwarden-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Security
- Password Manager
- Open Source
- Vault
- Identity
- SCIM
token_urls:
- https://identity.bitwarden.com/connect/token
---
